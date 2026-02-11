<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Valentine 💖</title>
    <style>
        body {
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            overflow: hidden;
        }

        .box {
            text-align: center;
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        h1 {
            color: #ff3366;
        }

        button {
            padding: 10px 25px;
            font-size: 18px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin: 15px;
        }

        #yes {
            background: #28a745;
            color: white;
        }

        #no {
            background: #dc3545;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

<div class="box">
    <h1>Chandu ❤️</h1>
    <h2>Will you be my Valentine?</h2>
    <button id="yes" onclick="yesClicked()">Yes 💖</button>
</div>

<button id="no">No 💔</button>

<script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
        const x = Math.random() * (window.innerWidth - 100);
        const y = Math.random() * (window.innerHeight - 50);
        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    });

    function yesClicked() {
        document.body.innerHTML = `
            <div style="
                height:100vh;
                display:flex;
                justify-content:center;
                align-items:center;
                background:linear-gradient(135deg,#ff758c,#ff7eb3);
                color:white;
                font-family:Arial;
                text-align:center;
            ">
                <h1>Yayyy! 💕<br>Chandu is my Valentine 💖</h1>
            </div>
        `;
    }
</script>

</body>
</html>
