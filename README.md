# sasha-smirnov.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Открытие бота...</title>
    <script>
        // Получаем параметры из URL
        const urlParams = new URLSearchParams(window.location.search);
        const startParam = urlParams.get('start') || 'default_start';

        // Формируем ссылку на бота с параметром
        const botUrl = https://t.me/StableGrowzBot?start=${encodeURIComponent(startParam)};

        // Ждём 1 секунду и делаем редирект (для iOS)
        setTimeout(() => {
            window.location.href = botUrl;
        }, 1000);
    </script>
</head>
<body>
    <p>Если бот не открылся автоматически, <a id="botLink" href="#">нажмите здесь</a>.</p>
    <script>
        document.getElementById('botLink').href = botUrl;
    </script>
</body>
</html>
