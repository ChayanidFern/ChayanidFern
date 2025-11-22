<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Fern Portfolio</title>
    <style>
        body {
            margin: 0;
            font-family: "Poppins", sans-serif;
            background: #0e0e0e;
            color: #fff;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 60px;
        }

        header {
            text-align: center;
            margin-top: 60px;
        }

        h1 {
            font-size: 2.8rem;
            font-weight: 600;
            max-width: 800px;
            line-height: 1.5;
        }

        .emoji-heart {
            color: #ff4d6d;
        }

        /* Rabbit Snowball Animation (Fluffy style) */
        .rabbit-container {
            width: 120px;
            height: 120px;
            margin: 20px auto;
            animation: hop 2.5s infinite ease-in-out;
        }

        .rabbit {
            width: 100%;
            filter: drop-shadow(0px 0px 10px rgba(255,255,255,0.15));
        }

        @keyframes hop {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-25px); }
        }

        h2 {
            font-size: 1.8rem;
            border-bottom: 2px solid #333;
            padding-bottom: 6px;
            margin-bottom: 12px;
        }

        .content-block {
            width: 70%;
            max-width: 900px;
        }

        .tech-stack {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
        }

        .tag {
            background: #1b1b1b;
            padding: 8px 18px;
            font-size: 1rem;
            border: 1px solid #333;
            border-radius: 6px;
        }

        .connect a {
            display: inline-block;
            margin-right: 15px;
            font-size: 1.1rem;
            text-decoration: none;
            color: #6cf0ff;
        }

        footer {
            margin: 50px auto;
            font-size: 0.9rem;
            color: #888;
        }
    </style>
</head>
<body>

<header>
    <h1>Hello my name is Chayanid <br> Can you call me Fern <span class="emoji-heart">❤️</span> <br> I study Computer Science at the University of Phayao</h1>

    <div class="rabbit-container">
        <img class="rabbit" src="https://cdn-icons-png.flaticon.com/512/616/616408.png" alt="rabbit" />
    </div>
</header>

<section class="content-block">
    <h2>Tech Stack</h2>
    <div class="tech-stack">
        <span class="tag">Python</span>
        <span class="tag">Figma</span>
    </div>
</section>

<section class="content-block">
    <h2>Connect</h2>
    <div class="connect">
        <a href="mailto:example@gmail.com">Email</a>
    </div>
</section>

<footer>© 2025 Fern Portfolio — Minimal & Modern 🖤</footer>

</body>
</html>
