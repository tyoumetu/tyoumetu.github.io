<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>創作資料庫</title>

<style>

body{
    margin:0;
    font-family:sans-serif;
    color:white;
    min-height:100vh;

    background-color:#070b14;

    background-image:
        linear-gradient(
            rgba(0,255,255,0.08) 1px,
            transparent 1px
        ),
        linear-gradient(
            90deg,
            rgba(0,255,255,0.08) 1px,
            transparent 1px
        ),
        radial-gradient(
            circle at center,
            #13213d,
            #070b14 70%
        );

    background-size:
        50px 50px,
        50px 50px,
        cover;
}

header{
    text-align:center;
    padding:25px;
    background:rgba(0,0,0,0.75);
    border-bottom:2px solid #00ffff;
    box-shadow:0 0 20px rgba(0,255,255,0.5);
}

header h1{
    margin:0;
    color:#00ffff;
    letter-spacing:5px;
    text-shadow:
        0 0 5px #00ffff,
        0 0 15px #00ffff;
}

#character1{
    position:fixed;
    bottom:20px;
    left:-100px;
    z-index:1000;

    animation:
        walkRight 20s linear infinite;
}

#character2{
    position:fixed;
    bottom:100px;
    right:-100px;
    z-index:1000;

    animation:
        walkLeft 15s linear infinite;
}

#character1 img,
#character2 img{
    width:64px;
    image-rendering:pixelated;
}

@keyframes walkRight{
    0%{
        left:-100px;
    }

    100%{
        left:calc(100vw + 100px);
    }
}

@keyframes walkLeft{
    0%{
        right:-100px;
    }

    100%{
        right:calc(100vw + 100px);
    }
}

.container{
    max-width:900px;
    margin:auto;
    padding:30px;
}

#content{
    display:none;
}

.card{
    background:rgba(10,20,30,0.85);
    border:1px solid #00ffff55;
    border-radius:12px;
    padding:20px;
    margin-top:20px;
    box-shadow:0 0 15px rgba(0,255,255,0.15);
}

input[type="password"]{
    width:250px;
    padding:10px;
    border:none;
    border-radius:5px;
    outline:none;
}

button{
    padding:10px 18px;
    margin-top:10px;

    background:#102030;
    color:#00ffff;

    border:1px solid #00ffff;
    border-radius:5px;

    cursor:pointer;
    font-weight:bold;
}

button:hover{
    background:#00ffff;
    color:black;

    box-shadow:
        0 0 10px #00ffff,
        0 0 20px #00ffff;
}

.logout{
    border-color:#ff5555;
    color:#ff5555;
}

.logout:hover{
    background:#ff5555;
    color:white;
}

#message{
    color:#ff6666;
    margin-top:10px;
}

.status{
    color:#99ffff;
    font-size:14px;
}

@keyframes warningBlink {
    0%, 100% {
        opacity: 1;
        text-shadow: 0 0 15px red;
    }

    50% {
        opacity: 0.1;
        text-shadow: none;
    }
}

.warning {
    animation: warningBlink 0.7s infinite;
}

@keyframes warningBlink {
    0%, 100% {
        opacity: 1;
        text-shadow: 0 0 15px red;
    }
    50% {
        opacity: 0.15;
        text-shadow: none;
    }
}

.warning {
    color: red;
    animation: warningBlink 0.7s infinite;
}

/* 警告線 */
.warning-line {
    width: 80%;
    max-width: 600px;
    height: 4px;
    background: red;
    box-shadow: 0 0 10px red, 0 0 25px red;
    animation: lineBlink 0.7s infinite;
    margin: 25px 0;
}

@keyframes lineBlink {
    0%, 100% {
        opacity: 1;
        transform: scaleX(1);
    }
    50% {
        opacity: 0.2;
        transform: scaleX(0.85);
    }
}

</style>
</head>

<body>

<header>
    <h1>創作資料庫</h1>
</header>

