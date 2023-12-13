<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>message for you</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: whitesmoke;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
        }

        .gif {
            height: 100%;
            width: 100%;
        }

        h2 {
            text-align: center;
            font-size: 1.5em;
            color: #e94d58;
            margin: 15px 0;
        }

        .btn-group {
            width: 100%;
            height: 50px;
            display: flex;
            justify-content: center;
            margin-top: 50px;
        }

        button {
            position: absolute;
            width: 150px;
            height: inherit;
            color: white;
            font-size: 1.2em;
            border-radius: 30px;
            outline: none;
            cursor: pointer;
            box-shadow: 0 2px 4px gray;
            border: 2px solid #e94d58;
            font-size: 1.2em;
        }

        button:nth-child(1) {
            margin-left: -200px;
            background: #e94d58;
        }

        button:nth-child(2) {
            margin-right: -200px;
            background: white;
            color: #e94d58;
        }
    </style>
</head>
<body>
    <div class="wrapper">
        <h2 class="question">2024 boyfriend?</h2>
        <img class="gif" alt="gif" src="https://media.giphy.com/media/FTGah7Mx3ss04PcasF/giphy.gif"/>
        <div class="btn-group">
            <button class="yes-btn">Yes</button>
            <button class="no-btn">No</button>
        </div>
    </div>
    <script>
        const question = document.querySelector(".question");
        const gif = document.querySelector(".gif");
        const yesBtn = document.querySelector(".yes-btn");
        const noBtn = document.querySelector(".no-btn");

        yesBtn.addEventListener("click", () => {
          question.innerHTML = "Yay, I love you";
          gif.src = "https://media.giphy.com/media/UMon0fuimoAN9ueUNP/giphy.gif";
        });

        noBtn.addEventListener("mouseover", () => {
          const noBtnRect = noBtn.getBoundingClientRect();
          const maxX = window.innerWidth - noBtnRect.width;
          const maxY = window.innerHeight - noBtnRect.height;

          const randomX = Math.floor(Math.random() * maxX);
          const randomY = Math.floor(Math.random() * maxY);

          noBtn.style.left = randomX + "px";
          noBtn.style.top = randomY + "px";
        });
    </script>
</body>
</html>

<!---
AnnFelicity/AnnFelicity is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
