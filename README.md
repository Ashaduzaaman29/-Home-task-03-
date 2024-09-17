<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Comprehensive example of HTML tags, forms, units, and modern features.">
    <meta name="keywords" content="HTML, Forms, Inputs, CSS, JavaScript, Units, Graphics, Responsive, Semantic, XHTML">
    <title>Web Solutions Co. - Comprehensive HTML Example</title>


    <link rel="stylesheet" href="styles.css">

    <!-- Inline CSS for styling -->
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        section, article {
            padding: 20px;
            margin: 10px;
        }
        footer {
            background-color: #f1f1f1;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        .services, .team {
            display: flex;
            justify-content: space-around;
        }
        .team img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
        }
        .contact-form {
            background-color: #eaeaea;
            padding: 20px;
            border-radius: 10px;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
        }
        .highlight {
            color: red;
        }

        header, nav, section, article, aside, footer {
            display: block;
        }
    </style>
</head>
<body>


    <header>
        <h1>Welcome to Web Solutions Co.</h1>
        <p>Delivering Full-Stack Web and Mobile Solutions</p>
    </header>


    <nav>
        <a href="#about">About Us</a>
        <a href="#services">Services</a>
        <a href="#form-example">Form Example</a>
        <a href="#graphics">Graphics</a>
        <a href="#iframes">Iframes</a>
        <a href="#semantic">HTML Semantic</a>
        <a href="#entities">Entities & Symbols</a>
    </nav>


    <div class="container">

        <section id="about">
            <h2>About Web Solutions Co.</h2>
            <p>We specialize in delivering cutting-edge web and mobile applications, leveraging modern technologies to empower businesses.</p>
            <p>For more information, <a href="#contact" class="highlight">contact us today</a>.</p>
        </section>


        <section id="services">
            <h2>Our Services</h2>
            <div class="services">
                <article>
                    <h3>Web Development</h3>
                    <p>Building responsive, high-performance websites with modern frameworks like React, Vue, and Angular.</p>
                </article>
                <article>
                    <h3>Mobile Apps</h3>
                    <p>Developing cross-platform mobile apps using Flutter, React Native, and Swift for seamless user experiences.</p>
                </article>
                <article>
                    <h3>Cloud Integration</h3>
                    <p>Implementing scalable cloud solutions with AWS, Google Cloud, and Azure to meet your growing business needs.</p>
                </article>
            </div>
        </section>

        <section id="form-example">
            <h2>Contact Us Form</h2>
            <form action="/submit" method="POST" enctype="multipart/form-data" autocomplete="on" target="_self" novalidate>
                <fieldset>
                    <legend>Get in Touch</legend>
                    <label for="name">Full Name:</label>
                    <input type="text" id="name" name="name" placeholder="Your Name" required maxlength="50"><br><br>

                    <label for="email">Email Address:</label>
                    <input type="email" id="email" name="email" placeholder="your.email@example.com" required><br><br>

                    <label for="phone">Phone Number:</label>
                    <input type="tel" id="phone" name="phone" placeholder="123-456-7890" size="15"><br><br>

                    <label for="service">Service Interested In:</label>
                    <select id="service" name="service">
                        <optgroup label="Development">
                            <option value="web">Web Development</option>
                            <option value="mobile">Mobile Development</option>
                        </optgroup>
                        <optgroup label="Cloud Solutions">
                            <option value="cloud">Cloud Solutions</option>
                        </optgroup>
                    </select><br><br>

                    <label for="gender">Gender:</label><br>
                    <input type="radio" id="male" name="gender" value="male">
                    <label for="male">Male</label><br>
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Female</label><br><br>

                    <label for="message">Message:</label>
                    <textarea id="message" name="message" placeholder="Your message here..." required></textarea><br><br>

                    <label for="file-upload">Upload a File:</label>
                    <input type="file" id="file-upload" name="file"><br><br>

                    <button type="submit" formaction="/submit-form" formmethod="post" formtarget="_self" formenctype="multipart/form-data" formnovalidate>Submit</button>
                </fieldset>
            </form>
        </section>


        <section id="graphics">
            <h2>Our Technology Stack - Graphics</h2>


            <article>
                <h3>Canvas Drawing</h3>
                <canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;">
                    Your browser does not support the HTML5 canvas tag.
                </canvas>
                <script>
                    const canvas = document.getElementById('myCanvas');
                    const ctx = canvas.getContext('2d');
                    ctx.fillStyle = "#FF0000";
                    ctx.fillRect(20, 20, 150, 75);
                </script>
            </article>

            <article>
                <h3>SVG Logo</h3>
                <svg height="100" width="100">
                    <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="green" />
                    Sorry, your browser does not support inline SVG.
                </svg>
            </article>
        </section>


        <section id="iframes">
            <h2>Embedded Page - Iframe</h2>
            <p>Check out this embedded page from our partners:</p>
            <iframe src="https://www.example.com" width="600" height="400" frameborder="0" title="Iframe Example"></iframe>
        </section>


        <section id="semantic">
            <h2>HTML Semantic Elements</h2>
            <article>
                <h3>Overview of Semantic Tags</h3>
                <p>Semantic HTML tags help define the purpose of the content. Tags like <code>&lt;article&gt;</code>, <code>&lt;section&gt;</code>, <code>&lt;aside&gt;</code>, and <code>&lt;footer&gt;</code> provide a clear structure to the webpage.</p>
            </article>
        </section>


        <section id="entities">
            <h2>HTML Entities and Symbols</h2>
            <article>
                <h3>Common HTML Entities</h3>
                <p>Here are some commonly used entities:</p>
                <ul>
                    <li>&amp; (Ampersand)</li>
                    <li>&lt; (Less Than)</li>
                    <li>&gt; (Greater Than)</li>
                    <li>&copy; (Copyright)</li>
                    <li>&euro; (Euro)</li>
                </ul>

                <h3>Symbols</h3>
                <p>Here are some symbols you can use in HTML:</p>
                <ul>
                    <li>&#10084; (Heart)</li>
                    <li>&#9733; (Star)</li>
                    <li>&#9829; (Heart with a different code)</li>
                </ul>
            </article>
        </section>
    </div>

 
    <footer>
        <p>&copy; 2024 Web Solutions Co. All Rights Reserved.</p>
        <noscript>JavaScript is disabled on your browser, please enable it for better experience.</noscript>
    </footer>


    <script>

        document.querySelector('.highlight').style.color = 'blue';

     
        document.getElementById('phone').style.backgroundColor = '#eaeaea';
    </script>
</body>
</html>
