<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <title>Uknown error, please try again later</title>
</head>
<body>
    <h1>404</h1>
    <p>Uknown error..</p>
    <h2>We working on it, try again later</h2>
    <h2>Current time:</h2>
<p id="clock"></p>

<script>
function updateClock() {
    const now = new Date();

    const time = now.toLocaleTimeString('uk-UA');

    document.getElementById('clock').textContent =
        time;
}

updateClock();
setInterval(updateClock, 1000);
</script>
<p onclick="location.reload()" style="cursor: pointer;">
    Натисни на мене
</p>
</body>
</html>
