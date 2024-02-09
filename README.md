<html>
<head>
    <style>
        body {
            background-image: url("https://th.bing.com/th/id/OIP.bVntZDkRww5bCDDsGoDTtgHaDt?w=296&h=175&c=7&r=0&o=5&dpr=1.3&pid=1.7");
            background-size: cover;
            filter: brightness(0.8);
        }
        h1 {
            color: yellow;
            text-align: center;
        }
        .icon {
            width: 100px;
            height: 100px;
            margin: 10px;
            display: inline-block;
        }
        .button {
            width: 200px;
            height: 100px;
            font-size: 40px;
            margin: 20px;
            position: relative;
        }
        #ok {
            background-color: green;
            color: white;
        }
        #no {
            background-color: blue;
            color: white;
        }
        .container {
            text-align: center;
        }
    </style>
    <script>
        function showAccount() {
            alert("Số tài khoản: 123456789\nNgân hàng: Vietcombank");
        }
        function moveButton() {
            var no = document.getElementById("no");
            var x = Math.floor(Math.random() * window.innerWidth - 200);
            var y = Math.floor(Math.random() * window.innerHeight - 100);
            no.style.left = x + "px";
            no.style.top = y + "px";
            var ok = document.getElementById("ok");
            ok.style.width = (parseInt(ok.style.width) * 2) + "px";
            ok.style.height = (parseInt(ok.style.height) * 2) + "px";
            ok.style.fontSize = (parseInt(ok.style.fontSize) * 2) + "px";
        }
    </script>
</head>
<body>
    <h1>Năm mới vui vẻ bạn lì xì cho mình nha</h1>
    
    <div class="container">
        <button id="ok" class="button" onclick="showAccount()">Ok</button>
        <button id="no" class="button" onclick="moveButton()">Đéo</button>
    </div>
</body>
</html>
