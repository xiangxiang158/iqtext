[智商测试.html](https://github.com/user-attachments/files/23120237/default.html)
<!doctype html>
<html lang="zh-CN">
<head>
<meta charset="utf-8">
<title>智商测试</title>
<style>
body{font-family:Arial,Helvetica,sans-serif;text-align:center;margin-top:10%}
input,button{font-size:1.2em;padding:.3em .6em;margin:.3em}
#out{color:#e91e63;font-size:1.4em;margin-top:1em}
</style>
</head>
<body>
<h2>测测你的智商</h2>
<input id="iq" type="number" placeholder="输入整数">
<button onclick="check()">开始测试</button>
<div id="out"></div>

<script>
// 把 Python 逻辑翻译成 JS，一样用
function check(){
    const a = Number(document.getElementById('iq').value);
    const out = document.getElementById('out');
    if(isNaN(a)) {out.innerText='请输入整数！'; return;}
    out.innerText = a<250 ? '连250都不如' : a===250 ? '有自知之明' : '自恋狂魔';
}
</script>
</body>
</html>
