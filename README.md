<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anay's Website</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .welcome-banner {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: linear-gradient(90deg, #ff7eb3, #ff758c);
            color: white;
            text-align: center;
            padding: 15px 0;
            font-size: 1.5rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            animation: slideDown 1s ease-out;
        }
        @keyframes slideDown {
            from {
                transform: translateY(-100%);
            }
            to {
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="welcome-banner">
        Hello Gamers! Welcome to my Website Hope you enjoy!
    </div>
    <script>
        // Optional: Add a fade-out effect after 5 seconds
        setTimeout(() => {
            const banner = document.querySelector('.welcome-banner');
            banner.style.transition = 'opacity 1s';
            banner.style.opacity = '0';
            setTimeout(() => banner.remove(), 1000); // Remove the banner after fade-out
        }, 5000);
    </script>
</body>
</html>
