<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Karthick B - Portfolio</title>
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            background-color: #00FFFF; /* Changed to Cyan */
            color: black;
            text-align: center;
        }

       
        .banner {
            background: url('31632aa5f671c9c7045d341526e5decf.jpg') no-repeat center center/cover;
            height: 250px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .name {
            background: rgba(0, 0, 0, 0.6);
            padding: 10px 20px;
            border-radius: 10px;
            font-size: 2.5rem;
            font-weight: bold;
            color: white;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }

        /* Navigation */
        header {
            background: #333;
            padding: 15px;
            display: flex;
            justify-content: center;
        }
        nav ul {
            list-style: none;
            display: flex;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
        }

        /* Hero Section */
        .hero {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .hero h1 span {
            color: #ff7b00;
        }
        .btn {
            background: #ff4800;
            padding: 10px 20px;
            text-decoration: none;
            color: white;
            border-radius: 5px;
            margin-top: 15px;
        }

        /* Skills Section */
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .skill {
            background: #ffe600;
            padding: 10px 15px;
            margin: 5px;
            border-radius: 5px;
        }

        /* Projects Section */
        .projects-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        .project-card {
            background: #222;
            margin: 15px;
            padding: 15px;
            border-radius: 10px;
            width: 300px;
            color: white;
        }

        /* Contact Section */
        form {
            display: flex;
            flex-direction: column;
            width: 50%;
            margin: auto;
        }
        form input, form textarea {
            margin: 10px 0;
            padding: 10px;
            border: none;
            border-radius: 5px;
        }
        form button {
            background: #88ff00;
            padding: 10px;
            border: none;
            color: white;
            cursor: pointer;
            border-radius: 5px;
        }

        /* Footer */
        footer {
            background: #333;
            padding: 15px;
            margin-top: 20px;
            color: white;
        }
    </style>
</head>
<body>

    <!-- Banner Section -->
    <div class="banner">
        <h1 class="name">Karthick B</h1>
    </div>

    <!-- Navigation -->
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Hi, I'm <span>Karthick B</span></h1>
        <p>A passionate Developer specialized in Web & Software Development.</p>
        <a href="#contact" class="btn">Hire Me</a>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>I am a **BCA graduate** with expertise in **HTML, CSS, JavaScript, Java, Python, C++, DSA, and SQL**. I love solving real-world problems through code and building interactive web applications.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2>Skills</h2>
        <div class="skills-container">
            <div class="skill">HTML</div>
            <div class="skill">CSS</div>
            <div class="skill">JavaScript</div>
            <div class="skill">Java</div>
            <div class="skill">Python</div>
            <div class="skill">C++</div>
            <div class="skill">DSA</div>
            <div class="skill">SQL</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Projects</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>Portfolio Website</h3>
                <p>A fully responsive personal portfolio website.</p>
            </div>
            <div class="project-card">
                <h3>To-Do App</h3>
                <p>A JavaScript-powered To-Do list application with a database.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>© 2025 Karthick B. All Rights Reserved.</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const scrollLinks = document.querySelectorAll("nav ul li a");
            scrollLinks.forEach(link => {
                link.addEventListener("click", e => {
                    e.preventDefault();
                    const targetId = link.getAttribute("href").substring(1);
                    document.getElementById(targetId).scrollIntoView({ behavior: "smooth" });
                });
            });
        });
    </script>

</body>
</html>
