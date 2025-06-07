<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="description" content="Free educational tutorials and resources by SparkForScholars" />
    <meta name="keywords" content="education, tutorials, YouTube, study guides" />
    <title>SparkForScholars - Ignite Your Learning</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        body {
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            scroll-behavior: smooth;
        }
        header {
            background: linear-gradient(90deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 2rem 1rem;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
            animation: fadeInDown 1s ease-in-out;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1.5rem;
            font-weight: 600;
            transition: color 0.3s ease, transform 0.3s ease;
        }
        nav a:hover {
            color: #ffd700;
            transform: scale(1.1);
        }
        main {
            max-width: 1300px;
            margin: 0 auto;
            padding: 3rem 1rem;
        }
        section {
            margin: 2rem 0;
            padding: 3rem;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        section:hover {
            transform: translateY(-5px);
        }
        .hero {
            background: url('https://source.unsplash.com/random/1200x400/?education') no-repeat center/cover;
            color: white;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        .hero h2::before {
            content: '\f19d'; /* Graduation cap icon */
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            margin-right: 0.5rem;
        }
        .videos {
            background: linear-gradient(135deg, #fff3e0 0%, #ffe0b2 100%);
        }
        .videos h2::before {
            content: '\f03d'; /* Video icon */
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            margin-right: 0.5rem;
        }
        .resources {
            background: linear-gradient(135deg, #e0f7fa 0%, #b2ebf2 100%);
        }
        .resources h2::before {
            content: '\f15c'; /* File icon */
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            margin-right: 0.5rem;
        }
        .blog {
            background: linear-gradient(135deg, #fce4ec 0%, #f8bbd0 100%);
        }
        .blog h2::before {
            content: '\f303'; /* Pen icon */
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            margin-right: 0.5rem;
        }
        .contact {
            background: linear-gradient(135deg, #f3e5f5 0%, #e1bee7 100%);
        }
        .contact h2::before {
            content: '\f0e0'; /* Envelope icon */
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            margin-right: 0.5rem;
        }
        .hero h2, .videos h2, .resources h2, .blog h2, .contact h2 {
            font-size: 2.2rem;
            margin-bottom: 1rem;
            color: #6a11cb;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        .hero video {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        .hero video:hover {
            transform: scale(1.02);
        }
        .btn {
            display: inline-block;
            padding: 0.75rem 1.5rem;
            background: #ff6f61;
            color: white;
            text-decoration: none;
            border-radius: 50px;
            margin-top: 1.5rem;
            font-weight: 600;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        .btn:hover {
            background: #e65b50;
            transform: translateY(-2px);
        }
        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        .video-grid div {
            text-align: center;
            background: white;
            padding: 1rem;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .video-grid div:hover {
            transform: translateY(-5px);
        }
        .video-grid iframe {
            border-radius: 10px;
            width: 100%;
            height: 200px;
        }
        .resource-list {
            list-style: none;
            margin: 1.5rem 0;
            padding: 1rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .resource-list li {
            margin: 0.75rem 0;
        }
        .resource-list a {
            color: #6a11cb;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }
        .resource-list a:hover {
            color: #ffd700;
        }
        .blog-post {
            margin: 1.5rem 0;
            padding: 1.5rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            cursor: pointer;
            transition: box-shadow 0.3s ease;
        }
        .blog-post:hover {
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
        }
        .blog-post h3 {
            color: #6a11cb;
            margin-bottom: 0.75rem;
        }
        .blog-content {
            max-height: 5rem;
            overflow: hidden;
            transition: max-height 0.5s ease;
        }
        .blog-content.expanded {
            max-height: none;
        }
        form {
            max-width: 600px;
            margin: 2rem auto;
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        form label {
            display: block;
            margin: 0.75rem 0;
            font-weight: 600;
            color: #6a11cb;
        }
        form input, form textarea {
            width: 100%;
            padding: 0.75rem;
            margin-bottom: 1.5rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            transition: border-color 0.3s ease;
        }
        form input:focus, form textarea:focus {
            border-color: #6a11cb;
            outline: none;
        }
        form button {
            padding: 0.75rem 2rem;
            background: #6a11cb;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        form button:hover {
            background: #510c99;
            transform: translateY(-2px);
        }
        footer {
            background: linear-gradient(90deg, #2575fc 0%, #6a11cb 100%);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }
        footer p {
            font-size: 1.1rem;
        }
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @media (max-width: 600px) {
            header h1 {
                font-size: 1.8rem;
            }
            nav a {
                display: block;
                margin: 0.75rem 0;
            }
            section {
                padding: 2rem 1rem;
            }
            .video-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
    <script>
        document.querySelectorAll('.blog-post').forEach(post => {
            post.addEventListener('click', () => {
                const content = post.querySelector('.blog-content');
                content.classList.toggle('expanded');
            });
        });
    </script>
</head>
<body>
    <header>
        <h1>Justbrainify - Ignite Your Learning</h1>
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
            <h2>Welcome to Justbrainify</h2>
            <p>Unleash your potential with our free tutorials and resources!</p>
            <video width="600" height="340" controls>
                <source src="Brainify  Empowering Your AI Learning Journey_free.mp4" type="video/mp4" />
                Your browser does not support the video tag.
            </video>
            <a href="#videos" class="btn">Explore Tutorials</a>
        </section>

        <section id="videos" class="videos">
            <h2>Featured Tutorials</h2>
            <div class="video-grid">
                <div>
                    <iframe src="https://www.youtube.com/embed/tgbNymZ7vqY" title="Math Basics" frameborder="0" allowfullscreen></iframe>
                    <p>Master Math Basics</p>
                </div>
                <div>
                    <iframe src="https://www.youtube.com/embed/9bZkp7q19f0" title="Science Explainers" frameborder="0" allowfullscreen></iframe>
                    <p>Discover Science</p>
                </div>
                <div>
                    <iframe src="https://www.youtube.com/embed/e-ORhEE9VVg" title="Programming Tutorials" frameborder="0" allowfullscreen></iframe>
                    <p>Code Like a Pro</p>
                </div>
            </div>
        </section>

        <section id="resources" class="resources">
            <h2>Study Resources</h2>
            <ul class="resource-list">
                <li><a href="math-formulas.pdf" download>3rd SEM Syllabus</a></li>
                <li><a href="science-notes.pdf" download>Science Revision Notes</a></li>
                <li><a href="beginners_python_cheat_sheet_pcc_all.pdf" download>Python Cheat Sheet</a></li>
            </ul>
        </section>

        <section id="blog" class="blog">
            <h2>Latest Insights</h2>
            <div class="blog-post">
                <h3>Study Smarter, Not Harder</h3>
                <div class="blog-content">
                    <p>Discover techniques to maximize your study efficiency and achieve better results in less time.</p>
                </div>
            </div>
            <div class="blog-post">
                <h3>Why Curiosity Fuels Success</h3>
                <div class="blog-content">
                    <p>Learn how a curious mindset can transform your learning journey and open new opportunities.</p>
                </div>
            </div>
        </section>

        <section id="contact" class="contact">
            <h2>Get in Touch</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required />

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required />

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="6" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </section>
    </main>

    <footer>
        <p>© 2025 Justbrainify. Igniting Minds, One Lesson at a Time.</p>
    </footer>
</body>
</html>
