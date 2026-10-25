1. Aim

The aim of this assignment is to convert a div-based webpage into a semantic HTML webpage and improve its accessibility, readability, and structure.

2. Objective

To use semantic HTML elements.

To organize navigation links inside the <nav> element.

To place the main content inside the <main> element.

To maintain a proper heading hierarchy.

To add meaningful alternative text to images.

To make links and webpage sections understandable.

3. Complete HTML Code

File Name: index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic HTML and Accessibility</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f7fb;
            color: #222;
        }

        header {
            background-color: #173b67;
            color: white;
            text-align: center;
            padding: 25px;
        }

        nav {
            background-color: #24558a;
            padding: 15px;
            text-align: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 12px;
            font-weight: bold;
        }

        nav a:hover,
        nav a:focus {
            text-decoration: underline;
        }

        main {
            max-width: 1000px;
            margin: 25px auto;
            padding: 20px;
        }

        section,
        article,
        aside {
            background-color: white;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
        }

        h2 {
            color: #173b67;
        }

        img {
            display: block;
            max-width: 100%;
            height: auto;
            margin: 15px auto;
            border-radius: 8px;
        }

        a {
            color: #0645ad;
        }

        nav a {
            color: white;
        }

        a:focus {
            outline: 3px solid orange;
            outline-offset: 3px;
        }

        footer {
            background-color: #173b67;
            color: white;
            text-align: center;
            padding: 20px;
        }

        footer a {
            color: white;
        }

        @media (max-width: 600px) {
            nav a {
                display: inline-block;
                margin: 6px;
            }

            main {
                padding: 10px;
            }
        }
    </style>
</head>

<body>

    <!-- Header -->
    <header>
        <h1>Welcome to My College Website</h1>
        <p>Learning, Innovation and Excellence</p>
    </header>

    <!-- Navigation -->
    <nav aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#courses">Courses</a>
        <a href="#technology">Technology</a>
        <a href="#contact">Contact</a>
    </nav>

    <!-- Main Content -->
    <main>

        <!-- Home Section -->
        <section id="home" aria-labelledby="home-heading">
            <h2 id="home-heading">Home</h2>

            <p>
                Welcome to my college website. This webpage provides
                information about college education, courses,
                technology and student development.
            </p>

            <img
                src="https://placehold.co/600x250/173b67/ffffff?text=College+Education"
                alt="Illustration representing college education and learning"
                width="600"
                height="250"
            >
        </section>

        <!-- About Section -->
        <section id="about" aria-labelledby="about-heading">
            <h2 id="about-heading">About My College</h2>

            <p>
                My college provides students with opportunities to gain
                knowledge, develop practical skills and prepare for
                their future careers. Students participate in academic
                activities, projects and teamwork.
            </p>
        </section>

        <!-- Courses Section -->
        <section id="courses" aria-labelledby="courses-heading">
            <h2 id="courses-heading">Courses and Departments</h2>

            <p>Some common engineering departments are:</p>

            <ul>
                <li>Computer Science and Engineering</li>
                <li>Mechanical Engineering</li>
                <li>Civil Engineering</li>
                <li>Electrical Engineering</li>
                <li>Electronics and Communication Engineering</li>
            </ul>
        </section>

        <!-- Article -->
        <article id="technology" aria-labelledby="technology-heading">
            <h2 id="technology-heading">Importance of Technology</h2>

            <p>
                Technology plays an important role in modern education.
                Students use computers, software and the internet to
                research information, complete assignments and learn
                programming.
            </p>

            <h3>Benefits of Technology</h3>

            <ul>
                <li>Improves problem-solving skills.</li>
                <li>Supports online learning and research.</li>
                <li>Helps students develop technical skills.</li>
            </ul>
        </article>

        <!-- Aside -->
        <aside aria-labelledby="tip-heading">
            <h2 id="tip-heading">Student Tip</h2>

            <p>
                Practise coding regularly, complete assignments on time
                and continue learning new technologies.
            </p>
        </aside>

        <!-- Contact Section -->
        <section id="contact" aria-labelledby="contact-heading">
            <h2 id="contact-heading">Contact Information</h2>

            <p>
                For college-related information, contact the college
                administration or visit the official website.
            </p>

            <p>
                <a
                    href="https://www.invertisuniversity.ac.in/"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    Visit Invertis University Official Website
                </a>
            </p>
        </section>

    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 My College Website. All rights reserved.</p>
        <p>Created for Assignment 3.4 — Semantic HTML & Accessibility.</p>
        <a href="#home">Back to Top</a>
    </footer>

</body>
</html>

4. Before and After Comparison

Before: Div-Based HTML

In the original div-based webpage, elements such as <div> were used to organize the header, navigation, content and footer. These containers did not clearly describe the purpose of each section.

Example:

<div class="header">
    <h1>My College Website</h1>
</div>

<div class="navigation">
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</div>

<div class="content">
    <h2>About My College</h2>
    <p>Welcome to my college website.</p>
</div>

<div class="footer">
    <p>Copyright 2026</p>
</div>

After: Semantic HTML

The webpage was restructured using meaningful HTML5 elements.

<header>
    <h1>My College Website</h1>
</header>

<nav aria-label="Main navigation">
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</nav>

<main>
    <section id="about">
        <h2>About My College</h2>
        <p>Welcome to my college website.</p>
    </section>
</main>

<footer>
    <p>Copyright 2026</p>
</footer>

5. Semantic HTML Elements Used

<header>: Contains the main heading and introductory information.

<nav>: Contains the navigation links.

<main>: Contains the main content of the webpage.

<section>: Groups related content into meaningful sections.

<article>: Contains a self-contained article about technology.

<aside>: Displays additional information and student tips.

<footer>: Contains copyright information and the Back to Top link.

6. Accessibility Improvements

Added lang="en" to identify the language of the webpage.

Added a viewport meta tag for responsive design.

Used a logical heading hierarchy with <h1>, <h2> and <h3>.

Added meaningful alt text to the image.

Added an accessible label to the navigation element.

Used descriptive text for links.

Added keyboard focus indicators to navigation links.

Used appropriate colors and readable text.

Added section labels using aria-labelledby.

Used responsive CSS to improve usability on smaller screens.

7. Testing and Validation

The following checks should be performed:

Open index.html in a web browser.

Check that all navigation links work correctly.

Verify that the Home, About, Courses, Technology and Contact links move to the correct sections.

Check that the image displays and has meaningful alternative text.

Use the Tab key to navigate through the links.

Inspect the webpage using the browser Developer Tools.

Validate the HTML using the W3C Nu HTML Checker.

Validation website: https://validator.w3.org/nu/

8. Before and After Screenshots

Screenshot 1: Before Semantic HTML

Capture a screenshot of the original div-based webpage before making changes.

File name: before-semantic-html.png

Screenshot 2: After Semantic HTML

Open the completed index.html webpage in a browser and capture a screenshot showing the updated semantic structure and design.

File name: after-semantic-html.png

Note: These screenshots must be captured from the actual webpage. The before screenshot should show the original div-based version, while the after screenshot should show the updated semantic version.

9. Result

The div-based webpage was converted into a semantic HTML webpage using <header>, <nav>, <main>, <section>, <article>, <aside> and <footer>. Accessibility was improved through meaningful alternative text, proper heading hierarchy, descriptive links, navigation labels and keyboard focus indicators.

The webpage is now better organized, easier to understand and more accessible to users and assistive technologies.