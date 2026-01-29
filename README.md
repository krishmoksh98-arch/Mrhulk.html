<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>MR HULK</title>

<style>
body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: radial-gradient(circle at center, #0f1f0f, #000);
    font-family: 'Arial', sans-serif;
    color: white;
    overflow: hidden;
}

/* Container */
.container {
    text-align: center;
}

/* Question */
h1 {
    font-size: 3rem;
    animation: glowPulse 2s infinite;
}

/* Button */
button {
    padding: 15px 35px;
    font-size: 1.3rem;
    background: #0aff64;
    color: #000;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    font-weight: bold;
    box-shadow: 0 0 20px #0aff64;
    transition: transform 0.2s, box-shadow 0.2s;
}

button:hover {
    transform: scale(1.08);
    box-shadow: 0 0 35px #0aff64, 0 0 60px #0aff64;
}

/* Answer text */
.answer {
    display: none;
    font-size: 4rem;
    font-weight: 900;
    margin-top: 30px;
    color: #0aff64;
    animation: hulkGlow 1.5s infinite alternate;
}

/* Animations */
@keyframes glowPulse {
    0% {
        text-shadow: 0 0 10px #0aff64, 0 0 20px #0aff64;
    }
    50% {
        text-shadow: 0 0 25px #0aff64, 0 0 50px #0aff64;
    }
    100% {
        text-shadow: 0 0 10px #0aff64, 0 0 20px #0aff64;
    }
}

@keyframes hulkGlow {
    from {
        text-shadow: 0 0 20px #0aff64, 0 0 40px #0aff64;
        transform: scale(1);
    }
    to {
        text-shadow: 0 0 40px #0aff64, 0 0 80px #0aff64;
        transform: scale(1.08);
    }
}
</style>
</head>

<body>

<div class="container">
    <h1>Who is MR HULK??</h1>
    <button onclick="reveal()">REVEAL</button>
    <div class="answer" id="answer">ANUJ BHATT</div>
</div>

<script>
function reveal() {
    document.getElementById("answer").style.display = "block";
}
</script>

</body>
</html>
