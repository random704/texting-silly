<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chat Application</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="login-container">
        <h2>Create Account</h2>
        <input type="text" id="username" placeholder="Enter username">
        <input type="password" id="password" placeholder="Enter password">
        <button onclick="createAccount()">Create Account</button>
    </div>

    <div id="chat-container" style="display: none;">
        <h2>Welcome <span id="loggedInUser"></span></h2>
        <div id="chatMessages"></div>
        <textarea id="messageInput" placeholder="Type your message..."></textarea>
        <button onclick="sendMessage()">Send</button>
    </div>

    <div id="user-count">
        <p>Users online: <span id="userCountDisplay">0</span></p>
    </div>

    <script>
        function createAccount() {
            let username = document.getElementById('username').value.trim();
            let password = document.getElementById('password').value.trim();

            // Check if username or password is empty
            if (!username || !password) {
                alert('Username and password are required!');
                return;
            }

            // Store username in local storage
            localStorage.setItem('username', username);

            // Update user count
            let userCount = parseInt(localStorage.getItem('userCount') || 0);
            userCount++;
            localStorage.setItem('userCount', userCount);
            document.getElementById('userCountDisplay').innerText = userCount;

            // Hide login container and show chat container
            document.getElementById('login-container').style.display = 'none';
            document.getElementById('chat-container').style.display = 'block';

            // Display logged in user's name
            document.getElementById('loggedInUser').innerText = username;

            // Load chat history
            loadChatHistory();
        }

        function sendMessage() {
            let message = document.getElementById('messageInput').value.trim();
            let chatMessages = document.getElementById('chatMessages');

            if (!message) {
                alert('Please enter a message.');
                return;
            }

            // Append message to chat
            let username = localStorage.getItem('username');
            let messageElement = document.createElement('div');
            messageElement.className = 'message';
            messageElement.innerHTML = `<strong>${username}:</strong> ${message}`;
            chatMessages.appendChild(messageElement);

            // Save message to local storage
            let messages = JSON.parse(localStorage.getItem('messages')) || [];
            messages.push({ username: username, message: message });
            localStorage.setItem('messages', JSON.stringify(messages));

            // Clear message input
            document.getElementById('messageInput').value = '';
        }

        function loadChatHistory() {
            let messages = JSON.parse(localStorage.getItem('messages')) || [];
            let chatMessages = document.getElementById('chatMessages');
            chatMessages.innerHTML = '';

            messages.forEach(function(msg) {
                let messageElement = document.createElement('div');
                messageElement.className = 'message';
                messageElement.innerHTML = `<strong>${msg.username}:</strong> ${msg.message}`;
                chatMessages.appendChild(messageElement);
            });
        }

        // Update user count display on page load
        window.onload = function() {
            let userCount = parseInt(localStorage.getItem('userCount') || 0);
            document.getElementById('userCountDisplay').innerText = userCount;
        };
    </script>
</body>
</html>
