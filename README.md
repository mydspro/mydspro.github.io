## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/mydspro/mydspro.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

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
<input type="checkbox" name="coffee2" id="wone"value='1'>1분반
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

</body>
</html>


# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/mydspro/mydspro.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
