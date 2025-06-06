<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background: #f5f5f5;
        }

        header {
            background: #333;
            color: white;
            padding: 15px;
        }

        nav ul {
            list-style: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 10px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
        }

        section {
            padding: 50px;
        }

        .project {
            display: inline-block;
            margin: 20px;
        }

        .project img {
            width: 300px;
            height: auto;
            border-radius: 10px;
        }

        footer {
            background: #333;
            color: white;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <h1>My Portfolio</h1>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Me</h2>
        <p>Welcome to my portfolio! I am a creative developer passionate about design and coding.</p>
    </section>

    <section id="projects">
        <h2>Projects</h2>
        <div class="project">
            <img src="images/project1.jpg" alt="Project 1">
            <p>Project 1 - Amazing website built with HTML, CSS, JS.</p>
        </div>
        <div class="project">
            <img src="images/project2.jpg" alt="Project 2">
            <p>Project 2 - An awesome design experiment.</p>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <p>Email: example@email.com</p>
    </section>

    <footer>
        <p>&copy; 2025 My Portfolio</p>
    </footer>

    <script>
        document.querySelectorAll('nav ul li a').forEach(link => {
            link.addEventListener('click', event => {
                event.preventDefault();
                document.querySelector(link.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
            });
        });
    </script>
</body>
</html>
