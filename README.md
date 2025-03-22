<!DOCTYPE html>
<html>
<head>
    <title>Motivation Button</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: lightgray;
        }

        #motivationButton {
            background-color: red;
            color: white;
            font-size: 24px;
            font-weight: bold;
            padding: 50px 100px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <button id="motivationButton">Press for Motivation!</button>

    <audio id="motivationAudio" src="you_can_do_it_australian.mp3"></audio>

    <script>
        const button = document.getElementById('motivationButton');
        const audio = document.getElementById('motivationAudio');

        button.addEventListener('click', function() {
            audio.play();
        });
    </script>
</body>
</html>
