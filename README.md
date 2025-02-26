# Codsoft_taskno1
Creating a personal portfolio using CSS and HTML is a popular beginner web development  project.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(45deg, #ff7eb3, #ff758c, #ff7eb3);
            text-align: center;
            color: white;
        }
        header {
            padding: 20px;
            font-size: 24px;
            font-weight: bold;
        }
        .hero {
            padding: 50px 20px;
            animation: fadeIn 2s ease-in-out;
        }
        .name {
            color: yellow;
            font-weight: bold;
        }
        .portfolio {
            padding: 40px 20px;
        }
        .gallery {
            display: flex;
            justify-content: center;
            gap: 15px;
        }
        .qw{
            justify-content: center;

        }
        .item {
            background: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 10px;
            transition: transform 0.3s ease-in-out;
        }
        .item:hover {
            transform: scale(1.1);
        }
        @keyframes fadeIn {
            from { opacity: -10; }
            to { opacity: 5; }
        }
        q{
            background-color: black;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Portfolio</h1>
        <p>"Crafting seamless, stunning, and scalable web experiences."</p>
    </header>
    <section class="hero">
        <h2>Hello, I'm <span class="name">Your Mohammed suhail M</span></h2>
        <p>Web Developer | Designer | Freelancer</p>
    </section>
    <img src="e2.jpeg" alt="">
    <div class="qw">
        <p> Passionate web developer with a keen eye for design and functionality. Specializing in creating responsive, user-friendly websites and web applications that enhance user experience and drive results.   
            - Proficient in HTML, CSS, JavaScript, and modern frameworks like React and Vue.js.  
            - Experienced in back-end technologies such as Node.js, Express, and databases like MongoDB and MySQL.  
            - Skilled in UI/UX design principles, ensuring visually appealing and intuitive interfaces.  
            - Strong understanding of performance optimization, SEO, and cross-browser compatibility.  
            - Successfully delivered projects ranging from personal portfolios to complex enterprise applications.</p>
    </div>
    <section class="portfolio">
        <h2>My Work</h2>
        <div class="gallery">
            <div class="item">Project 1</div>
            <div class="item">Project 2</div>
            <div class="item">Project 3</div>
        </div>
    </section>
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const items = document.querySelectorAll(".item");
            items.forEach(item => {
                item.addEventListener("mouseenter", () => {
                    item.style.backgroundColor = "rgba(255, 255, 255, 0.5)";
                });
                item.addEventListener("mouseleave", () => {
                    item.style.backgroundColor = "rgba(255, 255, 255, 0.2)";
                });
            });
        });
    </script>
    <div class="q">
        <p>© 2025</p>
    </div>
</body>
</html>
