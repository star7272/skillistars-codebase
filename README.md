<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SKILLISTAR CODEBASE - Neon Learning Code Portal</title>

<style>
    /* ---------- GLOBAL STYLES ---------- */
    body, html {
        margin: 0;
        padding: 0;
        font-family: 'Poppins', sans-serif;
        background: #01010a;
        color: #fff;
        overflow-x: hidden;
    }

    /* ---------- CUSTOM ANIMATED BACKGROUND ---------- */
    body::before {
        content: '';
        position: fixed;
        top: 0; left: 0;
        width: 100%; height: 100%;
        background: linear-gradient(270deg, #0ff, #ff00ff, #00ff00, #ff0);
        background-size: 800% 800%;
        animation: gradientBG 20s ease infinite;
        z-index: -2;
    }

    @keyframes gradientBG {
        0% {background-position:0% 50%}
        50% {background-position:100% 50%}
        100% {background-position:0% 50%}
    }

    /* ---------- NEON TITLE ---------- */
    h1 {
        font-size: 48px;
        color: #0ff;
        text-shadow: 0 0 10px #0ff, 0 0 20px #0ff, 0 0 40px #0ff;
        white-space: nowrap;
        position: relative;
        display: inline-block;
        animation: moveTitle 10s linear infinite, glow 2s ease-in-out infinite alternate;
        margin: 50px 0;
    }

    @keyframes moveTitle {
        0% { transform: translateX(-100%); }
        50% { transform: translateX(50%); }
        100% { transform: translateX(-100%); }
    }

    @keyframes glow {
        0% { text-shadow: 0 0 10px #0ff, 0 0 20px #0ff, 0 0 30px #ff00ff; }
        50% { text-shadow: 0 0 25px #ff0, 0 0 50px #ff0, 0 0 70px #ff00ff; }
        100% { text-shadow: 0 0 10px #0ff, 0 0 20px #0ff, 0 0 30px #ff00ff; }
    }

    /* ---------- MAIN NEON LINKS ---------- */
    .links a {
        display: inline-block;
        margin: 12px;
        padding: 12px 28px;
        border-radius: 12px;
        color: #0ff;
        border: 2px solid #0ff;
        text-decoration: none;
        font-size: 20px;
        font-weight: 600;
        text-shadow: 0 0 5px #0ff;
        box-shadow: 0 0 10px #0ff;
        transition: 0.3s;
    }

    .links a:hover {
        color: #ff0;
        box-shadow: 0 0 20px #ff0, 0 0 40px #ff00ff;
        transform: scale(1.1);
    }

    /* ---------- CONTACT BOX ---------- */
    .contact-box {
        margin: 50px auto;
        padding: 25px;
        max-width: 450px;
        border-radius: 14px;
        border: 2px solid #0ff;
        background: rgba(0,0,0,0.4);
        box-shadow: 0 0 20px #0ff;
    }

    .contact-box h2 {
        color: #ff00ff;
        text-shadow: 0 0 10px #ff00ff;
    }

    .contact-box p {
        font-size: 18px;
        line-height: 1.6;
        color: #cfefff;
    }

    .contact-box a {
        color: #0ff;
        font-weight: bold;
        text-decoration: none;
        text-shadow: 0 0 5px #0ff;
    }

    /* ---------- SIDEBAR QUICK ACTION ---------- */
    #quickActionsToggle {
        position: fixed;
        bottom: 20px;
        right: 20px;
        background: #000;
        border: 2px solid #0ff;
        cursor: pointer;
        border-radius: 50px;
        padding: 12px 20px;
        color: #0ff;
        font-size: 18px;
        box-shadow: 0 0 12px #0ff;
        z-index: 999;
    }

    #quickActions {
        display: none;
        position: fixed;
        right: 20px;
        bottom: 80px;
        background: rgba(0, 0, 0, 0.9);
        width: 200px;
        padding: 15px;
        border-radius: 14px;
        border: 2px solid #0ff;
        box-shadow: 0 0 15px #0ff;
    }

    #quickActions a {
        display: block;
        margin: 8px 0;
        font-size: 16px;
        color: #0ff;
        text-decoration: none;
        text-shadow: 0 0 5px #0ff;
    }

    #quickActions a:hover {
        color: #ff0;
        text-shadow: 0 0 10px #ff0, 0 0 20px #ff00ff;
    }

    /* ---------- NEON FOOTER ---------- */
    footer {
        margin-top: 80px;
        padding: 20px 10px;
        background: #000;
        color: #0ff;
        text-shadow: 0 0 5px #0ff;
        border-top: 2px solid #0ff;
        box-shadow: 0 0 15px #0ff inset;
        font-size: 16px;
    }

    footer a {
        color: #ff0;
        text-decoration: none;
        text-shadow: 0 0 5px #ff0;
    }
</style>
</head>
<body>

<!-- NEON TITLE -->
<h1>SKILLISTAR CODEBASE - Neon Learning Code Portal</h1>

<!-- NEON LINKS -->
<div class="links">
    <a href="about.html" target="_blank">About Us</a>
    <a href="privacy.html" target="_blank">Privacy Policy</a>
    <a href="terms.html" target="_blank">Terms & Conditions</a>
    <a href="lessons.html" target="_blank">Lessons</a>
</div>

<!-- CONTACT ME SECTION -->
<div class="contact-box">
    <h2>📞 Contact Me</h2>
    <p>For support, inquiries, or updates:</p>
    <p><strong>WhatsApp:</strong> <a href="https://wa.me/254738017513" target="_blank">Chat Now</a></p>
    <p><strong>Email:</strong> skillistars@gmail.com</p>
</div>

<!-- QUICK ACTION SIDEBAR -->
<button id="quickActionsToggle">⚡ Quick Actions</button>
<div id="quickActions">
    <a href="about.html" target="_blank">About</a>
    <a href="privacy.html" target="_blank">Privacy</a>
    <a href="terms.html" target="_blank">Terms</a>
    <a href="lessons.html" target="_blank">Lessons</a>
    <a href="https://wa.me/254738017513" target="_blank">Contact</a>
</div>

<!-- FOOTER -->
<footer>
    © 2025 SKILLISTAR CODEBASE — All rights reserved | 
    <a href="privacy.html">Privacy</a> · <a href="terms.html">Terms</a>
</footer>

<script>
    // Quick Actions toggle
    const toggleBtn = document.getElementById('quickActionsToggle');
    const quickPanel = document.getElementById('quickActions');

    toggleBtn.addEventListener('click', () => {
        quickPanel.style.display = quickPanel.style.display === 'block' ? 'none' : 'block';
    });
</script>

</body>
</html>
