
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coupon Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Coupon Website</h1>
    </header>
    <main>
        <section class="coupon">
            <h2>Coupon Title</h2>
            <p>Description of the coupon.</p>
            <button onclick="showCode('code1')">Show Code</button>
            <p id="code1" class="coupon-code">SAVE10</p>
        </section>
        <section class="coupon">
            <h2>Coupon Title</h2>
            <p>Description of the coupon.</p>
            <button onclick="showCode('code2')">Show Code</button>
            <p id="code2" class="coupon-code">DISCOUNT20</p>
        </section>
    </main>
    <script src="scripts.js"></script>
</body>
</html>body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1rem;
    text-align: center;
}

main {
    padding: 2rem;
}

.coupon {
    background-color: #fff;
    border: 1px solid #ddd;
    padding: 1rem;
    margin: 1rem 0;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.coupon h2 {
    margin: 0 0 0.5rem;
}

.coupon-code {
    display: none;
    font-weight: bold;
    color: #d9534f;
    margin-top: 0.5rem;
}function showCode(id) {
    var codeElement = document.getElementById(id);
    codeElement.style.display = codeElement.style.display === 'none' ? 'block' : 'none';
}