<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NEXA GAMES - Deepak Patil</title>
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    <style>
        :root {
            --primary: #8b5cf6;
            --secondary: #ec4899;
            --bg: #020617;
            --card-bg: rgba(15, 23, 42, 0.9);
            --text: #f8fafc;
            --accent: #f59e0b;
            --p1: #ff4d4d;
            --p2: #2e86de;
            --neon-glow: 0 0 15px rgba(139, 92, 246, 0.5);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Inter', 'Segoe UI', sans-serif; user-select: none; }

        body {
            background-color: var(--bg);
            background-image: 
                radial-gradient(circle at 20% 30%, rgba(139, 92, 246, 0.15) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(236, 72, 153, 0.15) 0%, transparent 40%);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: var(--text);
            overflow: hidden; 
            padding: 20px;
        }

        /* INTRO ANIMATION STYLES */
        #intro-overlay {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: var(--bg);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            z-index: 9999;
            transition: opacity 1s ease-in-out;
        }

        .intro-text {
            font-size: 1.2rem;
            color: #94a3b8;
            letter-spacing: 4px;
            margin-bottom: 10px;
            opacity: 0;
            animation: fadeInOut 4s forwards 0.5s;
        }

        .dev-name {
            font-size: 3rem;
            font-weight: 900;
            background: linear-gradient(to right, #fff, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-transform: uppercase;
            opacity: 0;
            filter: blur(10px);
            animation: revealDev 5s forwards 1s;
        }

        .game-title-reveal {
            font-size: 4rem;
            font-weight: 900;
            color: white;
            position: absolute;
            opacity: 0;
            transform: scale(0.8);
            animation: revealGame 4s forwards 6s;
        }

        @keyframes fadeInOut {
            0% { opacity: 0; transform: translateY(10px); }
            20%, 80% { opacity: 1; transform: translateY(0); }
            100% { opacity: 0; transform: translateY(-10px); }
        }

        @keyframes revealDev {
            0% { opacity: 0; filter: blur(20px); transform: scale(0.9); }
            30% { opacity: 1; filter: blur(0px); transform: scale(1); }
            70% { opacity: 1; filter: blur(0px); transform: scale(1.05); }
            100% { opacity: 0; filter: blur(20px); transform: scale(1.1); }
        }

        @keyframes revealGame {
            0% { opacity: 0; transform: scale(0.5); filter: brightness(2); }
            50% { opacity: 1; transform: scale(1.1); filter: brightness(1); }
            100% { opacity: 0; transform: scale(1.5); filter: blur(10px); }
        }

        /* MAIN APP STYLES */
        #main-app {
            opacity: 0;
            transform: translateY(20px);
            transition: 1s ease-out;
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 100%;
        }

        #main-app.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .header { text-align: center; margin-bottom: 20px; }
        h1 { 
            font-size: 2.8rem; 
            font-weight: 900; 
            letter-spacing: 2px;
            background: linear-gradient(135deg, #fff 30%, var(--primary) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-transform: uppercase;
        }

        .game-nav {
            display: flex;
            gap: 8px;
            margin-bottom: 20px;
            background: rgba(255, 255, 255, 0.05);
            padding: 6px;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-btn {
            padding: 8px 16px;
            border-radius: 14px;
            border: none;
            background: transparent;
            color: #94a3b8;
            cursor: pointer;
            font-weight: 600;
            font-size: 0.8rem;
            transition: 0.3s;
        }

        .nav-btn.active {
            background: var(--primary);
            color: white;
            box-shadow: var(--neon-glow);
        }

        .game-area {
            background: var(--card-bg);
            padding: 20px;
            border-radius: 30px;
            backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 40px 100px rgba(0,0,0,0.6);
            position: relative;
            min-width: 360px;
            max-width: 450px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* AI Feature Styles */
        .ai-commentary {
            margin-top: 15px;
            font-size: 0.85rem;
            color: #a5b4fc;
            text-align: center;
            padding: 10px;
            background: rgba(139, 92, 246, 0.1);
            border-radius: 12px;
            border-left: 3px solid var(--primary);
            display: none;
            animation: fadeIn 0.5s ease;
        }

        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        /* Roast Game Styles */
        .roast-container {
            width: 100%;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .roast-display {
            background: rgba(0,0,0,0.5);
            padding: 15px;
            border-radius: 15px;
            min-height: 100px;
            font-style: italic;
            border: 1px dashed var(--secondary);
            color: #ff9ff3;
            font-size: 0.95rem;
            line-height: 1.4;
        }
        .roast-input {
            background: rgba(255,255,255,0.05);
            border: 1px solid rgba(255,255,255,0.2);
            color: white;
            padding: 12px;
            border-radius: 10px;
            outline: none;
            width: 100%;
            user-select: text;
        }
        .roast-btn {
            background: var(--secondary);
            color: white;
            padding: 10px;
            border-radius: 10px;
            border: none;
            font-weight: 800;
            cursor: pointer;
        }
        .roast-btn:disabled { opacity: 0.5; cursor: not-allowed; }

        .memory-timer-wrapper {
            margin-bottom: 15px;
            padding: 5px 15px;
            background: rgba(236, 72, 153, 0.1);
            border-radius: 10px;
            border: 1px solid var(--secondary);
            color: var(--secondary);
            font-weight: 800;
            display: none; 
        }

        .game-module { width: 100%; display: flex; flex-direction: column; align-items: center; }

        .candy-grid {
            display: grid;
            grid-template-columns: repeat(7, 45px);
            grid-template-rows: repeat(7, 45px);
            gap: 5px;
            padding: 10px;
            background: rgba(0,0,0,0.3);
            border-radius: 15px;
            border: 2px solid rgba(255,255,255,0.05);
        }

        .candy {
            width: 45px; height: 45px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            cursor: pointer;
            transition: 0.2s;
        }
        .candy.selected { outline: 3px solid white; box-shadow: 0 0 15px white; }

        .ttt-grid { display: grid; grid-template-columns: repeat(3, 90px); gap: 10px; }
        .cell { 
            width: 90px; height: 90px; background: rgba(255,255,255,0.03); 
            border-radius: 15px; display: flex; align-items: center; justify-content: center; 
            font-size: 2.5rem; font-weight: 900; cursor: pointer; border: 1px solid rgba(255,255,255,0.1);
        }
        .cell.x { color: var(--p1); }
        .cell.o { color: var(--p2); }
        .winner { background: var(--primary) !important; color: white !important; }

        .score-board { margin-top: 15px; display: flex; gap: 20px; font-weight: 800; }
        .turn-indicator { margin-top: 20px; font-weight: 700; font-size: 1rem; color: #94a3b8; }
        .active-user { color: var(--primary); text-transform: uppercase; }

        .footer { margin-top: 30px; }
        .dev-badge { background: rgba(255, 255, 255, 0.03); padding: 8px 20px; border-radius: 100px; color: #64748b; font-size: 0.8rem; }
        .dev-badge span { color: var(--text); font-weight: 800; }

        .hidden { display: none !important; }
        #message-box {
            position: fixed; bottom: 30px; left: 50%; transform: translate(-50%, 100px);
            background: white; color: black; padding: 10px 30px; border-radius: 15px;
            font-weight: 800; transition: 0.5s; z-index: 1000;
        }
        #message-box.show { transform: translate(-50%, 0); }
    </style>
</head>
<body>

    <div id="intro-overlay">
        <p class="intro-text">PRESENTED BY</p>
        <h2 class="dev-name">Deepak Patil</h2>
        <h1 class="game-title-reveal">NEXA GAMES</h1>
    </div>

    <div id="main-app">
        <div id="message-box">READY</div>

        <div class="header">
            <h1>NEXA GAMES</h1>
            <p id="game-title" style="color: var(--secondary); font-size: 0.8rem; font-weight: 800; text-transform: uppercase; letter-spacing: 2px;">TIC TAC TOE</p>
        </div>

        <nav class="game-nav">
            <button class="nav-btn active" onclick="switchGame('ttt')">TIC-TAC-TOE</button>
            <button class="nav-btn" onclick="switchGame('candy')">CANDY CRUSH</button>
            <button class="nav-btn" onclick="switchGame('mem')">MEMORY</button>
            <button class="nav-btn" onclick="switchGame('roast')">ROAST BATTLE</button>
        </nav>

        <div class="game-area">
            <div id="mem-timer-container" class="memory-timer-wrapper">
                TIME REMAINING: <span id="mem-timer-val">30</span>s
            </div>
            
            <div id="ttt-game" class="game-module">
                <div class="ttt-grid" id="ttt-grid">
                    <div class="cell" data-i="0"></div><div class="cell" data-i="1"></div><div class="cell" data-i="2"></div>
                    <div class="cell" data-i="3"></div><div class="cell" data-i="4"></div><div class="cell" data-i="5"></div>
                    <div class="cell" data-i="6"></div><div class="cell" data-i="7"></div><div class="cell" data-i="8"></div>
                </div>
                <!-- ✨ AI COMMENTARY BOX -->
                <div id="ttt-ai-commentary" class="ai-commentary">✨ NEXA is analyzing your "strategy"...</div>
            </div>

            <div id="candy-game" class="game-module hidden">
                <div class="candy-grid" id="candy-grid"></div>
                <div class="score-board">
                    <div style="color: var(--p1)">P1: <span id="p1-score">0</span></div>
                    <div style="color: var(--p2)">P2: <span id="p2-score">0</span></div>
                </div>
            </div>

            <div id="roast-game" class="game-module hidden">
                <div class="roast-container">
                    <div class="roast-display" id="roast-reply">"NEXA: I'm waiting. Give me your best shot, mortal."</div>
                    <input type="text" class="roast-input" id="roast-input" placeholder="Type your insult here..." onkeydown="if(event.key==='Enter') startRoastBattle()">
                    <button class="roast-btn" id="roast-submit" onclick="startRoastBattle()">✨ ROAST NEXA ✨</button>
                </div>
            </div>

            <div id="mem-game" class="game-module hidden">
                <div class="mem-grid" id="mem-grid" style="display: grid; grid-template-columns: repeat(4, 65px); gap: 10px;"></div>
            </div>

            <p class="turn-indicator">TURN: <span id="turn-info" class="active-user">USER 1</span></p>
        </div>

        <footer class="footer">
            <div class="dev-badge">Developed by <span>DEEPAK PATIL</span></div>
        </footer>
    </div>

    <script>
        const apiKey = ""; // API key injection
        window.addEventListener('load', () => {
            setTimeout(() => {
                const overlay = document.getElementById('intro-overlay');
                const mainApp = document.getElementById('main-app');
                overlay.style.opacity = '0';
                setTimeout(() => {
                    overlay.style.display = 'none';
                    mainApp.classList.add('visible');
                    document.body.style.overflow = 'auto';
                    resetCurrentGame();
                }, 1000);
            }, 10000); 
        });

        let currentGame = 'ttt';
        let currentPlayer = 1;
        let memTimerId = null;
        let memTimeLeft = 30;
        let memMatches = 0;
        
        const audioCtx = new (window.AudioContext || window.webkitAudioContext)();
        function playNote(f, t='sine', d=0.1) {
            if(audioCtx.state === 'suspended') audioCtx.resume();
            const o = audioCtx.createOscillator(); const g = audioCtx.createGain();
            o.type = t; o.frequency.value = f;
            g.gain.setValueAtTime(0.05, audioCtx.currentTime);
            g.gain.exponentialRampToValueAtTime(0.001, audioCtx.currentTime + d);
            o.connect(g); g.connect(audioCtx.destination);
            o.start(); o.stop(audioCtx.currentTime + d);
        }

        function toast(msg) {
            const b = document.getElementById('message-box');
            b.innerText = msg; b.classList.add('show');
            setTimeout(() => b.classList.remove('show'), 2000);
        }

        function switchTurn() {
            currentPlayer = currentPlayer === 1 ? 2 : 1;
            const turnEl = document.getElementById('turn-info');
            turnEl.innerText = `USER ${currentPlayer}`;
            turnEl.style.color = currentPlayer === 1 ? 'var(--p1)' : 'var(--p2)';
        }

        function switchGame(game) {
            currentGame = game;
            clearInterval(memTimerId); 
            document.getElementById('mem-timer-container').style.display = (game === 'mem') ? 'block' : 'none';
            
            document.querySelectorAll('.game-module').forEach(m => m.classList.add('hidden'));
            document.getElementById(`${game}-game`).classList.remove('hidden');
            document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
            if(event) event.target.classList.add('active');
            document.getElementById('game-title').innerText = game.toUpperCase();
            resetCurrentGame();
        }

        function resetCurrentGame() {
            currentPlayer = 1;
            const turnEl = document.getElementById('turn-info');
            turnEl.innerText = `USER 1`;
            turnEl.style.color = 'var(--p1)';

            if(currentGame === 'ttt') initTTT();
            if(currentGame === 'mem') initMem();
            if(currentGame === 'candy') initCandy();
        }

        // --- ✨ GEMINI API WRAPPER WITH RETRY LOGIC ---
        async function askGemini(prompt, systemInstruction) {
            let delay = 1000;
            for (let i = 0; i < 5; i++) {
                try {
                    const response = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({
                            contents: [{ parts: [{ text: prompt }] }],
                            systemInstruction: { parts: [{ text: systemInstruction }] }
                        })
                    });
                    if (!response.ok) throw new Error("API Limit");
                    const data = await response.json();
                    return data.candidates?.[0]?.content?.parts?.[0]?.text;
                } catch (err) {
                    await new Promise(resolve => setTimeout(resolve, delay));
                    delay *= 2;
                }
            }
            return null;
        }

        // --- ✨ AI ROAST BATTLE LOGIC ---
        async function startRoastBattle() {
            const inputEl = document.getElementById('roast-input');
            const replyEl = document.getElementById('roast-reply');
            const submitBtn = document.getElementById('roast-submit');
            const userRoast = inputEl.value.trim();

            if (!userRoast) return;

            inputEl.value = "";
            submitBtn.disabled = true;
            replyEl.innerText = "NEXA is typing a devastating comeback...";

            const systemPrompt = "You are NEXA, a sarcastic, witty AI game master. A user just roasted you. You must: 1. Roast them back even harder. 2. At the very end of your response, decide if they won the battle. If their roast was truly clever and funny, end with 'RESULT: USER WON'. If your roast was better, end with 'RESULT: NEXA WON'. Keep it short and savage.";
            
            const aiResponse = await askGemini(userRoast, systemPrompt);
            
            if (aiResponse) {
                replyEl.innerText = aiResponse.replace(/RESULT: (USER|NEXA) WON/g, "").trim();
                if (aiResponse.includes("USER WON")) {
                    toast("✨ YOU OUT-BURNED THE AI! ✨");
                    confetti();
                    playNote(800, 'square', 0.5);
                } else {
                    playNote(200, 'sawtooth', 0.5);
                }
            } else {
                replyEl.innerText = "NEXA: Your roasting skills are so bad they broke my connection. Try again.";
            }
            submitBtn.disabled = false;
        }

        // --- ✨ AI MATCH ANALYZER (TTT) ---
        async function analyzeTTT(state, winner) {
            const commentaryEl = document.getElementById('ttt-ai-commentary');
            commentaryEl.style.display = "block";
            commentaryEl.innerText = "✨ NEXA is reviewing the footage...";

            const boardStr = state.map((s, i) => s || (i + 1)).join(", ");
            const prompt = `The game ended. Board state: [${boardStr}]. Winner: ${winner || "Draw"}. Players were User 1 (X) and User 2 (O).`;
            const systemPrompt = "You are NEXA, the AI Game Master. Provide a short, sarcastic, 1-sentence analysis of the Tic-Tac-Toe game. Roast the loser or the draw. Be funny.";

            const analysis = await askGemini(prompt, systemPrompt);
            if (analysis) {
                commentaryEl.innerText = `✨ NEXA: ${analysis}`;
            } else {
                commentaryEl.style.display = "none";
            }
        }

        // --- CANDY CRUSH LOGIC ---
        const candyIcons = ['🍎', '🍇', '🍊', '🍓', '🍍', '🥥'];
        const width = 7;
        let candies = [];
        let p1Score = 0;
        let p2Score = 0;
        let selectedCandy = null;

        function initCandy() {
            const grid = document.getElementById('candy-grid');
            grid.innerHTML = "";
            candies = [];
            p1Score = 0; p2Score = 0;
            updateScores();
            for (let i = 0; i < 49; i++) {
                const candy = document.createElement('div');
                candy.className = 'candy';
                candy.setAttribute('id', i);
                candy.innerText = candyIcons[Math.floor(Math.random() * candyIcons.length)];
                candy.onclick = () => handleCandyClick(i);
                grid.appendChild(candy);
                candies.push(candy);
            }
            while(checkAndRefill(false));
        }

        function handleCandyClick(i) {
            if (!selectedCandy) {
                selectedCandy = candies[i];
                selectedCandy.classList.add('selected');
            } else {
                const id1 = parseInt(selectedCandy.id);
                const id2 = i;
                const valid = [id1-1, id1+1, id1-width, id1+width];
                if (valid.includes(id2)) {
                    const icon1 = candies[id1].innerText;
                    const icon2 = candies[id2].innerText;
                    candies[id1].innerText = icon2;
                    candies[id2].innerText = icon1;
                    if (!checkAndRefill(true)) {
                        setTimeout(() => {
                            candies[id1].innerText = icon1;
                            candies[id2].innerText = icon2;
                        }, 300);
                    } else {
                        playNote(600);
                        switchTurn();
                    }
                }
                selectedCandy.classList.remove('selected');
                selectedCandy = null;
            }
        }

        function checkAndRefill(doScore) {
            let matched = false;
            for (let i = 0; i < 49; i++) {
                let r3 = [i, i+1, i+2];
                if (i%width < width-2 && r3.every(idx => candies[idx].innerText === candies[i].innerText && candies[i].innerText !== "")) {
                    if (doScore) addScore(3);
                    r3.forEach(idx => candies[idx].innerText = "");
                    matched = true;
                }
                let c3 = [i, i+width, i+width*2];
                if (i < 35 && c3.every(idx => candies[idx].innerText === candies[i].innerText && candies[i].innerText !== "")) {
                    if (doScore) addScore(3);
                    c3.forEach(idx => candies[idx].innerText = "");
                    matched = true;
                }
            }
            if (matched) {
                for (let i = 0; i < 42; i++) {
                    if (candies[i+width].innerText === "") {
                        candies[i+width].innerText = candies[i].innerText;
                        candies[i].innerText = "";
                    }
                }
                for (let i = 0; i < width; i++) {
                    if (candies[i].innerText === "") candies[i].innerText = candyIcons[Math.floor(Math.random()*candyIcons.length)];
                }
                setTimeout(() => checkAndRefill(doScore), 300);
                return true;
            }
            return false;
        }

        function addScore(n) {
            if (currentPlayer === 1) p1Score += n; else p2Score += n;
            updateScores();
            if(n>=3) { playNote(800); if(n>3) confetti(); }
        }

        function updateScores() {
            document.getElementById('p1-score').innerText = p1Score;
            document.getElementById('p2-score').innerText = p2Score;
        }

        // --- TTT LOGIC ---
        let tttState = Array(9).fill("");
        function initTTT() {
            tttState = Array(9).fill("");
            document.getElementById('ttt-ai-commentary').style.display = "none";
            document.querySelectorAll('#ttt-grid .cell').forEach(c => { 
                c.innerText = ""; c.classList.remove('winner','x','o'); 
            });
        }
        document.getElementById('ttt-grid').addEventListener('click', e => {
            const i = e.target.dataset.i;
            if(i === undefined || tttState[i]) return;
            const mark = currentPlayer === 1 ? 'X' : 'O';
            tttState[i] = mark;
            e.target.innerText = mark;
            e.target.classList.add(mark.toLowerCase());
            playNote(currentPlayer === 1 ? 400 : 500);
            const wins = [[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]];
            let winnerFound = null;
            let won = wins.some(c => {
                if(tttState[c[0]] && tttState[c[0]] === tttState[c[1]] && tttState[c[0]] === tttState[c[2]]) {
                    c.forEach(idx => document.querySelectorAll('#ttt-grid .cell')[idx].classList.add('winner'));
                    winnerFound = tttState[c[0]] === 'X' ? 'User 1' : 'User 2';
                    return true;
                }
            });

            if(won) { 
                toast(`${winnerFound.toUpperCase()} WINS!`); 
                confetti(); 
                analyzeTTT([...tttState], winnerFound);
            }
            else if(!tttState.includes("")) {
                toast("DRAW!");
                analyzeTTT([...tttState], null);
            }
            else switchTurn();
        });

        // --- MEMORY MATCH LOGIC ---
        let flipped = [];
        function initMem() {
            clearInterval(memTimerId);
            memTimeLeft = 30;
            memMatches = 0;
            document.getElementById('mem-timer-val').innerText = memTimeLeft;
            
            memTimerId = setInterval(() => {
                memTimeLeft--;
                document.getElementById('mem-timer-val').innerText = memTimeLeft;
                if(memTimeLeft <= 0) {
                    clearInterval(memTimerId);
                    toast("TIME OUT! TRY AGAIN");
                    initMem();
                }
            }, 1000);

            const icons = ['💎','💎','🚀','🚀','👻','👻','🔥','🔥','🍕','🍕','⚡','⚡','🌈','🌈','🍭','🍭'];
            const shuffled = icons.sort(() => Math.random() - 0.5);
            const grid = document.getElementById('mem-grid');
            grid.innerHTML = "";
            shuffled.forEach(icon => {
                const card = document.createElement('div');
                card.className = 'cell'; card.style.fontSize = '1.5rem';
                card.onclick = () => {
                    if(card.innerText || flipped.length === 2) return;
                    card.innerText = icon; flipped.push(card);
                    if(flipped.length === 2) {
                        if(flipped[0].innerText === flipped[1].innerText) { 
                            flipped = []; 
                            memMatches++;
                            playNote(800); 
                            if(memMatches === 8) {
                                clearInterval(memTimerId);
                                toast("ALL MATCHED! YOU WIN!");
                                confetti();
                            }
                        }
                        else { 
                            setTimeout(() => { 
                                flipped.forEach(c => c.innerText = ""); 
                                flipped = []; 
                                switchTurn(); 
                            }, 600); 
                        }
                    }
                };
                grid.appendChild(card);
            });
        }
    </script>
</body>
</html>