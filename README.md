<!DOCTYPE html>
<html>
<head>
<script>
function getOption() {
    var obj = document.getElementById("mySelect");
    var num=document.getElementById("frm1").elements[0];
    var name=document.getElementById("frm1").elements[1];
    var coffee = document.forms[0];
    var txt = "";
    var i;
    for (i = 0; i < coffee.length; i++) {
        if (coffee[i].checked) {
            txt = txt + coffee[i].value + " ";
        }
    }
    document.getElementById("order").innerHTML = num.value+name.value+' '+obj.options[obj.selectedIndex].text+' '+txt;
        
}
</script>
</head>
<body>

<p>트레이드요정!:</p>

<form id="frm1" action="/action_page.php">
학번: <input type="text"  id="fnum" name="fnum"><br>
이름: <input type="text" name="fname"><br><br>
트레이드를 원하는 과목을 고르세요:
<select id="mySelect">
  <option>체육2</option>
  <option>체육4</option>
  <option>체육6</option>
  <option>창의수학</option>
</select>
<br><br>
현재분반을 고르세요<br>
<input type="checkbox" name="coffee" id="none" value='1'>1분반
<input type="checkbox" name="coffee" id="ntwo"value='2'>2분반
<input type="checkbox" name="coffee" id="ntri"value='3'>3분반
<input type="checkbox" name="coffee" id="nfor"value='4'>4분반
<input type="checkbox" name="coffee" id="nfiv"value='5'>5분반
<input type="checkbox" name="coffee" id="nsix"value='6'>6분반
<input type="checkbox" name="coffee" id="nsev"value='7'>7분반<br>
<br>
가고 싶은 분반을 고르세요<br>
[ ]1분반
<input type="checkbox" name="coffee2" id="wtwo"value='2'>2분반
<input type="checkbox" name="coffee2" id="wtri"value='3'>3분반
<input type="checkbox" name="coffee2" id="wfor"value='4'>4분반
<input type="checkbox" name="coffee2" id="wfiv"value='5'>5분반
<input type="checkbox" name="coffee2" id="wsix"value='6'>6분반
<input type="checkbox" name="coffee2" id="wsev"value='7'>7분반<br>
<br><input type="button" id='hw'onclick="getOption()" value="저장하기">
<script type="text/javascript" src="save.js"></script>
<br><br>
</form>

<p id="order"></p>
<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://mydspro.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
</body>
</html>
