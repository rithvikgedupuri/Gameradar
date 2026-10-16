# 🎮 Project: Build Your Own GamesRadar Website!

Follow this step-by-step mission checklist to build your very own gaming portal from absolute scratch, hook up a real website name, and add interactive features!

---

## 🛠️ Mission 1: Build the Launchpad (Create Your GitHub Repository)
*First, we need a place on the internet to store your website files.*

- [ ] **Log in to GitHub:** Open your browser and go to your GitHub account.
- [ ] **Create a New Repository:** Click the **`+`** icon in the upper-right corner and select **New repository**.
- [ ] **Name Your Project:** Choose a cool name for your gaming hub (e.g., `rithvikgedupuri.github.io`).
- [ ] **Set Visibility to Public:** Ensure **Public** is selected so your friends can see your site.
- [ ] **Add a Initialize File:** Check the box that says **Add a README file**.
- [ ] **Launch:** Click the green **Create repository** button at the bottom.
- [ ] **Create the Main Page:** Inside your new repository, click **Add file** ➔ **Create new file**. Name the file exactly `index.html`. Write `<h1>Hello World</h1>` inside it and click **Commit changes**.

---

## 🌐 Mission 2: Get Your Custom Web Name (Link Your GoDaddy Domain)
*Let's make your website look official by pointing your GoDaddy domain name directly to your GitHub files.*

### Part A: Setup on GoDaddy
- [ ] **Open GoDaddy DNS:** Log in to your GoDaddy Domain Portfolio, find your domain, and click **DNS** to open the management page.
- [ ] **Clean Up Old Records:** If you see an existing row that says `A` • `@` • `Parked`, delete it by clicking the trash can icon.
- [ ] **Add GitHub's IP Addresses:** Click **Add New Record** 4 separate times to add these four **A Records**:
  * **Type:** `A` | **Name:** `@` | **Value:** `185.199.108.153`
  * **Type:** `A` | **Name:** `@` | **Value:** `185.199.109.153`
  * **Type:** `A` | **Name:** `@` | **Value:** `185.199.110.153`
  * **Type:** `A` | **Name:** `@` | **Value:** `185.199.111.153`
- [ ] **Point the Subdomain:** Find the row for the `CNAME` record where the Name is `www`. Click **Edit** and change its value to `yourusername.github.io` (replace with your actual GitHub username). Click **Save**.

### Part B: Setup on GitHub
- [ ] **Open Settings:** Go to your repository on GitHub and click the **Settings** tab at the top.
- [ ] **Navigate to Pages:** Click **Pages** in the left sidebar menu.
- [ ] **Enter Your Domain:** Scroll down to the **Custom domain** box, type your GoDaddy domain (e.g., `yourdomain.com`), and click **Save**.
- [ ] **Secure Your Site:** Once the green "DNS check successful" message appears, check the box for **Enforce HTTPS**.

---
# Mission 3: Configure Custom Domains to Root Domain

To point your new subdomain (`gamerador.rameshgedupuri.space`) to your GitHub Pages site, you need to configure settings in both your **GoDaddy DNS panel** and your **GitHub repository**. 

## Step 1: Add a CNAME Record in GoDaddy
1. Click the black **Add New Record** button located right above your DNS records table.
2. Fill out the fields with the following details:
   * **Type:** `CNAME`
   * **Name:** `gamerador`
   * **Value (or Data):** `rithvikgedupuri.github.io.` *(Note: Match this to the target username displayed in your existing `www` record)*
   * **TTL:** `1 Hour` (or default)
3. Save the record.

## Step 2: Configure Your GitHub Repository
1. Go to the GitHub repository containing the project you want this subdomain to display.
2. Click on **Settings** (the gear icon at the top of the repository).
3. Scroll down to the **Pages** section in the left sidebar.
4. Under **Custom domain**, type your complete subdomain: `gamerador.rameshgedupuri.space`.
5. Click **Save**.

## Step 3: Enforce HTTPS
* Once GitHub successfully verifies your domain ownership (this usually takes a few minutes to an hour), check the box for **Enforce HTTPS** in that same GitHub Pages settings menu.

---
## 🏆 Mission 4: Write Your Top 5 Gaming Countdown
*Time to add content just like a real game journalist on GamesRadar!*

