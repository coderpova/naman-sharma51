# naman-sharma51
this is my 8th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhatsApp Video Chat UI</title>
    <style>
        :root {
            --wa-green: #075E54;
            --wa-light-green: #25D366;
            --wa-chat-bg: #e5ddd5;
            --wa-incoming: #ffffff;
            --wa-outgoing: #dcf8c6;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #d1d1d1;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        /* Container */
        .chat-container {
            width: 100%;
            max-width: 400px;
            height: 600px;
            background-color: var(--wa-chat-bg);
            display: flex;
            flex-direction: column;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            border-radius: 10px;
            overflow: hidden;
        }

        /* Header */
        .header {
            background-color: var(--wa-green);
            color: white;
            padding: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .back-arrow { font-size: 20px; cursor: pointer; }
        .avatar { width: 35px; height: 35px; background: #ccc; border-radius: 50%; }
        .user-info { flex: 1; }
        .user-info div { font-weight: bold; font-size: 16px; }
        .user-info span { font-size: 12px; opacity: 0.8; }

        /* Chat Area */
        .message-area {
            flex: 1;
            padding: 20px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        /* General Bubble Styles */
        .bubble {
            max-width: 85%;
            padding: 8px 10px;
            border-radius: 8px;
            position: relative;
            font-size: 14px;
            box-shadow: 0 1px 1px rgba(0,0,0,0.1);
        }

        /* Video Bubble (Outgoing) */
        .outgoing {
            align-self: flex-end;
            background-color: var(--wa-outgoing);
        }

        .video-wrapper {
            width: 100%;
            border-radius: 5px;
            overflow: hidden;
            margin-bottom: 5px;
        }

        .video-wrapper iframe {
            width: 100%;
            aspect-ratio: 16/9;
            border: none;
            display: block;
        }

        .timestamp {
            font-size: 10px;
            color: #666;
            text-align: right;
            display: block;
        }

        /* Footer / Input */
        .footer {
            padding: 10px;
            background: #f0f0f0;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .input-box {
            flex: 1;
            background: white;
            padding: 10px 15px;
            border-radius: 20px;
            font-size: 14px;
            color: #999;
        }

        .mic-btn {
            background: var(--wa-green);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    </style>
</head>
<body>

    <div class="chat-container">
        <div class="header">
            <span class="back-arrow">←</span>
            <div class="avatar"></div>
            <div class="user-info">
                <div>ABES Study Group</div>
                <span>online</span>
            </div>
        </div>

        <div class="message-area">
            
            <div class="bubble outgoing">
                <div class="video-wrapper">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0" title="Video message"></iframe>
                </div>
                Check out this logic for the Monostable Multivibrator! 📚
                <span class="timestamp">08:50 AM ✓✓</span>
            </div>

        </div>

        <div class="footer">
            <div class="input-box">Type a message</div>
            <div class="mic-btn">🎤</div>
        </div>
    </div>

</body>
</html>
