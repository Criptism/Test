<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>RNG GUI - Enhanced</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;900&display=swap');
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html, body {
      height: 100%;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
      background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #16213e 100%);
      color: #fff;
      overflow-x: hidden;
    }

    .particles {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 0;
      opacity: 0.15;
    }

    .particle {
      position: absolute;
      border-radius: 50%;
      animation: float 20s infinite ease-in-out;
    }

    @keyframes float {
      0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.3; }
      25% { transform: translate(100px, -50px) scale(1.1); opacity: 0.6; }
      50% { transform: translate(-50px, 100px) scale(0.9); opacity: 0.4; }
      75% { transform: translate(150px, 50px) scale(1.05); opacity: 0.5; }
    }

    .layout {
      position: relative;
      z-index: 1;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: center;
      min-height: 100vh;
      gap: 40px;
      padding: 60px 40px;
    }

    .container {
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
      flex: none;
    }

    .title {
      font-size: 42px;
      font-weight: 900;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      margin-bottom: 10px;
      text-transform: uppercase;
      letter-spacing: 2px;
      animation: glow 3s ease-in-out infinite;
    }

    @keyframes glow {
      0%, 100% { filter: drop-shadow(0 0 20px rgba(102, 126, 234, 0.4)); }
      50% { filter: drop-shadow(0 0 30px rgba(118, 75, 162, 0.6)); }
    }

    .label {
      width: 480px;
      min-height: 120px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, rgba(102, 126, 234, 0.15) 0%, rgba(118, 75, 162, 0.15) 100%);
      backdrop-filter: blur(20px);
      border: 2px solid rgba(255, 255, 255, 0.1);
      border-radius: 20px;
      font-weight: 700;
      font-size: 24px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5), 
                  0 0 40px rgba(102, 126, 234, 0.2);
      user-select: none;
      padding: 25px;
      text-align: center;
      transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      position: relative;
      overflow: hidden;
    }

    .label::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.03), transparent);
      transform: rotate(45deg);
      animation: shimmer 3s infinite;
    }

    @keyframes shimmer {
      0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
      100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
    }

    .label.hit {
      background: linear-gradient(135deg, rgba(0, 255, 157, 0.3) 0%, rgba(0, 204, 255, 0.3) 100%);
      border-color: rgba(0, 255, 157, 0.5);
      box-shadow: 0 20px 60px rgba(0, 255, 157, 0.4),
                  0 0 60px rgba(0, 255, 157, 0.3);
      animation: pulse 0.6s ease-in-out;
    }

    .label.miss {
      background: linear-gradient(135deg, rgba(255, 102, 102, 0.15) 0%, rgba(255, 51, 102, 0.15) 100%);
      animation: shake 0.4s ease-in-out;
    }

    @keyframes pulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.05); }
    }

    @keyframes shake {
      0%, 100% { transform: translateX(0); }
      25% { transform: translateX(-10px); }
      75% { transform: translateX(10px); }
    }

    .stats-container {
      display: flex;
      gap: 20px;
      margin: 10px 0;
    }

    .stat-card {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 15px;
      padding: 20px 30px;
      min-width: 150px;
      transition: all 0.3s ease;
    }

    .stat-card:hover {
      background: rgba(255, 255, 255, 0.08);
      transform: translateY(-5px);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    }

    .stat-label {
      font-size: 12px;
      text-transform: uppercase;
      letter-spacing: 1px;
      opacity: 0.6;
      margin-bottom: 8px;
    }

    .stat-value {
      font-size: 32px;
      font-weight: 900;
      background: linear-gradient(135deg, #00ff9d 0%, #00ccff 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .stat-value.attempts {
      background: linear-gradient(135deg, #ffcc00 0%, #ff9d00 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .button-group {
      display: flex;
      gap: 15px;
      margin: 15px 0;
    }

    button {
      padding: 16px 32px;
      border-radius: 15px;
      border: none;
      font-weight: 700;
      font-size: 16px;
      cursor: pointer;
      transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      position: relative;
      overflow: hidden;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    button::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      width: 0;
      height: 0;
      border-radius: 50%;
      background: rgba(255, 255, 255, 0.3);
      transform: translate(-50%, -50%);
      transition: width 0.6s, height 0.6s;
    }

    button:active::before {
      width: 300px;
      height: 300px;
    }

    #rollBtn {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: #fff;
      box-shadow: 0 10px 30px rgba(102, 126, 234, 0.4);
    }

    #rollBtn:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 40px rgba(102, 126, 234, 0.6);
    }

    #rollBtn:active {
      transform: translateY(0);
    }

    #autoBtn {
      background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
      color: #fff;
      box-shadow: 0 10px 30px rgba(240, 147, 251, 0.4);
    }

    #autoBtn:hover {
      transform: translateY(-3px);
      box-shadow: 0 15px 40px rgba(240, 147, 251, 0.6);
    }

    #autoBtn.active {
      background: linear-gradient(135deg, #ff6b6b 0%, #c92a2a 100%);
    }

    .picked {
      margin-top: 15px;
      font-size: 14px;
      opacity: 0.8;
      color: #ddd;
      padding: 12px 24px;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 10px;
      border: 1px solid rgba(255, 255, 255, 0.1);
      font-family: 'Courier New', monospace;
    }

    .sub {
      font-size: 13px;
      opacity: 0.6;
      margin-top: 10px;
    }

    .sub code {
      background: rgba(255, 255, 255, 0.1);
      padding: 4px 10px;
      border-radius: 6px;
      font-family: 'Courier New', monospace;
      color: #00ff9d;
    }

    .history {
      background: rgba(0, 0, 0, 0.3);
      backdrop-filter: blur(20px);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 20px;
      max-height: 80vh;
      width: 400px;
      overflow-y: auto;
      padding: 25px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
    }

    .history::-webkit-scrollbar {
      width: 8px;
    }

    .history::-webkit-scrollbar-track {
      background: rgba(255, 255, 255, 0.05);
      border-radius: 10px;
    }

    .history::-webkit-scrollbar-thumb {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      border-radius: 10px;
    }

    .history strong {
      display: block;
      font-size: 18px;
      font-weight: 700;
      margin-bottom: 15px;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .history-entry {
      padding: 12px 15px;
      margin: 8px 0;
      border-radius: 10px;
      font-size: 13px;
      line-height: 1.5;
      background: rgba(255, 255, 255, 0.03);
      border-left: 3px solid rgba(255, 255, 255, 0.2);
      transition: all 0.2s ease;
      animation: slideIn 0.3s ease;
    }

    @keyframes slideIn {
      from {
        opacity: 0;
        transform: translateX(-20px);
      }
      to {
        opacity: 1;
        transform: translateX(0);
      }
    }

    .history-entry:hover {
      background: rgba(255, 255, 255, 0.06);
      transform: translateX(5px);
    }

    .hit {
      color: #00ff9d;
      font-weight: bold;
      border-left-color: #00ff9d;
      background: rgba(0, 255, 157, 0.08);
    }

    .miss {
      color: #ff9999;
      border-left-color: #ff6666;
    }

    @media (max-width: 1024px) {
      .layout {
        flex-direction: column;
        align-items: center;
      }
      
      .history {
        width: 90%;
        max-width: 480px;
      }
      
      .label {
        width: 90%;
        max-width: 480px;
      }
    }
  </style>
</head>
<body>
  <div class="particles" id="particles"></div>

  <div class="layout">
    <div class="container">
      <div class="title">🎲 RNG MASTER</div>
      
      <div id="label" class="label">Press Roll to Begin</div>
      
      <div class="stats-container">
        <div class="stat-card">
          <div class="stat-label">🎯 Total Hits</div>
          <div class="stat-value" id="counter">0</div>
        </div>
        <div class="stat-card">
          <div class="stat-label">🔄 Attempts</div>
          <div class="stat-value attempts" id="attempt">0</div>
        </div>
      </div>

      <div class="button-group">
        <button id="rollBtn">🎲 Roll</button>
        <button id="autoBtn">▶️ Auto Roll</button>
      </div>

      <div id="picked" class="picked">Picked: None yet</div>
      <div class="sub">Primary Target: <code>tttttttttttttg</code></div>
    </div>

    <div id="history" class="history">
      <strong>📜 Roll History</strong>
      <div class="history-entry">No attempts yet. Press Roll to start!</div>
    </div>
  </div>

  <script>
    const particlesContainer = document.getElementById('particles');
    for (let i = 0; i < 15; i++) {
      const particle = document.createElement('div');
      particle.className = 'particle';
      particle.style.width = Math.random() * 100 + 50 + 'px';
      particle.style.height = particle.style.width;
      particle.style.left = Math.random() * 100 + '%';
      particle.style.top = Math.random() * 100 + '%';
      particle.style.background = `linear-gradient(135deg, rgba(102, 126, 234, 0.3), rgba(118, 75, 162, 0.3))`;
      particle.style.animationDelay = Math.random() * 20 + 's';
      particle.style.animationDuration = Math.random() * 20 + 20 + 's';
      particlesContainer.appendChild(particle);
    }

    const strings = [
      "tttttttttttttg", "Yes!", "No!", "Maybe...", "Hmm...", "Error: undefined", "Success!", 
      "Try again later", "Absolutely!", "Probably not", "Wait—what?", "Loading...", "Done!", 
      "Calculating...", "Processing...", "Lucky guess?", "Better luck next time!", "Not today", 
      "Whoops!", "Yesn't", "Why tho?", "You wish!", "Suspicious...", "Almost!", "Retry?", "Boom!", 
      "Kaboom!", "System overloaded", "404 Not Found", "Approved", "Denied", "Granted", "Refused", 
      "It's fate!", "Coin flip...", "Heads!", "Tails!", "Yup", "Nope", "Try harder!", "L", "W", 
      "Maybe later", "Hmmmm", "Suspense...", "Wait for it...", "Ha!", "Glitched?", "Randomized!", 
      "Pick again", "Recalculating...", "Deja vu", "In progress...", "Pending...", "Done already?", 
      "Yay!", "Bruh", "Seriously?", "Hmm.", "Oh no", "Oh yes", "Why not?", "Wait...", "Processing error", 
      "Debugging...", "Restart required", "Rebooting...", "Reticulating splines...", "Loading data...", 
      "Success!!", "Try one more time", "No signal", "Powering up...", "Access granted", "Access denied", 
      "Hello world!", "Ping!", "Pong!", "Beep boop", "Calculating odds...", "Luck = 0", "Luck = 100", 
      "This is fine", "That's illegal", "Corrupted", "Rewriting reality...", "You saw nothing", 
      "RNG loves you", "RNG hates you", "Neutral outcome", "Cosmic balance...", "Out of bounds", 
      "Random seed", "Try again?", "Maybe yes", "Maybe no", "Quantum fluctuation", "Entropy rising...",
      "404: Luck not found", "Achievement unlocked!", "Connection lost", "Reconnecting...", "Critical hit!",
      "Miss!", "Dodge!", "Parry!", "Blocked!", "Evaded!", "One-shot!", "Clutch!", "GG", "EZ", "Diff",
      "Skill issue", "Git gud", "Based", "Cringe", "Sheesh", "Bussin", "Cap", "No cap", "Fr fr",
      "Ratio", "Touch grass", "Certified moment", "Peak fiction", "Mid", "Bussin fr", "Slay",
      "Downloading...", "Installing...", "Initializing...", "Compiling...", "Extracting...", 
      "Validating...", "Authenticating...", "Synchronizing...", "Optimizing...", "Finalizing...",
      "Stack overflow", "Segmentation fault", "Memory leak", "Buffer overflow", "Null pointer",
      "Undefined behavior", "Race condition", "Deadlock detected", "Thread blocked", "Timeout",
      "Connection refused", "Server error", "Client error", "Bad request", "Unauthorized",
      "Forbidden", "Payment required", "Gone", "I'm a teapot", "Too many requests",
      "Service unavailable", "Gateway timeout", "Network error", "DNS failure", "SSL error",
      "Certificate expired", "Handshake failed", "Protocol error", "Parse error", "Syntax error",
      "Type error", "Reference error", "Range error", "Eval error", "URI error",
      "Breaking news!", "Alert!", "Warning!", "Caution!", "Notice", "Info", "Debug mode",
      "Verbose output", "Silent mode", "Stealth enabled", "Invisible", "Cloaked", "Hidden",
      "Revealed!", "Exposed!", "Discovered!", "Found!", "Located!", "Tracked!", "Monitored!",
      "Scanning...", "Searching...", "Seeking...", "Hunting...", "Pursuing...", "Chasing...",
      "Fleeing...", "Escaping...", "Running...", "Hiding...", "Ducking...", "Dodging...",
      "Weaving...", "Rolling...", "Jumping...", "Flying...", "Falling...", "Crashing...",
      "Exploding...", "Imploding...", "Expanding...", "Contracting...", "Rotating...", "Spinning...",
      "Vibrating...", "Oscillating...", "Pulsating...", "Throbbing...", "Beating...", "Pumping...",
      "Flowing...", "Streaming...", "Rushing...", "Surging...", "Flooding...", "Draining...",
      "Filling...", "Emptying...", "Charging...", "Discharging...", "Energizing...", "Depleting...",
      "Maximum power!", "Low battery", "Critical level", "Full capacity", "Overcharged!", "Drained",
      "Supercharged!", "Hyper mode!", "Turbo boost!", "Nitro active!", "Overdrive!", "Beast mode!",
      "God mode!", "Creative mode", "Survival mode", "Hardcore mode", "Peaceful mode", "Spectator mode",
      "Observer mode", "Admin mode", "Developer mode", "Debug mode", "Test mode", "Production mode",
      "Maintenance mode", "Safe mode", "Emergency mode", "Panic mode", "Chaos mode", "Order mode",
      "Balanced", "Unbalanced", "Stable", "Unstable", "Secure", "Insecure", "Safe", "Unsafe",
      "Protected", "Exposed", "Encrypted", "Decrypted", "Hashed", "Salted", "Compressed", "Decompressed",
      "Archived", "Extracted", "Backed up", "Restored", "Saved", "Loaded", "Cached", "Cleared",
      "Refreshed", "Updated", "Upgraded", "Downgraded", "Patched", "Fixed", "Broken", "Working",
      "Functional", "Dysfunctional", "Operational", "Offline", "Online", "Connected", "Disconnected",
      "Linked", "Unlinked", "Paired", "Unpaired", "Synced", "Desynced", "Matched", "Mismatched",
      "Aligned", "Misaligned", "Calibrated", "Uncalibrated", "Tuned", "Detuned", "Optimized", "Unoptimized",
      "Efficient", "Inefficient", "Fast", "Slow", "Quick", "Sluggish", "Rapid", "Gradual",
      "Instant", "Delayed", "Immediate", "Postponed", "Now", "Later", "Soon", "Eventually",
      "Never", "Always", "Sometimes", "Often", "Rarely", "Occasionally", "Frequently", "Constantly",
      "Perpetually", "Temporarily", "Permanently", "Briefly", "Momentarily", "Indefinitely", "Forever", "Eternity",
      "Infinity", "Zero", "One", "Two", "Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten",
      "Jackpot!", "Bonus round!", "Extra life!", "Game over", "Continue?", "Insert coin", "Ready?",
      "Fight!", "K.O.!", "Perfect!", "Excellent!", "Great!", "Good", "OK", "Bad", "Terrible", "Awful",
      "Legendary!", "Epic!", "Rare!", "Uncommon", "Common", "Trash", "Worthless", "Priceless", "Valuable",
      "Cosmic ray detected", "Singularity formed", "Black hole nearby", "Wormhole opened", "Time paradox",
      "Reality glitch", "Matrix error", "Simulation lag", "NPC behavior", "Main character energy",
      "Plot armor active", "Foreshadowing...", "Cliffhanger!", "Plot twist!", "Easter egg found!",
      "Secret unlocked!", "Hidden achievement", "Rare drop!", "Legendary loot!", "Mythic tier!",
      "Cursed item", "Blessed artifact", "Enchanted", "Disenchanted", "Forged", "Crafted", "Assembled",
      "Big brain time", "Galaxy brain", "Smooth brain", "Wrinkly brain", "Brain blast!", "Eureka!",
      "Aha moment!", "Lightbulb!", "Inspired!", "Motivated!", "Determined!", "Focused!", "Distracted...",
      "Vibing", "Chillin", "Grindin", "Hustlin", "Ballin", "Flexin", "Stuntin", "Wildin", "Actin up",
      "Zonked", "Boomed", "Yeet!", "Kobe!", "Swish!", "Nothing but net", "Airball", "Brick", "Posterized!",
      "Crossed up!", "Ankles broken!", "Dunked on!", "Rejected!", "Swatted!", "Blocked!", "Stuffed!",
      "And one!", "Foul!", "Technical!", "Flagrant!", "Ejected!", "Benched", "Subbed in", "MVP!", "GOAT!",
      "Hall of Fame", "All-star", "Rookie", "Veteran", "Legend", "Icon", "Pioneer", "Innovator", "Creator",
      "Destroyer", "Builder", "Breaker", "Maker", "Taker", "Giver", "Keeper", "Seeker", "Finder", "Loser",
      "Winner", "Champion", "Runner-up", "Third place", "Participant", "Spectator", "Observer", "Witness",
      "No witnesses", "Leave no trace", "Ghost protocol", "Shadow ops", "Stealth mission", "Infiltration",
      "Exfiltration", "Extraction", "Insertion", "Deployment", "Retrieval", "Recovery", "Rescue", "Abort!",
      "Self-destruct!", "Countdown started", "T-minus 10", "Ignition!", "Liftoff!", "We have liftoff!",
      "Houston, we have a problem", "Mission accomplished", "Objective complete", "Target eliminated",
      "Package secured", "Area cleared", "All clear", "Hostiles detected", "Engage!", "Retreat!", "Fall back!",
      "Hold position!", "Advance!", "Charge!", "Push forward!", "Stand ground!", "Take cover!", "Suppressing fire!",
      "Reloading!", "Out of ammo!", "Need backup!", "On my way!", "Roger that", "Copy that", "10-4",
      "Affirmative", "Negative", "Stand by", "Go ahead", "Over and out", "Wilco", "Mayday!", "SOS!",
      "Emergency!", "Code red!", "Code blue", "Code green", "All hands on deck!", "Battle stations!",
      "Red alert!", "Condition one", "DEFCON 1", "Nuclear launch detected", "Incoming!", "Brace!",
      "Impact!", "Direct hit!", "Near miss", "Glancing blow", "Ricochet", "Deflected", "Absorbed",
      "Nullified", "Negated", "Cancelled", "Reversed", "Reflected", "Redirected", "Amplified", "Weakened",
      "Buffed", "Nerfed", "Balanced", "OP", "Underpowered", "Broken", "Fixed", "Patched", "Hotfix deployed"
    ];

    const TARGETS = [
      "tttttttttttttg", "Success!", "Kaboom!", "Ping!", "Coin flip...", "You saw nothing", 
      "Entropy rising...", "Access granted", "Hello world!", "Recalculating...", 
      "Reticulating splines...", "Random seed", "Quantum fluctuation", "RNG loves you", 
      "Cosmic balance...", "Achievement unlocked!", "Critical hit!", "Jackpot!", 
      "Legendary!", "Secret unlocked!", "Mythic tier!", "MVP!", "GOAT!", "Winner",
      "Champion", "Mission accomplished", "Perfect!", "God mode!", "Maximum power!",
      "Supercharged!", "Hyper mode!", "Turbo boost!", "Big brain time", "Galaxy brain",
      "Eureka!", "Easter egg found!", "Legendary loot!", "Plot twist!", "Blessed artifact",
      "Hall of Fame", "All-star", "Posterized!", "Direct hit!", "We have liftoff!",
      "Objective complete", "Buffed", "Legendary drop!", "Clutch!", "One-shot!"
    ];

    const MAX_HISTORY = 100;
    const DEBOUNCE_TIME = 500;

    const labelEl = document.getElementById('label');
    const pickedEl = document.getElementById('picked');
    const rollBtn = document.getElementById('rollBtn');
    const autoBtn = document.getElementById('autoBtn');
    const counterEl = document.getElementById('counter');
    const attemptEl = document.getElementById('attempt');
    const historyEl = document.getElementById('history');

    let hitCount = 0;
    let attemptCount = 0;
    let historyLog = [];
    let canRoll = true;
    let autoRolling = false;
    let autoInterval = null;

    function randomIndex(max) {
      if (window.crypto && window.crypto.getRandomValues) {
        const arr = new Uint32Array(1);
        window.crypto.getRandomValues(arr);
        return arr[0] % max;
      } else return Math.floor(Math.random() * max);
    }

    function updateHistoryDisplay() {
      if (historyLog.length === 0) {
        historyEl.innerHTML = "<strong>📜 Roll History</strong><div class='history-entry'>No attempts yet. Press Roll to start!</div>";
        return;
      }
      const entries = historyLog.slice(-50).reverse().map(entry => {
        const colorClass = entry.hit ? "hit" : "miss";
        const emoji = entry.hit ? "🎯" : "❌";
        return `<div class="history-entry ${colorClass}">${emoji} #${entry.attempt}: "${entry.string}" ${entry.hit ? "<strong>HIT!</strong>" : ""}</div>`;
      }).join("");
      historyEl.innerHTML = "<strong>📜 Roll History</strong>" + entries;
    }

    function rollOnce() {
      if (!canRoll) return;
      canRoll = false;
      setTimeout(() => canRoll = true, DEBOUNCE_TIME);

      attemptCount++;
      const idx = randomIndex(strings.length);
      const picked = strings[idx];
      const isHit = TARGETS.includes(picked);

      labelEl.classList.remove('hit', 'miss');

      if (isHit) {
        labelEl.textContent = "🎯 RNG HIT! The target string was picked!";
        labelEl.classList.add('hit');
        hitCount++;
        historyLog.push({ attempt: attemptCount, string: picked, hit: true });
        attemptCount = 0;
      } else {
        labelEl.textContent = `❌ RNG missed. Nothing happens.`;
        labelEl.classList.add('miss');
        historyLog.push({ attempt: attemptCount, string: picked, hit: false });
      }

      if (historyLog.length > MAX_HISTORY) {
        historyLog = historyLog.slice(-MAX_HISTORY);
      }

      updateHistoryDisplay();
      counterEl.textContent = hitCount;
      pickedEl.textContent = `Picked: "${picked}"`;
      attemptEl.textContent = attemptCount;
    }

    rollBtn.addEventListener("click", rollOnce);

    autoBtn.addEventListener("click", () => {
      if (!autoRolling) {
        autoRolling = true;
        autoBtn.textContent = "⏸️ Stop Auto";
        autoBtn.classList.add('active');
        autoInterval = setInterval(rollOnce, 500);
      } else {
        autoRolling = false;
        autoBtn.textContent = "▶️ Auto Roll";
        autoBtn.classList.remove('active');
        clearInterval(autoInterval);
      }
    });

    updateHistoryDisplay();
  </script>
</body>
</html>
