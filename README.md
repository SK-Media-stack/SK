<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8" />
<title>Football Control Panel Uploader</title>

<style>
body, html{
    margin:0; padding:0;
    width:100%; height:100%;
    overflow:hidden;
    background:rgba(0,0,0,0);
}
.container{
    width:100%;
    height:100%;
    display:flex;
    justify-content:center;
    align-items:center;
}
.box{
    width:600px; padding:20px;
    border:2px solid #444;
    background:#222;
    color:#fff;
    font-family:sans-serif;
}
button{
    padding:10px 20px;
    margin:5px;
    font-size:16px;
    cursor:pointer;
}
</style>

</head>
<body>

<div class="container">
    <div class="box">
        <h2>Football Control</h2>
        <button onclick="pressBtn('GOAL')">GOAL</button>
        <button onclick="pressBtn('HALF')">HALF</button>
        <button onclick="pressBtn('END')">END</button>

        <div id="log"></div>
    </div>
</div>

<script>
// demo handler
function pressBtn(type){
    let log = document.getElementById("log");
    let p = document.createElement("p");
    p.innerText = "Pressed: " + type;
    log.appendChild(p);
}
</script>

</body>
</html>
