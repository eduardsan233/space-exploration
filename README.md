# space-exploration
space upp add subscriptions 
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Space Exploration</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #0a0a0a;
            color: white;
            text-align: center;
        }
        header {
            background: rgba(0, 0, 50, 0.8);
            padding: 20px;
            font-size: 24px;
            animation: fadeIn 2s ease-out;
        }
        .hero {
            background: url('https://source.unsplash.com/1600x900/?space') no-repeat center center/cover;
            height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 40px;
            font-weight: bold;
            opacity: 0;
            animation: fadeIn 3s ease-out forwards;
        }
        .content {
            padding: 40px;
            font-size: 20px;
            opacity: 0;
            animation: slideUp 2s ease-out forwards;
            animation-delay: 1s;
        }
        .footer {
            padding: 20px;
            background: rgba(0, 0, 50, 0.8);
            font-size: 16px;
            animation: fadeIn 2s ease-out forwards;
            animation-delay: 2s;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        @keyframes slideUp {
            from {
                transform: translateY(30px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <header>Space Exploration Agency</header>
    <div class="hero">Исследуем космос вместе!</div>
    <div class="content">
        <p>Мы разрабатываем инновационные технологии для исследования дальнего космоса.</p>
        <button onclick="alert('Добро пожаловать в космическое агентство!')">Узнать больше</button>
    </div>
    <div class="footer">&copy; 2025 Space Exploration Agency</div>

    <script>
        window.addEventListener('scroll', function() {
            const content = document.querySelector('.content');
            const hero = document.querySelector('.hero');
            
            if (window.scrollY > 100) {
                content.style.animation = 'slideUp 2s ease-out forwards';
                hero.style.opacity = 0.5;
            } else {
                content.style.animation = 'none';
                hero.style.opacity = 1;
            }
        });
    </script>
</body>
</html>
