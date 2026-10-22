Step 1: Install Visual Studio Code
Go to the official website: code.visualstudio.com.
Download and run the installer for your operating system (Windows, macOS, or Linux).
Follow the setup wizard prompts to finish the installation.
Step 2: Install Node.js (LTS Version)
Go to the official Node.js website: nodejs.org.
Download the LTS (Long Term Support) version installer.   
Node.js
Run the installer and complete the setup wizard (make sure to keep the option checked to add Node.js to your system PATH).
Step 3: Install VS Code Extensions
Open Visual Studio Code.
Click on the Extensions icon on the left sidebar (or press Ctrl+Shift+X / Cmd+Shift+X).
Search for and install:
Live Server (by Ritwick Dey)
Prettier - Code formatter (by Prettier)
Step 4 & 5: Create the Project Folder and Files
Open your terminal (or Command Prompt) or use VS Code (File > Open Folder) to create a folder named web-development-practice on your computer.
Inside this folder, create three files:
index.html
style.css
script.js
You can populate them with the following starter code:
index.html
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Development Environment Setup</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Hello, World!</h1>
        <p>My web development environment is successfully set up.</p>
        <button id="clickBtn">Click Me</button>
    </div>
    <script src="script.js"></script>
</body>
</html>
style.css
CSS
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.container {
    text-align: center;
    background: white;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

h1 {
    color: #333;
}

button {
    padding: 10px 20px;
    font-size: 16px;
    background-color: #007acc;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #005999;
}
script.js
JavaScript
document.getElementById('clickBtn').addEventListener('click', () => {
    alert('Environment setup verified successfully!');
});
Step 6: Run the HTML File Using Live Server
Open the web-development-practice folder inside VS Code.
Open the index.html file.
Click on the "Go Live" button at the bottom right corner of the VS Code status bar.
Your default browser will automatically open and display the web page at [http://127.0.0.1:5500](http://127.0.0.1:5500).
Step 7: Verify Node.js and npm Installation
Open your terminal (or open the integrated terminal in VS Code via Ctrl + ~ or Cmd + ~).
Run the following commands to check the versions:
Bash
node -v
npm -v
Verify that version numbers are printed out successfully in the terminal.