<div class="container">

    <div id="login">

        <h2>アクセス認証</h2>

        <p>
            閲覧権限を確認しています。<br>
            パスワードを入力してください。
        </p>

        <input
            type="password"
            id="password"
            placeholder="Password">

        <br>

        <button onclick="login()">
            認証
        </button>

        <p id="message"></p>

    </div>


    <div id="content">

        <h2>ようこそ、仮想世界へ</h2>

        <p class="status">
            ACCESS GRANTED
        </p>

        <div id="character1">
    <img id="sprite1" src="walk1.png">
</div>

<div id="character2">
    <img id="sprite2" src="enemy1.png">
</div>
    


        <div class="card">

            <h3>📁 設定資料</h3>

            <p>
                すべての設定資料を収録
            </p>

            <button onclick="downloadFolder('世界観設定.zip')">
                資料を取得
            </button>

        </div>

        <button
            class="logout"
            onclick="logout()">
            ログアウト
        </button>

    </div>

    



</div>

<script>

const PASSWORD = "command";
const LOGIN_MINUTES = 1;

let failedCount = 0;
const MAX_TRIES = 3;

window.onload = () => {

    const expire =
        localStorage.getItem("loginExpire");

    if(
        expire &&
        Date.now() < Number(expire)
    ){
        showContent();
    }

    document
        .getElementById("password")
        .addEventListener(
            "keydown",
            function(e){

                if(e.key === "Enter"){
                    login();
                }

            }
        );

};

function login(){

    const password =
        document
        .getElementById("password")
        .value;

    if(password === PASSWORD){

        const expire =
    Date.now()
    + LOGIN_MINUTES
    * 60
    * 1000;

    localStorage.setItem(
        "loginExpire",
        expire
    );

        showContent();

    }else{
        failedCount++;

        document
        .getElementById("message")
        .textContent =
        "パスワードが違います";
        
         if(failedCount >= MAX_TRIES){

            document.body.innerHTML = `

            <div style="
                height:100vh;
                background:black;
                color:red;
                display:flex;
                flex-direction:column;
                justify-content:center;
                align-items:center;
                text-align:center;
                font-family:monospace;
            ">
            
             <h1>
                <span class="warning">
                    ⚠SECURITY ALERT⚠
                    </span>
            </h1>
            
            <div class="warning-line"></div>

                <p>
                <span class="warning">
                    不正アクセスを検知しました
                </span>
                </p>

                <p>
                <span class="warning">
                アクセスを遮断します
                </span>
                </p>
            <div class="warning-line"></div>

            </div>
            `;
        }
    }

}

function showContent(){

    document
        .getElementById("login")
        .style.display = "none";

    document
        .getElementById("content")
        .style.display = "block";

    if (expire) {

        setTimeout(() => {

            logout();

        }, expire - Date.now());

    }

}

function downloadFolder(file){

    const a =
        document.createElement("a");

    a.href = file;
    a.download = file;

    document.body.appendChild(a);

    a.click();

    document.body.removeChild(a);

}

function logout(){

    localStorage.removeItem(
        "loginExpire"
    );

    location.reload();

}

const frames1 = [
    "walk1.png",
    "walk2.png",
    "walk3.png",
    "walk4.png"
];

const frames2 = [
    "enemy1.png",
    "enemy2.png",
    "enemy3.png",
    "enemy4.png"
];

let frame1 = 0;
let frame2 = 0;

setInterval(() => {

    frame1 = (frame1 + 1) % frames1.length;
    frame2 = (frame2 + 1) % frames2.length;

    document.getElementById("sprite1").src =
        frames1[frame1];

    document.getElementById("sprite2").src =
        frames2[frame2];

}, 150);

function showContent(){

    document
        .getElementById("login")
        .style.display = "none";

    document
        .getElementById("content")
        .style.display = "block";

    const expire =
        Number(localStorage.getItem("loginExpire"));

    if(expire){
        setTimeout(() => {
            logout();
        }, expire - Date.now());
    }
}

</script>

</body>
</html>
