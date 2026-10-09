LUMEN CONSOLE  -  install it as an app

What is in this folder
  index.html, manifest.webmanifest, sw.js, three icons.  Keep them together.

Option 1: quickest, no hosting (computer)
  Open lumen-standalone.html in Chrome, open the Chrome menu, find
  "Cast, save and share" and choose "Create shortcut", then tick "Open as window".
  (Menu names change a little between Chrome versions.)

Option 2: a real installable app (computer or phone)
  1. Put this whole folder on any free static web host (it must be https).
  2. Open the address in Chrome.
  3. Computer: click the install icon at the right end of the address bar.
     Phone: Chrome menu > Install app / Add to Home screen.
  Lumen then opens in its own window with its own icon.

Option 3: install from your own computer, no hosting
  1. Install Python, open a terminal in this folder and run:
       python3 -m http.server 8000
  2. Open http://localhost:8000 in Chrome and install from the address bar.
  3. After installing, the app should start from its icon even when the server is off.

Inside the app
  - Voice on: the core reacts to your voice. Clap twice (or press Power) to shut down or wake.
  - On-device brain: a free small AI that runs on your computer (Chrome with WebGPU).
  - API key: optional, only if you have one.
  - The microphone permission is asked once per site when installed from https or localhost.
