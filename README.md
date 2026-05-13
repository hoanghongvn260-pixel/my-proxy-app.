<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gửi Người Thương</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #ffc0cb; /* Màu hồng nhạt */
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            overflow: hidden;
        }

        .container {
            text-align: center;
        }

        /* Hiệu ứng trái tim đập */
        .heart {
            background-color: red;
            display: inline-block;
            height: 100px;
            margin: 0 10px;
            position: relative;
            top: 0;
            transform: rotate(-45deg);
            width: 100px;
            animation: beat .8s infinite;
        }

        .heart:before,
        .heart:after {
            content: "";
            background-color: red;
            border-radius: 50%;
            height: 100px;
            position: absolute;
            width: 100px;
        }

        .heart:before {
            top: -50px;
            left: 0;
        }

        .heart:after {
            left: 50px;
            top: 0;
        }

        @keyframes beat {
            0% { transform: scale(1) rotate(-45deg); }
            50% { transform: scale(1.2) rotate(-45deg); }
            100% { transform: scale(1) rotate(-45deg); }
        }

        h1 {
            color: #d00000;
            margin-top: 50px;
            font-size: 24px;
            text-shadow: 1px 1px 2px white;
        }

        .message {
            background: rgba(255, 255, 255, 0.8);
            padding: 15px;
            border-radius: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            color: #333;
            max-width: 300px;
            margin: 20px auto;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="heart"></div>
        <h1>Yêu Em Nhiều Lắm ❤️</h1>
        <div class="message">
            Cảm ơn em đã luôn ở bên cạnh anh. Tặng em món quà nhỏ do chính tay anh code nè! 
        </div>
    </div>

</body>
</html>
