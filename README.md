
<!DOCTYPE html>
<html>
<head>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        a {
            text-decoration: none;
        }

        .box {
            font-size: 20px;
            color: white;
            height: 250px;
            width: 350px;
            border-radius: 10px;
            background: #191919;
            flex-direction: column;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .buttons-container {
            display: flex;
            justify-content: space-around;
            height: 50px;
            width: 150px;
        }
        button {
            height: 30px;
            width: 150px;
            background: white;
            border-radius: 5px;
            color: blue;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <div class="box">
        <p>Fica comigo?</p>
        <div class="buttons-container">
            <button>
                <a href="https://wa.me/qr/ZVMRPS27YHHEF1">Sim</a>
            </button>
            <button id="no">Nao</button>
        </div>
    </div>
</body>
<script>
    let button = document.getElementById('no');
    let height = window.innerHeight - 50;
    let width = window.innerWidth - 50;

    button.addEventListener('mouseover', function () {
        button.style.position = "absolute";
        button.style.top = Math.random() * height + "px"
        button.style.left = Math.random() * width + "px"
    })
</script>
</html>