- [ ] **Edit index.html:** Open your `index.html` file on GitHub and click the **Pencil icon ✏️** to edit it.
- [ ] **Paste the Countdown Template:** Scroll to the bottom of your file and paste this block:

```html
<!-- Start of Top 5 Game List -->
<hr style="margin: 30px 0; border: 1px solid #ccc;">

<h2 style="font-family: sans-serif; color: #333;">🏆 My Top 5 Games of the Year</h2>
<p style="font-family: sans-serif; color: #555;">Here are my absolute favorite games right now and exactly why you should play them:</p>

<ol style="font-family: sans-serif; font-size: 16px; line-height: 1.8; color: #222;">
  <li>🚀 <strong>[Game Name 1]</strong> - Type why this game is awesome here!</li>
  <li>🧱 <strong>[Game Name 2]</strong> - What is your favorite thing to do in this game?</li>
  <li>👑 <strong>[Game Name 3]</strong> - Why is this game in the top 3?</li>
  <li>🏎️ <strong>[Game Name 4]</strong> - Add a cool detail or mode you like.</li>
  <li>👾 <strong>[Game Name 5]</strong> - Write a quick tip for anyone playing this game.</li>
</ol>
<!-- End of Top 5 Game List -->
```
- [ ] **Make It Yours:** Change the placeholder `[Game Name]` text and descriptions to feature your favorite video games.
- [ ] **Save:** Click the green **Commit changes** button.

---

## 📊 Mission 5: Settle the Debate (Create a Live Voting Poll)
*Get your audience involved by letting them vote on their favorite platforms or games.*

- [ ] **Design Your Poll:** Go to StrawPoll.com. Type a fun gaming question (e.g., *Xbox vs. PlayStation vs. Nintendo*) and add your options. Click **Create Poll**.
- [ ] **Grab the Link:** Under the **Share** section at the bottom, click the copy icon next to your unique poll link.
- [ ] **Edit index.html Again:** Open your `index.html` file on GitHub and hit the **Pencil icon ✏️**.
- [ ] **Paste the Interactive Button Template:** Scroll to the absolute bottom of your file and paste this code:

```html
<!-- Start of Voting Poll Section -->
<hr style="margin: 30px 0; border: 1px solid #ccc;">

<div style="font-family: sans-serif; text-align: center; background-color: #f9f9f9; padding: 20px; border-radius: 8px; border: 1px solid #ddd;">
  <h2 style="color: #333; margin-top: 0;">📊 Cast Your Vote!</h2>
  <p style="color: #555;">Help me settle the debate! Vote for your favorite game on my official poll:</p>
  
  <!-- PASTE YOUR COPIED LINK INSIDE THE href="" QUOTES BELOW -->
  <a href="PASTE_YOUR_STRAWPOLL_LINK_HERE" target="_blank" style="display: inline-block; background-color: #4F46E5; color: white; padding: 12px 24px; text-decoration: none; font-weight: bold; border-radius: 6px; margin-top: 10px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">👉 Click Here to Vote Now! 👈</a>
</div>
<!-- End of Voting Poll Section -->
```
- [ ] **Link It Up:** Replace `PASTE_YOUR_STRAWPOLL_LINK_HERE` with the actual link you copied from StrawPoll. Keep the quotes around it!
- [ ] **Publish Live:** Click **Commit changes**. Open your site, click your shiny new button, and see if it works!


# 🚀 Mission 6: Build a 4-Game Learning Arcade

Welcome to your next developer milestone! In this mission, you will back up your current layout, create two brand-new educational games, and deploy a responsive 4-game dashboard.

---

### 💾 Part A: Save a Backup of Your Existing Homepage
Before changing any code, it is best practice to save a backup of your working setup.

1. **Open your repository:** Go to GitHub and open your gaming hub repository.
2. **Open the file:** Click on `index.html`.
3. **Copy everything:** Click inside the code window, press `Ctrl + A` (or `Cmd + A` on Mac) to highlight everything, and copy it (`Ctrl + C` / `Cmd + C`).
4. **Save it locally:** Open a text editor on your computer (like Notepad or TextEdit), paste the code inside, and save the file on your machine as `index_backup.txt`.

---

