# swetha-love
<!DOCTYPE html>
<html>
<head>
    <title>Swetha ❤️ Visnu</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            text-align: center;
            color: white;
        }

        h1 {
            margin-top: 40px;
            font-size: 40px;
        }

        p {
            width: 70%;
            margin: auto;
            font-size: 20px;
        }

        .heart {
            font-size: 50px;
            animation: beat 1s infinite;
        }

        @keyframes beat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        #timer {
            font-size: 22px;
            margin-top: 20px;
        }

        .btn {
            padding: 12px 25px;
            font-size: 18px;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            margin: 10px;
        }

        #yesBtn {
            background-color: #ff3366;
            color: white;
        }

        #noBtn {
            background-color: white;
            color: #ff3366;
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Swetha ❤️ Visnu</h1>
    <div class="heart">❤️</div>

    <p>
        From 6th standard... 💫 <br><br>
        Once we met in the auto and came towards a universe 
        which cannot be broken by any universe 🫂🙈💋🧿 <br><br>
        My Panda 🐼, I love you for your character, your dusky beauty,
        and your innocent heart ❤️
    </p>

    <div id="timer"></div>

    <h2>Will You Be My Valentine? 💍</h2>

    <button class="btn" id="yesBtn" onclick="yesClick()">YES ❤️</button>
    <button class="btn" id="noBtn" onmouseover="moveNo()">NO 😜</button>

    <script>
        // Love Timer
        var startDate = new Date("June 1, 2014 00:00:00").getTime();

        setInterval(function() {
            var now = new Date().getTime();
            var distance = now - startDate;

            var days = Math.floor(distance / (1000 * 60 * 60 * 24));
            var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            var seconds = Math.floor((distance % (1000 * 60)) / 1000);

            document.getElementById("timer").innerHTML =
                "We have been together for 💕<br>" +
                days + " Days " + hours + " Hours " +
                minutes + " Minutes " + seconds + " Seconds ❤️";
        }, 1000);

        function yesClick() {
            alert("I Love You Forever My Panda 🐼❤️ - Visnu");
        }

        function moveNo() {
            var button = document.getElementById("noBtn");
            var x = Math.random() * window.innerWidth;
            var y = Math.random() * window.innerHeight;
            button.style.left = x + "px";
            button.style.top = y + "px";
        }
    </script>

</body>
</html>