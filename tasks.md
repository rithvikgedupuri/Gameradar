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

## 🏆 Mission 3: Write Your Top 5 Gaming Countdown
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

## 📊 Mission 4: Settle the Debate (Create a Live Voting Poll)
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