### 🧮 Part B: Create the "Math Attack" Game (`math.html`)
This game helps practice rapid addition. Kids can later edit the code to try multiplication or use larger numbers!

1. Go back to your main repository page on GitHub.
2. Click **Add file** ➔ **Create new file**.
3. Name the file exactly: `math.html`
4. Paste the following code into the editor:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Math Attack</title>
    <style>
        body { background-color: #121214; color: #ffffff; font-family: 'Segoe UI', sans-serif; text-align: center; padding: 50px 20px; }
        .game-box { background-color: #1e1e24; border: 2px solid #03dac6; border-radius: 12px; padding: 40px; max-width: 400px; margin: 0 auto; box-shadow: 0 4px 15px rgba(0,0,0,0.5); }
        .question { font-size: 2.5rem; margin: 20px 0; font-weight: bold; color: #6200ee; background: #fff; padding: 10px; border-radius: 8px; }
        input { font-size: 1.5rem; padding: 10px; width: 60%; text-align: center; border-radius: 6px; border: none; margin-bottom: 20px; color: #000; }
        .btn { background-color: #03dac6; color: #121214; border: none; padding: 12px 25px; font-size: 1.1rem; font-weight: bold; border-radius: 6px; cursor: pointer; }
        .back-link { display: inline-block; margin-top: 25px; color: #03dac6; text-decoration: none; }
    </style>
</head>
<body>

    <div class="game-box">
        <h2>🧮 Math Attack!</h2>
        <p>Solve the problem as fast as you can to score XP!</p>
        
        <div class="question" id="problem">? + ?</div>
        <input type="number" id="answerInput" placeholder="Type answer..." autofocus>
        <br>
        <button class="btn" id="submitBtn">SUBMIT</button>
        
        <h3 style="color: #ff4757;">Score: <span id="score">0</span> XP</h3>
        
        <a href="index.html" class="back-link">⬅️ Back to Hub</a>
    </div>

    <script>
        let score = 0;
        let num1, num2, correctAnswer;

        const problemDisplay = document.getElementById('problem');
        const input = document.getElementById('answerInput');
        const submitBtn = document.getElementById('submitBtn');
        const scoreDisplay = document.getElementById('score');

        function generateQuestion() {
            // CODE CHALLENGE: Change the 10 to 50 or 100 to make the numbers bigger!
            num1 = Math.floor(Math.random() * 10) + 1;
            num2 = Math.floor(Math.random() * 10) + 1;
            
            // CODE CHALLENGE: Change "+" to "*" to turn this into a multiplication game!
            correctAnswer = num1 + num2; 
            problemDisplay.innerText = `${num1} + ${num2}`;
            input.value = '';
            input.focus();
        }

        function checkAnswer() {
            if (parseInt(input.value) === correctAnswer) {
                score += 10;
                scoreDisplay.innerText = score;
                alert("🎉 Correct! +10 XP");
                generateQuestion();
            } else {
                alert("❌ Oops! Try that one again.");
            }
        }

        submitBtn.addEventListener('click', checkAnswer);
        input.addEventListener('keypress', (e) => { if (e.key === 'Enter') checkAnswer(); });

        generateQuestion();
    </script>
</body>
</html>
```
5. Scroll down and click the green **Commit changes...** button.

---

### 🔮 Part C: Create the "Number Wizard" Game (`guess.html`)
This game teaches logical estimation (guessing higher or lower) to find a hidden number between 1 and 50.

1. Go back to your main repository page on GitHub.
2. Click **Add file** ➔ **Create new file**.
3. Name the file exactly: `guess.html`
4. Paste the following code into the editor:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Number Wizard</title>
    <style>
        body { background-color: #121214; color: #ffffff; font-family: 'Segoe UI', sans-serif; text-align: center; padding: 50px 20px; }
        .game-box { background-color: #1e1e24; border: 2px solid #03dac6; border-radius: 12px; padding: 40px; max-width: 400px; margin: 0 auto; }
        input { font-size: 1.5rem; padding: 10px; width: 50%; text-align: center; border-radius: 6px; border: none; margin: 20px 0; color: #000; }
        .btn { background-color: #6200ee; color: white; border: none; padding: 12px 25px; font-size: 1.1rem; border-radius: 6px; cursor: pointer; }
        .back-link { display: inline-block; margin-top: 25px; color: #03dac6; text-decoration: none; }
    </style>
</head>
<body>

    <div class="game-box">
        <h2>🔮 Number Wizard</h2>
        <p>I am thinking of a number between <strong>1 and 50</strong>. Can you find it?</p>
        
        <input type="number" id="guessInput" placeholder="??">
        <br>
        <button class="btn" id="guessBtn">GUESS</button>
        
        <h3 id="hint" style="color: #ffa502; margin-top: 20px;">Take a guess!</h3>
        <p>Attempts: <span id="attempts">0</span></p>
        
        <a href="index.html" class="back-link">⬅️ Back to Hub</a>
    </div>

    <script>
        // CODE CHALLENGE: Change 50 to 100 to expand the guessing universe range!
        const secretNumber = Math.floor(Math.random() * 50) + 1;
        let attempts = 0;

        const input = document.getElementById('guessInput');
        const button = document.getElementById('guessBtn');
        const hint = document.getElementById('hint');
        const attemptsDisplay = document.getElementById('attempts');

        button.addEventListener('click', () => {
            const userGuess = parseInt(input.value);
            attempts++;
            attemptsDisplay.innerText = attempts;

            if (userGuess === secretNumber) {
                hint.style.color = "#2ed573";
                hint.innerText = `🎉 YOU WIN! The number was ${secretNumber}! It took ${attempts} tries.`;
            } else if (userGuess < secretNumber) {
                hint.innerText = "📈 HIGHER! Try a bigger number.";
            } else if (userGuess > secretNumber) {
                hint.innerText = "📉 LOWER! Try a smaller number.";
            }
            input.value = '';
        });
    </script>
</body>
</html>
```
5. Scroll down and click the green **Commit changes...** button.

---

### Part D: 
1. Add the `clicker.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clicker Mania</title>
    <style>
        body {
            background-color: #121214;
            color: #ffffff;
            font-family: sans-serif;
            text-align: center;
            padding: 50px 20px;
        }
        .game-box {
            background-color: #1e1e24;
            border: 2px solid #03dac6;
            border-radius: 12px;
            padding: 40px;
            max-width: 400px;
            margin: 0 auto;
        }
        .btn {
            background-color: #6200ee;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2rem;
            border-radius: 8px;
            cursor: pointer;
        }
        .back-link {
            display: inline-block;
            margin-top: 20px;
            color: #03dac6;
            text-decoration: none;
        }
    </style>
</head>
<body>

    <div class="game-box">
        <h2>👾 Clicker Mania</h2>
        <div style="font-size: 2rem; color: #ff4757; margin: 20px 0;">Score: <span id="score">0</span></div>
        <button class="btn" id="clickBtn">💥 CLICK!</button>
        <br>
        <a href="index.html" class="back-link">⬅️ Back to Hub</a>
    </div>

    <script>
        let score = 0;
        document.getElementById('clickBtn').addEventListener('click', () => {
            score++;
            document.getElementById('score').innerText = score;
        });
    </script>

</body>
</html>

```

### Part E: Add `reaction.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reflex Reflex</title>
    <style>
        body {
            background-color: #121214;
            color: #ffffff;
            font-family: 'Segoe UI', sans-serif;
            text-align: center;
            padding: 50px 20px;
        }
        .game-box {
            background-color: #1e1e24;
            border: 2px solid #03dac6;
            border-radius: 12px;
            padding: 40px;
            max-width: 500px;
            margin: 0 auto;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }
        #target {
            width: 200px;
            height: 200px;
            background-color: #ff4757;
            border-radius: 50%;
            margin: 30px auto;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: bold;
            user-select: none;
            transition: background 0.1s;
        }
        .back-link {
            display: inline-block;
            margin-top: 25px;
            color: #03dac6;
            text-decoration: none;
            font-weight: bold;
        }
        .back-link:hover { text-decoration: underline; }
    </style>
</head>
<body>

    <div class="game-box">
        <h2>⚡ Reflex Tester</h2>
        <p>Wait for the red circle to turn <strong>GREEN</strong>, then click it as fast as you can!</p>
        
        <div id="target">CLICK TO START</div>
        
        <h3 id="result">Best Time: -- ms</h3>
        
        <a href="index.html" class="back-link">⬅️ Back to Hub</a>
    </div>

    <script>
        const target = document.getElementById('target');
        const result = document.getElementById('result');
        
        let startTime, endTime;
        let timerTimeout;
        let gameState = 'idle'; // idle, waiting, green

        target.addEventListener('click', () => {
            if (gameState === 'idle') {
                // Start the test sequence
                target.style.backgroundColor = '#ff4757';
                target.innerText = 'WAIT FOR IT...';
                result.innerText = 'Get ready...';
                gameState = 'waiting';
                
                // Random delay between 1.5 and 4 seconds
                const delay = Math.random() * 2500 + 1500;
                
                timerTimeout = setTimeout(() => {
                    target.style.backgroundColor = '#2ed573';
                    target.innerText = 'CLICK!!!';
                    startTime = Date.now();
                    gameState = 'green';
                }, delay);
                
            } else if (gameState === 'waiting') {
                // Cheated! Clicked too early
                clearTimeout(timerTimeout);
                target.style.backgroundColor = '#ffa502';
                target.innerText = 'TOO EARLY!';
                result.innerText = 'Trigger happy! Try again.';
                gameState = 'idle';
                
            } else if (gameState === 'green') {
                // Successful hit
                endTime = Date.now();
                const reactionTime = endTime - startTime;
                target.style.backgroundColor = '#6200ee';
                target.innerText = 'RESET';
                result.innerText = `Your Time: ${reactionTime} ms!`;
                gameState = 'idle';
            }
        });
    </script>

</body>
</html>

```

### 🌐 Part D: Deploy the New 4-Box Arcade Hub (`index.html`)
Now update your primary entry page to display all four games side-by-side in a clean, responsive layout.

1. Open your **`index.html`** file on GitHub.
2. Click the **Pencil icon ✏️** to edit it.
3. Completely delete everything currently inside the file.
4. Paste this full master portal layout code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arcade Portal</title>
    <style>
        body {
            background-color: #121214;
            color: #ffffff;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
        }
        header {
            padding: 40px 20px;
            background: linear-gradient(135deg, #6200ee, #03dac6);
            border-radius: 12px;
            margin-bottom: 30px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }
        h1 { margin: 0; font-size: 2.5rem; text-transform: uppercase; letter-spacing: 2px; }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        .card {
            background-color: #1e1e24;
            border: 2px solid #333;
            border-radius: 12px;
            padding: 25px;
            transition: transform 0.2s, border-color 0.2s;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .card:hover {
            transform: translateY(-5px);
            border-color: #03dac6;
        }
        .card h3 { margin-top: 0; color: #03dac6; }
        .btn {
            display: inline-block;
            background-color: #6200ee;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 6px;
            font-weight: bold;
            margin-top: 15px;
        }
        .btn:hover { background-color: #3700b3; }
    </style>
</head>
<body>

    <header>
        <h1>🎮 Kid's Coding Arcade </h1>
        <p>Play the games, then open up GitHub to change how they work!</p>
    </header>

    <div class="grid">
        <!-- Game 1 -->
        <div class="card">
            <h3>Clicker Mania</h3>
            <p>Score points by clicking as fast as you can before time runs out!</p>
            <a href="clicker.html" class="btn">Play Now</a>
        </div>

        <!-- Game 2 -->
        <div class="card">
            <h3>⚡ Reflex Tester</h3>
            <p>Test your speed! Click the target the exact millisecond it flashes green.</p>
            <a href="reaction.html" class="btn" style="background-color: #03dac6; color: #121214;">Play Now</a>
        </div>

        <!-- Game 3 -->
        <div class="card">
            <h3>🧮 Math Attack!</h3>
            <p>A high-speed math quest. Rapid addition helper to gain points!</p>
            <a href="math.html" class="btn" style="background-color: #ff4757;">Play Now</a>
        </div>

        <!-- Game 4 -->
        <div class="card">
            <h3>🔮 Number Wizard</h3>
            <p>Use elimination logic to hunt down the system's hidden secret number.</p>
            <a href="guess.html" class="btn" style="background-color: #ffa502; color: #121214;">Play Now</a>
        </div>
    </div>

</body>
</html>

```


