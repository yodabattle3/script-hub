<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Script Hub</title>
    <style>
        :root {
            /* Primary Colors */
            --primary-bg: #191919;
            --secondary-bg: #252525;

            /* scripts  */
            --card-bg: #2a2a2a;
            --primary-text: #f833ff; /* main theme like mostly everything thats Purple*/
            --secondary-text: #ffffff;
            --accent-color: #ffcc00;

             /* Search bar  */
            --button-color: #8814b6;
            --button-hover: #ff5555;

            /* verified badges */
            --verified-tag: #00cc66;
            --not-verified-tag: #ff4757;

             /* notification button */
            --notification-bg: rgba(25, 25, 25, 0.9);

            /* copy button */
            --copy-button: #3399ff;
            --copy-button-hover: #66b3ff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--primary-bg);
            color: var(--secondary-text);
            padding: 20px;
        }

        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 30px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--primary-text);
        }

        .title {
            font-size: 28px;
            font-weight: bold;
            color: var(--primary-text);
            text-shadow: 0 0 5px rgba(255, 51, 51, 0.3);
        }

        .search-container {
            display: flex;
            align-items: center;
        }

        .search-input {
            padding: 10px 15px;
            border-radius: 20px;
            border: 1px solid var(--primary-text);
            background-color: var(--secondary-bg);
            color: var(--secondary-text);
            width: 250px;
            font-size: 14px;
            outline: none;
            transition: all 0.3s ease;
        }

        .search-input:focus {
            box-shadow: 0 0 5px var(--primary-text);
        }

        .search-button {
            background-color: var(--button-color);
            color: var(--secondary-text);
            border: none;
            border-radius: 20px;
            padding: 10px 15px;
            margin-left: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .search-button:hover {
            background-color: var(--button-hover);
        }

        .scripts-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }

        .script-card {
            background-color: var(--card-bg);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            border: 1px solid #333333;
        }

        .script-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.4);
            border-color: var(--primary-text);
        }

        .script-image-container {
            position: relative;
            height: 180px;
            overflow: hidden;
        }

        .script-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .script-card:hover .script-image {
            transform: scale(1.05);
        }

        .verification-tag {
            position: absolute;
            top: 10px;
            right: 10px;
            background-color: var(--verified-tag);
            color: #000;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 12px;
            z-index: 1;
        }

        .not-verified {
            background-color: var(--not-verified-tag);
        }

        .script-content {
            padding: 15px;
        }

        .script-title {
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 10px;
            color: var(--primary-text);
        }

        .script-description {
            font-size: 14px;
            color: var(--secondary-text);
            margin-bottom: 15px;
            line-height: 1.5;
            height: 63px;
            overflow: hidden;
        }

        .copy-button {
            width: 100%;
            padding: 10px;
            background-color: var(--copy-button);
            color: var(--secondary-text);
            border: 2px solid #ffffff;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
        }

        .copy-button:hover {
            background-color: var(--copy-button-hover);
            transform: scale(1.02);
        }

        .no-results {
            grid-column: 1 / -1;
            text-align: center;
            padding: 30px;
            font-size: 18px;
            color: var(--secondary-text);
        }

        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            background-color: var(--notification-bg);
            color: var(--secondary-text);
            border-left: 4px solid var(--verified-tag);
            padding: 15px 20px;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: transform 0.3s ease, opacity 0.3s ease;
            transform: translateX(120%);
            opacity: 0;
        }

        .notification.show {
            transform: translateX(0);
            opacity: 1;
        }

        .notification-title {
            font-weight: bold;
            margin-bottom: 5px;
            color: var(--primary-text);
        }

        .notification-message {
            font-size: 14px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1 class="title">Script Hub</h1>
        <div class="search-container">
            <input type="text" id="searchInput" class="search-input" placeholder="Search scripts...">
            <button class="search-button" onclick="searchScripts()">Search</button>
        </div>
    </div>

    <div class="scripts-container" id="scriptsContainer">
        <!-- Script cards will be dynamically added here -->
    </div>

    <div class="notification" id="notification">
        <div class="notification-title" id="notificationTitle">Success</div>
        <div class="notification-message" id="notificationMessage"></div>
    </div>

    <script>
        
        class Script {
            constructor(id, title, description, imagePath, scriptContent, verified = true) {
                this.id = id;
                this.title = title;
                this.description = description;
                this.imagePath = imagePath;
                this.scriptContent = scriptContent;
                this.verified = verified;
            }
        }

      
       const scripts = [
            new Script(
                "script1",
                "ANIMAL SIMULATOR GUI",
                "ANIMAL SIMULATOR GUI With many features such as esp, autfarm, kill aura, hitbox expander, and more!",
                "images/rko.png",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/Golddeathninja/af/refs/heads/main/a"))()'
            ),
            new Script(
                "script2",
                "WRD ESP",
                "Highlights all Player in the game",
                "images/b.png",
                "-- Auto Farm Script\nlocal function startFarming()\n    print(\"Auto Farming Started!\")\nend\n\nstartFarming()"
            ),
            new Script(
                "script3",
                "Rivals GUI",
                "- ESP - Infinite Jump - No Clip",
                "images/rivals.png",
                'print("rivals gui")'
            ),
            new Script(
                "script4",
                "AEYA Chat bypasser V2",
                "Allows you to Say anything in chat without being tagged",
                "images/ChatBypass.png",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/102827252527/Chatbypass/refs/heads/main/AEYAbypasser.txt"))()'
            ),
            new Script(
                "script5",
                "Server Finder",
                "Increase your movement speed to get around the map faster than ever.",
                "images/Server_Finder.png",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/Isnotalwi/Roblox-Script/refs/heads/main/Finder%20Server%20Beta.lua"))()'
            ),
            new Script(
                "script6",
                "Simple Spy",
                "impleSpy is a penetration testing tool designed to intercept remote calls from the client to the server.",
                "images/SimpleSpy.png",
                'loadstring(game:HttpGet("https://github.com/exxtremestuffs/SimpleSpySource/raw/master/SimpleSpy.lua"))()'
				 ),
            new Script(
                "script7",
                "Fisch Script",
                "This fisch script is very good and has no key system which makes it pretty sigma dont you think and was made by skidware_m .",
                "images/Fisch1.png",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/skidware-m/fischscript-by-skidware_m/refs/heads/main/patohub%201.2.1%20newest%20but%20encrypted.lua"))()'
				),
            new Script(
                "script8",
                "The script has been around for very long since the first days of roblox exploting.",
                "images/yeild.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()'
				),
            new Script(
                "script9",
                "Car Crushers",
                "This script is to help you teleport around the game and macro and troll people .",
                "images/carcrash.jpg",
                'loadstring(game:HttpGet("https://gist.githubusercontent.com/dkdc123/4c6ddbd228028476f6400611b3b9b50c/raw/77e502a6ecbf6d880048d23677b99e3ca60772a4/gistfile1.txt"))()'
				),
            new Script(
                "script10",
                "Tabohub",
                "A good dead rails script .",
                "images/deads.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/refs/heads/main/TbaoHubDeadRails"))()'
				),
            new Script(
                "script11",
                "Dex explorer",
                "Used to see the files inside of the game .",
                "images/dex.jpg",
                'loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Dex%20Explorer.txt"))()'
				),
            new Script(
                "script12",
                "Ez hub",
                "popular script hub .",
                "images/ezhub.png",
                'loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Ez%20Hub.txt"))()'
				),
            new Script(
                "script13",
                "Blue lock",
                "helps you run and many other over 50 features .",
                "images/bluelock.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/Bhusant/Bathroom-attack/refs/heads/main/Bathroom"))()'
				),
            new Script(
                "script14",
                "SpeedHub X",
                "Supports the most popular games .",
                "images/dex.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()'
				),
            new Script(
                "script15",
                "Da hood ",
                "very good script.",
                "images/dahood.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/Bhusant/Bathroom-attack/refs/heads/main/Bathroom"))()'
				),
            new Script(
                "script16",
                "Da hood Modded",
                "BEST DA HOOD script ever.",
                "images/dahood.jpg",
                'loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/Rippeed/DaHoodinary/main/chariotsware"))()'
				),
            new Script(
                "script17",
                "Blade ball",
                "project tj script is very overpowered.",
                "images/bladeball.jpg",
                'loadstring(game:HttpGetAsync("https://lua-library.btteam.net/script-auth.txt"))()'
				),
            new Script(
                "script18",
                "Jail break",
                "lots of features over 50.",
                "images/jailbreak.jpg",
                'loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/730854e5b6499ee91deb1080e8e12ae3.lua"))()'
				),
            new Script(
                "script19",
                "Build a boat",
                "ONE OF THE BEST SCRIPTS EVER MADE OF BUILD A BOAT VERY OP.",
                "images/buildaboat.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/TheRealAsu/BABFT/refs/heads/main/Jan25_Source.lua"))()'
				),
            new Script(
                "script20",
                "blox fruits",
                "lets be real who plays blox fruits but this script is pretty good.",
                "images/bloxfruits.jpg",
                'loadstring(game:HttpGet("https://lua-library.btteam.net/script-auth.txt"))()'
               ),
            new Script(
                "script20",
                "troll",
                "pretty sigma troll script.",
                "images/troll.jpg",
                'loadstring(game:HttpGet("https://raw.githubusercontent.com/Bhusant/Bathroom-attack/refs/heads/main/Bathroom"))()'
            ),
        ];

        
        function renderScripts(scriptsToRender = scripts) {
            const container = document.getElementById('scriptsContainer');
            container.innerHTML = '';

            if (scriptsToRender.length === 0) {
                container.innerHTML = '<div class="no-results">No scripts found matching your search.</div>';
                return;
            }

            scriptsToRender.forEach(script => {
                const scriptCard = document.createElement('div');
                scriptCard.className = 'script-card';
                scriptCard.id = script.id;

                scriptCard.innerHTML = `
                    <div class="script-image-container">
                        <div class="verification-tag ${!script.verified ? 'not-verified' : ''}">
                            ${script.verified ? 'Verified' : 'Not Verified'}
                        </div>
                        <img src="${script.imagePath}" alt="${script.title}" class="script-image">
                    </div>
                    <div class="script-content">
                        <h3 class="script-title">${script.title}</h3>
                        <p class="script-description">${script.description}</p>
                        <button class="copy-button" onclick="copyScriptToClipboard('${script.id}')">Copy Script</button>
                    </div>
                `;

                container.appendChild(scriptCard);
            });
        }

        
        function copyScriptToClipboard(scriptId) {
            const script = scripts.find(s => s.id === scriptId);
            if (script) {
                
                const textarea = document.createElement('textarea');
                textarea.value = script.scriptContent;
                document.body.appendChild(textarea);
                textarea.select();
                
                try {
                    
                    document.execCommand('copy');
                    showNotification("Success", `${script.title} copied to clipboard!`);
                } catch (err) {
                    console.error('Failed to copy text: ', err);
                }
                
                
                document.body.removeChild(textarea);
            }
        }

        
        function showNotification(title, message) {
            const notification = document.getElementById('notification');
            const notificationTitle = document.getElementById('notificationTitle');
            const notificationMessage = document.getElementById('notificationMessage');
            
            notificationTitle.textContent = title;
            notificationMessage.textContent = message;
            
            notification.classList.add('show');
            
            
            setTimeout(() => {
                notification.classList.remove('show');
            }, 3000);
        }

        
        function searchScripts() {
            const searchTerm = document.getElementById('searchInput').value.toLowerCase();
            
            if (!searchTerm) {
                renderScripts();
                return;
            }
            
            const filteredScripts = scripts.filter(script =>
                script.title.toLowerCase().includes(searchTerm) ||
                script.description.toLowerCase().includes(searchTerm)
            );
            
            renderScripts(filteredScripts);
        }

        
        document.getElementById('searchInput').addEventListener('input', searchScripts);

        
        window.onload = function() {
            renderScripts();
        };

        
        function addScript(title, description, imagePath, scriptContent, verified = true) {
            const id = "script" + (scripts.length + 1);
            const newScript = new Script(id, title, description, imagePath, scriptContent, verified);
            scripts.push(newScript);
            renderScripts();
            return newScript;
        }

        
        window.ScriptHub = {
            copyScriptToClipboard,
            addScript
        };
    </script>
</body>
</html>
