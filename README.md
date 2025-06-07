<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="description" content="Free educational tutorials and resources by Brainify" />
    <meta name="keywords" content="education, tutorials, YouTube, study guides" />
    <title>SparkForScholars - Learn with Us</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            line-height: 1.6;
            color: #333;
        }
        header {
            background: #1e90ff;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        header h1 {
            margin-bottom: 0.5rem;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1rem;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        section {
            padding: 2rem 0;
            border-bottom: 1px solid #ddd;
        }
        .hero {
            text-align: center;
        }
        .hero iframe {
            max-width: 100%;
        }
        .btn {
            display: inline-block;
            padding: 0.5rem 1rem;
            background: #28a745;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 1rem;
        }
        .btn:hover {
            background: #218838;
        }
        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 1rem;
        }
        .video-grid div {
            text-align: center;
        }
        .resource-list {
            list-style: none;
            margin: 1rem 0;
        }
        .resource-list li {
            margin: 0.5rem 0;
        }
        .resource-list a {
            color: #1e90ff;
            text-decoration: none;
        }
        .resource-list a:hover {
            text-decoration: underline;
        }
        .blog-post {
            margin: 1rem 0;
            padding: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
        }
        .blog-post h3 {
            margin-bottom: 0.5rem;
        }
        .blog-content {
            max-height: 4rem;
            overflow: hidden;
            transition: max-height 0.3s ease;
        }
        .blog-content.expanded {
            max-height: none;
        }
        form {
            max-width: 500px;
            margin: 1rem 0;
        }
        form label {
            display: block;
            margin: 0.5rem 0;
        }
        form input, form textarea {
            width: 100%;
            padding: 0.5rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        form button {
            padding: 0.5rem 1rem;
            background: #1e90ff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        form button:hover {
            background: #0066cc;
        }
        footer {
            background: #f4f4f4;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }
        @media (max-width: 600px) {
            nav a {
                display: block;
                margin: 0.5rem 0;
            }
            .hero iframe {
                width: 100%;
                height: auto;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Brainify - Learn with Us</h1>
        <nav>
            <a href="#hero">Home</a>
            <a href="#videos">Videos</a>
            <a href="#resources">Resources</a>
            <a href="#blog">Blog</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section id="hero" class="hero">
            <h2>Welcome to Brainify</h2>
            <p>Explore free tutorials and resources to help you excel in your studies.</p>
           <video width="560" height="315" controls>
  <source src="Brainify  Empowering Your AI Learning Journey_free.mp4" type="video/mp4" />
  Your browser does not support the video tag.
</video>

        </section>

        <section id="videos">
            <h2>Featured Videos</h2>
            <div class="video-grid">
                <div>
                    <iframe width="300" height="169" src="https://www.youtube.com/embed/tgbNymZ7vqY" title="Video 1" frameborder="0" allowfullscreen></iframe>
                    <p>Math Basics</p>
                </div>
                <div>
                    <iframe width="300" height="169" src="https://www.youtube.com/embed/9bZkp7q19f0" title="Video 2" frameborder="0" allowfullscreen></iframe>
                    <p>Science Explainers</p>
                </div>
                <div>
                    <iframe width="300" height="169" src="https://www.youtube.com/embed/e-ORhEE9VVg" title="Video 3" frameborder="0" allowfullscreen></iframe>
                    <p>Programming Tutorials</p>
                </div>
            </div>
        </section>

       <section id="resources">
    <h2>Study Resources</h2>
    <ul class="resource-list">
        <li><a href="files/math-formulas.pdf" download>Download 3nd SEM SYllabus</a></li>
        <li><a href="files/science-notes.pdf" download>Science Revision Notes</a></li>
        <li><a href="beginners_python_cheat_sheet_pcc_all.pdf" download>Python Programming Cheat Sheet</a></li>
    </ul>
</section>


        <section id="blog">
            <h2>Latest Blog Posts</h2>
            <div class="blog-post">
                <h3>How to Study Smarter, Not Harder</h3>
                <div class="blog-content">
                    <p>Most students think studying more equals better grades. But what if we told you it’s about technique, not time?</p>
                </div>
            </div>
            <div class="blog-post">
                <h3>Top 5 YouTube Channels for Learning</h3>
                <div class="blog-content">
                    <p>Discover the best YouTube channels that provide high-quality educational content for free.</p>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>Contact Us</h2>
            <form>
                <label for="name">Name</label>
                <input type="text" id="name" name="name" required />

                <label for="email">Email</label>
                <input type="email" id="email" name="email" required />

                <label for="message">Message</label>
                <textarea id="message" name="message" rows="4" required></textarea>

                <button type="submit">Send</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Brainify. All rights reserved.</p>
    </footer>

    <script>
        document.querySelectorAll('.blog-post').forEach(post => {
            post.addEventListener('click', () => {
                const content = post.querySelector('.blog-content');
                content.classList.toggle('expanded');
            });
        });
    </script>
</body>
</html>
