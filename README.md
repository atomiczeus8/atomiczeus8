<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zandacross GitHub Banner</title>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@500;600;700&family=Poppins:wght@800;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-left: #a5c7f7;
            --bg-right: #2d5b8c;
            --terminal-bg: #cde4ff;
            --terminal-text: #1e3d59;
            --title-color: #1a2f4c;
        }

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
            background-color: #f0f4f8;
            font-family: 'Poppins', sans-serif;
        }

        /* Banner Container Frame */
        .banner-container {
            width: 1000px;
            height: 380px;
            border-radius: 20px;
            overflow: hidden;
            display: flex;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
            border: 5px solid #bce0fd;
            position: relative;
            /* Using a clean linear-gradient split to ensure it NEVER breaks */
            background: linear-gradient(105deg, var(--bg-left) 0%, var(--bg-left) 42%, var(--bg-right) 42.1%, var(--bg-right) 100%);
        }

        /* Left Side Content Area */
        .left-section {
            flex: 1;
            height: 100%;
            display: flex;
            align-items: flex-end;
            justify-content: center;
            padding-bottom: 20px;
            padding-left: 20px;
            z-index: 2;
        }

        /* Right Side Content Area */
        .right-section {
            flex: 1.4;
            height: 100%;
            padding: 40px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            z-index: 2;
        }

        /* Character Wrapper & Animated Sleep Z */
        .character-wrapper {
            position: relative;
            width: 90%;
            max-width: 320px;
            text-align: center;
        }

        .chibi-img {
            width: 100%;
            height: auto;
            display: block;
        }

        .sleeping-z {
            position: absolute;
            top: -10px;
            left: 25px;
            font-size: 3.5rem;
            font-weight: 900;
            color: #fff;
            text-shadow: 3px 3px 0px #000;
            animation: floatUp 2.5s infinite ease-in-out;
        }

        /* Header Row Layout */
        .header-row {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 100%;
        }

        .tech-icons {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .svg-icon {
            width: 48px;
            height: 48px;
            filter: drop-shadow(2px 4px 6px rgba(0,0,0,0.15));
        }

        .main-title {
            font-size: 3.5rem;
            font-weight: 900;
            color: #ffffff; /* Shifted to white to contrast perfectly with the dark blue side */
            letter-spacing: 2px;
            line-height: 1;
        }

        /* Terminal Styling */
        .terminal-box {
            background-color: var(--terminal-bg);
            border-radius: 18px;
            padding: 22px;
            font-family: 'Fira Code', monospace;
            font-size: 1.2rem;
            color: var(--terminal-text);
            font-weight: 600;
            box-shadow: inset 0 2px 8px rgba(0,0,0,0.05);
            line-height: 1.6;
            width: 100%;
        }

        .comment {
            color: #53708e;
        }

        .blue-text {
            color: #0b5394;
        }

        /* Footer Link */
        .banner-footer {
            text-align: right;
            font-family: 'Fira Code', monospace;
            color: #a5c7f7;
            font-size: 1rem;
            opacity: 0.8;
            width: 100%;
        }

        /* Core Animations */
        .cursor {
            animation: blink 1s infinite steps(2, start);
        }

        @keyframes blink {
            to { visibility: hidden; }
        }

        @keyframes floatUp {
            0% { transform: translate(0, 0) scale(0.7); opacity: 0; }
            40% { opacity: 1; }
            100% { transform: translate(-25px, -50px) scale(1.3); opacity: 0; }
        }
    </style>
</head>
<body>

    <div class="banner-container">
        <div class="left-section">
            <div class="character-wrapper">
                <img src="aemeath-ames.gif" alt="Sleeping Chibi" class="chibi-img">
                <div class="sleeping-z">Z</div>
            </div>
        </div>

        <div class="right-section">
            
            <div class="header-row">
                <div class="tech-icons">
                    <svg class="svg-icon" viewBox="0 0 448 512" xmlns="
                    
