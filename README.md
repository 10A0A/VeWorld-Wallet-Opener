
VeWorld Wallet Opener
A simple tool to open the VeWorld Wallet in your browser with a button. This project contains one HTML file with a button that tries to connect to the VeWorld Wallet (a Web3 wallet for the VeChainThor blockchain).

What You Need
Browser : Google Chrome or Microsoft Edge.
VeWorld Wallet : Install the VeWorld extension in your browser.
Optional: A local web server (e.g., Python) if you have issues with file:// URLs.
How to Use
Download the code:
Click "Download ZIP" or clone the repository:

git clone https://github.com/10A0A/veworld-wallet-opener.git

Install the VeWorld extension from the Chrome Web Store.
Ensure the extension is enabled (chrome://extensions/).
Start a local web server (recommended):

python -m http.server 8000

Open the page in your browser:

http://localhost:8000/index.html

Click the "Open VeWorld Wallet" button.
If the wallet is installed, a pop-up should appear asking for connection confirmation.
Note : Opening the index.html file directly may not work in some browsers due to security restrictions.

Troubleshooting
Wallet doesn’t open?
Make sure the VeWorld extension is installed and enabled.
Open the browser console (F12 → Console) and check for errors.
Use a local web server instead of file://.
No response when clicking?
Ensure the file is loaded via http://localhost.
Limitations
May not work with local files (file://).
The wallet must support window.vechain or window.ethereum.
Customization
To use a specific DApp page, modify the openVeWorld function in index.html:

javascript

window.location.href = 'https://example-dapp.com'; // Replace with your DApp URL
License
This project is licensed under the MIT License.

That’s it! Enjoy using the VeWorld Wallet! 😊
