
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unknown error, please try again later</title>
</head>
<body>
    <h1>-170</h1>
    <p>An unknown error has occurred.</p>
    <h2>We're working on it. Try again later.</h2>
    <p>Error code: -170</p>

    <br><br>

    <h2>Current time:</h2>
    <p id="clock">Loading...</p>

    <script>
        function updateClock() {
            const now = new Date();

            const time = now.toLocaleTimeString('uk-UA', {
                hour: '2-digit',
                minute: '2-digit',
                second: '2-digit',
                hour12: false
            });

            document.getElementById('clock').textContent = time;
        }

        updateClock();
        setInterval(updateClock, 1000);
    </script>

    <br><br>

    <p onclick="location.reload()"
       style="cursor: pointer; text-decoration: underline;">
        Click here to reload.
    </p>
</body>
</html>
```
