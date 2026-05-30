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
        }

        /* Left Side (Diagonal Split Background) */
        .left-section {
            flex: 1.1;
            background: var(--bg-left);
            position: relative;
            display: flex;
            align-items: flex-end;
            justify-content: center;
            padding-bottom: 10px;
        }

        /* Angled cut dividing the two backgrounds */
        .left-section::after {
            content: '';
            position: absolute;
            right: -50px;
            top: 0;
            width: 100px;
            height: 100%;
            background: var(--bg-left);
            transform: skewX(-12deg);
            z-index: 1;
        }

        /* Right Side Background */
        .right-section {
            flex: 1.5;
            background: var(--bg-right);
            z-index: 2;
            padding: 40px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            position: relative;
        }

        /* Character Wrapper & Animated Sleep Z */
        .character-wrapper {
            position: relative;
            z-index: 3;
            width: 85%;
            text-align: center;
        }

        .chibi-img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        .sleeping-z {
            position: absolute;
            top: -10px;
            left: 15px;
            font-size: 3.5rem;
            font-weight: 900;
            color: #fff;
            text-shadow: 3px 3px 0px #000;
            font-family: 'Poppins', sans-serif;
            animation: floatUp 2.5s infinite ease-in-out;
        }

        /* Header Row Layout */
        .header-row {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .tech-icons {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .svg-icon {
            width: 50px;
            height: 50px;
            filter: drop-shadow(2px 4px 6px rgba(0,0,0,0.15));
        }

        .main-title {
            font-size: 3.8rem;
            font-weight: 900;
            color: var(--title-color);
            letter-spacing: 2px;
            line-height: 1;
        }

        /* Terminal Styling */
        .terminal-box {
            background-color: var(--terminal-bg);
            border-radius: 18px;
            padding: 25px;
            font-family: 'Fira Code', monospace;
            font-size: 1.25rem;
            color: var(--terminal-text);
            font-weight: 600;
            box-shadow: inset 0 2px 8px rgba(0,0,0,0.05);
            line-height: 1.7;
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
                    <svg class="svg-icon" viewBox="0 0 448 512" xmlns="http://www.w3.org/2000/svg">
                        <path fill="#3776ab" d="M439.4 153.1c0-28.5-23.2-51.4-51.8-51.4H360V144c0 22.1-17.9 40-40 40h-88v40h88c44.1 0 80-35.9 80-80v-40.9h1.6c11.4 0 20.6 9.3 20.6 20.7v50.4c0 11.4-9.2 20.6-20.6 20.6h-11.4v40h11.4c28.6 0 51.8-23 51.8-51.5v-50.6zm-241 124.2c0-11 9-20 20-20s20 9 20 20-9 20-20 20-20-9-20-20z"/>
                        <path fill="#ffd343" d="M248 224H160c-44.1 0-80 35.9-80 80v40.9H78.4c-11.4 0-20.6-9.3-20.6-20.7v-50.4c0-11.4 9.2-20.6 20.6-20.6h11.4v-40H78.4C49.8 213.2 26.6 236.2 26.6 264.7v50.6c0 28.5 23.2 51.4 51.8 51.4H88V320c0-22.1 17.9-40 40-40h88v-40zm-12 114.2c0-11-9-20-20-20s-20 9-20 20 9 20 20 20 20-9 20-20z"/>
                    </svg>
                    
                    <svg class="svg-icon" viewBox="0 0 448 512" xmlns="http://www.w3.org/2000/svg">
                        <path fill="#b0c4de" d="M448 96c0 53-114.3 96-256 96S0 149 0 96s114.3-96 256-96 256 43 256 96zM256 240c141.7 0 256-43 256-96v48c0 53-114.3 96-256 96S0 245 0 192v-48c0 53 114.3 96 256 96zm0 96c141.7 0 256-43 256-96v48c0 53-114.
