


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nitin Key Generator (Neon)</title>
    <style>
        /* Define Neon Colors and Glows */
        :root {
            --neon-green: #39ff14; /* Bright Neon Green */
            --neon-blue: #00ffff; /* Bright Neon Cyan/Blue */
            --dark-bg: #1a1a1a;
            --text-color: #f0f0f0;
        }

        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            background-color: var(--dark-bg);
            color: var(--text-color);
            text-align: center;
        }

        /* Neon Glow Effect Mixin */
        .neon-glow-green {
            text-shadow: 0 0 5px var(--neon-green), 0 0 10px var(--neon-green);
            box-shadow: 0 0 10px var(--neon-green), 0 0 20px var(--neon-green) inset;
        }

        .neon-glow-blue {
            text-shadow: 0 0 5px var(--neon-blue), 0 0 10px var(--neon-blue);
            box-shadow: 0 0 10px var(--neon-blue), 0 0 20px var(--neon-blue) inset;
        }

        /* Logo Styling */
        .logo-container {
            margin-bottom: 20px;
        }

        .logo-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--neon-blue); 
            box-shadow: 0 0 15px var(--neon-blue), 0 0 30px var(--neon-blue); /* Neon Blue Border Glow */
        }

        h1 {
            color: var(--text-color);
            margin-top: 10px;
            margin-bottom: 30px;
            font-size: 2.2em;
            letter-spacing: 3px;
            font-weight: 700;
            /* Applying Neon Green Glow to Heading */
            text-shadow: 0 0 7px var(--neon-green), 0 0 15px var(--neon-green);
        }

        /* Key Generator Box */
        .generator-box {
            background-color: #2b2b2b;
            padding: 30px;
            border-radius: 15px;
            border: 2px solid var(--neon-blue);
            box-shadow: 0 0 25px rgba(0, 255, 255, 0.4);
            width: 90%;
            max-width: 450px;
        }
        
        h3 {
            color: var(--neon-blue);
            text-shadow: 0 0 5px var(--neon-blue);
        }
        
        /* Links and Key Area */
        .link-buttons a, #generate-btn {
            display: block;
            width: 100%;
            padding: 12px;
            margin: 15px 0;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
        }

        .link-buttons a {
            background-color: transparent;
            color: var(--neon-green);
            border: 2px solid var(--neon-green);
        }

        .link-buttons a:hover {
            background-color: var(--neon-green);
            color: var(--dark-bg);
            box-shadow: 0 0 15px var(--neon-green);
        }

        #generate-btn {
            background-color: var(--neon-blue);
            color: var(--dark-bg);
            border: none;
            font-size: 1.2em;
            font-weight: 900;
        }
        
        #generate-btn:hover:not(:disabled) {
            box-shadow: 0 0 15px var(--neon-blue), 0 0 30px var(--neon-blue);
        }

        #generate-btn:disabled {
            background-color: #4a4a4a; /* Darker disabled color */
            color: #888;
            cursor: not-allowed;
            box-shadow: none;
        }
        
        /* Key Output Styling */
        .key-area {
            margin-top: 20px;
            padding: 15px;
            border: 2px dashed var(--neon-green);
            border-radius: 8px;
            background-color: #333;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        #key-output {
            color: var(--neon-green);
            font-size: 1.2em;
            font-weight: bold;
            word-break: break-all;
            text-shadow: 0 0 3px var(--neon-green);
            flex-grow: 1;
            text-align: left;
        }
        
        #copy-btn {
            margin-left: 10px;
            padding: 8px 12px;
            background-color: var(--neon-blue);
            color: var(--dark-bg);
            border: none;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        #copy-btn:hover {
             background-color: #00e0e0;
        }
        
        /* Notification Styling */
        #notification {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--neon-green);
            color: var(--dark-bg);
            padding: 10px 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px var(--neon-green);
            opacity: 0;
            transition: opacity 0.5s ease-in-out;
            font-weight: bold;
            z-index: 100;
        }
        
        #notification.show {
            opacity: 1;
        }
    </style>
</head>
<body>

    <div class="logo-container">
        <img src="https://i.ibb.co/1GhmSWtd/4eab94c04804ace625815663904f3ff6.jpg" alt="Nitin Logo" class="logo-img">
    </div>

    <h1 class="neon-glow-green">Nitin Key Generator</h1>

    <div class="generator-box">
        <h3>🔗 Key Activation Requirements</h3>
        <p>Key prapt karne ke liye, neeche diye gaye links ko **click karke open** karna zaroori hai:</p>

        <div class="link-buttons">
            <a href="https://youtube.com/@sanatanigamer90?si=EOpDfaO0ZnpqLN_9" target="_blank" onclick="linkClicked('yt')">
                🔴 YouTube Channel Kholo
            </a>
            <a href="https://t.me/+MVN6iStjmxIxNTBl" target="_blank" onclick="linkClicked('tg')">
                ✈️ Telegram Group Kholo
            </a>
        </div>
        
        <hr style="border-color: var(--neon-blue);">

        <button id="generate-btn" disabled>
            Key Generate Karein
        </button>

        <div class="key-area">
            <span id="key-output">
                </span>
            <button id="copy-btn" style="display:none;" onclick="copyKey()">
                Copy
            </button>
        </div>
    </div>
    
    <div id="notification">Key Copied Successfully!</div>

    <script>
        // Trackers and Elements
        let yt_clicked = false;
        let tg_clicked = false;
        const generateBtn = document.getElementById('generate-btn');
        const keyOutput = document.getElementById('key-output');
        const copyBtn = document.getElementById('copy-btn');
        const notification = document.getElementById('notification');
        const KEY_VALUE = "Nitin DIGITAL MODS"; // Defined the Key

        function checkConditions() {
            // Check if both links have been clicked
            if (yt_clicked && tg_clicked) {
                generateBtn.disabled = false; 
                generateBtn.textContent = "Key Generate Karein (Ready!)";
            } else {
                generateBtn.disabled = true; 
                generateBtn.textContent = "Pehle Dono Links Kholo";
            }
        }

        function linkClicked(linkType) {
            if (linkType === 'yt') {
                yt_clicked = true;
            } else if (linkType === 'tg') {
                tg_clicked = true;
            }
            checkConditions();
        }

        // --- Copy Key Functionality ---
        function copyKey() {
            // Use Clipboard API for modern browsers
            navigator.clipboard.writeText(keyOutput.textContent).then(() => {
                
                // Show Notification
                notification.textContent = "Key Copied: " + keyOutput.textContent;
                notification.classList.add('show');
                
                // Hide notification after 2 seconds
                setTimeout(() => {
                    notification.classList.remove('show');
                }, 2000);
            }).catch(err => {
                console.error('Could not copy text: ', err);
                alert('Copy failed! Please select and copy manually: ' + keyOutput.textContent);
            });
        }

        // Key generation logic
        generateBtn.addEventListener('click', () => {
            if (generateBtn.disabled) return; // Prevent action if somehow disabled

            // Display the key
            keyOutput.textContent = KEY_VALUE;
            
            // Show the copy button
            copyBtn.style.display = 'inline-block';
            
            // Update button status
            generateBtn.disabled = true;
            generateBtn.textContent = "Key Generated!";
            
            // Automatically copy key after generation (Optional)
            // copyKey(); 
        });

        // Initial check on page load
        keyOutput.textContent = "Click generate to see your key...";
        checkConditions();
    </script>
</body>
</html>
