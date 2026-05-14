document.open();
document.write(`
<!DOCTYPE html>
<html lang="en">
<head>

    <base href="https://cdn.jsdelivr.net/gh/moony9999/Voxtek-OS/">

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>gn-math</title>

    <link rel="icon" type="image/png" href="favicon.png">
    <link rel="apple-touch-icon" href="favicon.png">

    <style>
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            background: #0f172a;
            font-family: Arial, sans-serif;
        }

        #topbar {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            height: 52px;
            background: linear-gradient(135deg,#fc2651,#e91e47);
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 14px;
            box-sizing: border-box;
            z-index: 9999;
            color: white;
            box-shadow: 0 4px 10px rgba(0,0,0,.35);
        }

        #logo {
            font-size: 20px;
            font-weight: bold;
        }

        #controls {
            display: flex;
            gap: 10px;
        }

        .btn {
            background: rgba(255,255,255,.15);
            border: 1px solid rgba(255,255,255,.25);
            color: white;
            padding: 8px 14px;
            border-radius: 10px;
            cursor: pointer;
            transition: .2s;
            font-weight: 600;
        }

        .btn:hover {
            background: rgba(255,255,255,.25);
            transform: translateY(-1px);
        }

        #viewer {
            position: absolute;
            top: 52px;
            left: 0;
            width: 100%;
            height: calc(100% - 52px);
            border: none;
        }
    </style>

    <script>
        window.addEventListener('beforeunoad', function (event) {
            event.preventDefault();
            event.returnValue = '';
        });

        function fullscreenFrame() {
            const iframe = document.getElementById('viewer');

            if (iframe.requestFullscreen) {
                iframe.requestFullscreen();
            } else if (iframe.webkitRequestFullscreen) {
                iframe.webkitRequestFullscreen();
            } else if (iframe.msRequestFullscreen) {
                iframe.msRequestFullscreen();
            }
        }

        function reloadFrame() {
            document.getElementById('viewer').src =
                "OP%20VOXTEK.html?t=" + Date.now();
        }

        function openBlank() {
            window.open("OP%20VOXTEK.html", "_blank");
        }
    </script>

</head>

<body>

    <div id="topbar">
        <div id="logo">gn-math</div>

        <div id="controls">
            <button class="btn" onclick="reloadFrame()">Refresh</button>
            <button class="btn" onclick="fullscreenFrame()">Fullscreen</button>
            <button class="btn" onclick="openBlank()">Open Tab</button>
        </div>
    </div>

    <iframe
        id="viewer"
        src="OP%20VOXTEK.html"
        allowfullscreen>
    </iframe>

</body>
</html>
`);
document.close();
