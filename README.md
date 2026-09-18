# gamezone
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GameZone</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0b0b12;
            color: white;
        }

        header {
            background: #11111c;
            padding: 20px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #292938;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
        }

        .logo span {
            color: #6c63ff;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 25px;
        }

        .hero {
            padding: 80px 8%;
            text-align: center;
            background: linear-gradient(135deg, #11111c, #17172a);
        }

        .hero h1 {
            font-size: 55px;
            margin-bottom: 15px;
        }

        .hero h1 span {
            color: #6c63ff;
        }

        .hero p {
            color: #aaa;
            font-size: 18px;
            margin-bottom: 30px;
        }

        .button {
            display: inline-block;
            background: #6c63ff;
            color: white;
            padding: 14px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
        }

        .section {
            padding: 50px 8%;
        }

        .section h2 {
            margin-bottom: 25px;
            font-size: 30px;
        }

        .games {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
        }

        .game {
            background: #151521;
            border: 1px solid #292938;
            padding: 30px 20px;
            border-radius: 12px;
            text-align: center;
            transition: 0.2s;
        }

        .game:hover {
            transform: translateY(-5px);
            border-color: #6c63ff;
        }

        .game-icon {
            font-size: 45px;
            margin-bottom: 15px;
        }

        .game h3 {
            margin-bottom: 8px;
        }

        .game p {
            color: #999;
            font-size: 14px;
        }

        .ad {
            margin-top: 40px;
            min-height: 100px;
            border: 1px dashed #444;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #666;
        }

        footer {
            text-align: center;
            padding: 30px;
            color: #777;
            border-top: 1px solid #292938;
        }
    </style>
</head>

<body>

<header>
    <div class="logo">Game<span>Zone</span></div>

    <nav>
        <a href="#">Home</a>
        <a href="#games">Games</a>
        <a href="#quiz">Quiz</a>
    </nav>
</header>

<section class="hero">
    <h1>Welcome to <span>GameZone</span></h1>

    <p>
        Gaming news, guides, quizzes and everything gamers need.
    </p>

    <a href="#games" class="button">Explore Games</a>
</section>

<section class="section" id="games">

    <h2>🔥 Popular Games</h2>

    <div class="games">

        <div class="game">
            <div class="game-icon">🔫</div>
            <h3>Rainbow Six Siege</h3>
            <p>Operators, tips and settings</p>
        </div>

        <div class="game">
            <div class="game-icon">🏗️</div>
            <h3>Fortnite</h3>
            <p>Updates, tips and challenges</p>
        </div>

        <div class="game">
            <div class="game-icon">⛏️</div>
            <h3>Minecraft</h3>
            <p>Seeds, builds and guides</p>
        </div>

        <div class="game">
            <div class="game-icon">🧱</div>
            <h3>Roblox</h3>
            <p>Games, codes and quizzes</p>
        </div>

        <div class="game">
            <div class="game-icon">⚽</div>
            <h3>EA FC</h3>
            <p>Squads, career and tips</p>
        </div>

        <div class="game">
            <div class="game-icon">🎯</div>
            <h3>Call of Duty</h3>
            <p>Loadouts, weapons and guides</p>
        </div>

    </div>

    <div class="ad">
        ADVERTISEMENT
    </div>

</section>

<section class="section" id="quiz">

    <h2>🧠 Daily Gaming Quiz</h2>

    <div class="game">
        <h3>Which game is known for its block-based world?</h3>

        <br>

        <button class="button" onclick="answer('Minecraft')">
            Minecraft
        </button>

        <button class="button" onclick="answer('Fortnite')">
            Fortnite
        </button>

        <p id="answer" style="margin-top:20px;"></p>
    </div>

</section>

<footer>
    © 2026 GameZone — Built for gamers.
</footer>

<script>
    function answer(choice) {

        const result = document.getElementById("answer");

        if (choice === "Minecraft") {
            result.innerHTML = "✅ Correct!";
        } else {
            result.innerHTML = "❌ Try again!";
        }
    }
</script>

</body>
</html>
