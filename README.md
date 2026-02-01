# Valentine-
Will you be my valentine?
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        body { text-align: center; font-family: sans-serif; background: #fff0f5; padding-top: 100px; }
        h1 { color: #d63384; }
        .btn { padding: 15px 30px; font-size: 20px; cursor: pointer; border: none; border-radius: 10px; margin: 10px; transition: 0.2s; }
        #yes { background: #4CAF50; color: white; }
        #no { background: #f44336; color: white; position: relative; }
    </style>
</head>
<body>
    <h1>Will you be my Valentine? ❤️</h1>
    <button id="yes" class="btn" onclick="alert('Yay! 🚀 Merging heart into main branch...')">YES</button>
    <button id="no" class="btn" onmouseover="moveButton()" onclick="moveButton()">NO</button>

    <script>
        function moveButton() {
            const noBtn = document.getElementById('no');
            // Make it disappear or jump away
            const x = Math.random() * (window.innerWidth - noBtn.offsetWidth);
            const y = Math.random() * (window.innerHeight - noBtn.offsetHeight);
            noBtn.style.position = 'absolute';
            noBtn.style.left = x + 'px';
            noBtn.style.top = y + 'px';
            
            // Randomly make it disappear for a second to be extra annoying/funny
            if(Math.random() > 0.5) {
                noBtn.style.display = 'none';
                setTimeout(() => { noBtn.style.display = 'inline-block'; }, 500);
            }
        }
    </script>
</body>
</html>
