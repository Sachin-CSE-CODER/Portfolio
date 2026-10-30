# Ex01 Portfolio
## Date:30-10-26
## Regno:212224040283
## Name:SACHIN S

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
html
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sachin S | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation -->
    <header>
        <nav>
            <h2 class="logo">SACHIN<span>.</span></h2>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <p class="welcome">WELCOME TO MY PORTFOLIO</p>

            <h1>Hello, I'm <span>SACHIN S</span></h1>

            <h3>Computer Science Student | Developer</h3>

            <p>
                I am a Computer Science student passionate about
                programming, web development, Artificial Intelligence
                and Machine Learning. I love learning new technologies
                and building innovative projects.
            </p>

            <a href="#projects" class="btn">View My Projects</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <h2>About Me</h2>

        <p>
            I am a Computer Science and Engineering student at
            Saveetha Engineering College, Chennai. I have an interest
            in software development, Artificial Intelligence and
            Machine Learning. I enjoy solving problems, exploring
            new technologies and developing practical applications.
            My goal is to become a skilled software developer.
        </p>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="section">
        <h2>My Skills</h2>

        <div class="skills-container">
            <div class="skill">HTML</div>
            <div class="skill">CSS</div>
            <div class="skill">JavaScript</div>
            <div class="skill">Python</div>
            <div class="skill">Java</div>
            <div class="skill">C Programming</div>
            <div class="skill">Machine Learning</div>
            <div class="skill">Deep Learning</div>
            <div class="skill">SQL</div>
            <div class="skill">React</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="section">
        <h2>My Projects</h2>

        <div class="projects-container">

            <div class="project-card">
                <h3>PDS Queue Management System</h3>
                <p>
                    A project designed to improve queue management
                    and reduce waiting time in the Public Distribution
                    System using technology.
                </p>
            </div>

            <div class="project-card">
                <h3>OS Scan Classification</h3>
                <p>
                    A Machine Learning project that uses
                    classification algorithms to identify
                    operating system scan patterns.
                </p>
            </div>

            <div class="project-card">
                <h3>Digital Product Development</h3>
                <p>
                    A web-based application developed using
                    PHP, MySQL, JavaScript and Tailwind CSS
                    for digital product management.
                </p>
            </div>

        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section contact">
        <h2>Contact Me</h2>

        <p>Email: Add your email address</p>
        <p>College: Saveetha Engineering College</p>
        <p>Department: Computer Science and Engineering</p>

        <a href="https://github.com/Sachin-CSE-CODER"
           target="_blank" class="btn">
            Visit My GitHub
        </a>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Sachin S | My Portfolio</p>
    </footer>

</body>
</html>

```
css
```

/* General Styling */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background-color: #111;
    color: white;
}

/* Navigation */
header {
    background-color: #000;
    padding: 20px 8%;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: white;
    font-size: 28px;
}

.logo span {
    color: red;
}

nav ul {
    display: flex;
    list-style: none;
    gap: 25px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

nav ul li a:hover {
    color: red;
}

/* Home Section */
.hero {
    min-height: 85vh;
    display: flex;
    align-items: center;
    padding: 50px 10%;
    background: linear-gradient(
        120deg, #000, #300000, #111
    );
}

.hero-content {
    max-width: 650px;
}

.welcome {
    color: red;
    letter-spacing: 3px;
    margin-bottom: 20px;
}

.hero h1 {
    font-size: 45px;
    margin-bottom: 15px;
}

.hero h1 span {
    color: red;
}

.hero h3 {
    margin-bottom: 20px;
    color: #ccc;
}

.hero p {
    line-height: 1.7;
    margin-bottom: 25px;
}

/* Button */
.btn {
    display: inline-block;
    background-color: red;
    color: white;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 10px;
}

.btn:hover {
    background-color: darkred;
}

/* Common Sections */
.section {
    padding: 65px 10%;
    text-align: center;
}

.section h2 {
    color: red;
    font-size: 32px;
    margin-bottom: 25px;
}

.section p {
    line-height: 1.8;
    color: #ccc;
    max-width: 850px;
    margin: auto;
}

/* Skills */
.skills-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 15px;
}

.skill {
    background-color: #222;
    border: 1px solid red;
    padding: 15px 25px;
    border-radius: 5px;
    transition: 0.3s;
}

.skill:hover {
    background-color: red;
    transform: translateY(-5px);
}

/* Projects */
.projects-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

.project-card {
    background-color: #222;
    border: 1px solid #444;
    padding: 25px;
    width: 280px;
    border-radius: 8px;
    transition: 0.3s;
}

.project-card:hover {
    border-color: red;
    transform: translateY(-8px);
}

.project-card h3 {
    color: red;
    margin-bottom: 15px;
}

.project-card p {
    font-size: 14px;
}

/* Contact */
.contact {
    background-color: #1a1a1a;
}

.contact p {
    margin-bottom: 10px;
}

/* Footer */
footer {
    background-color: black;
    text-align: center;
    padding: 20px;
    color: #aaa;
}

/* Responsive Design */
@media (max-width: 768px) {

    nav {
        flex-direction: column;
        gap: 20px;
    }

    nav ul {
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
    }

    .hero h1 {
        font-size: 32px;
    }

    .projects-container {
        flex-direction: column;
        align-items: center;
    }
}

```

## OUTPUT
<img width="1900" height="906" alt="image" src="https://github.com/user-attachments/assets/1eb6c784-f053-4489-b358-34192fb878e1" />
<img width="1896" height="802" alt="image" src="https://github.com/user-attachments/assets/54845aa8-51b8-4d01-a409-0cbb2a517d1d" />
<img width="1891" height="883" alt="image" src="https://github.com/user-attachments/assets/c6e3de45-a2df-4905-b164-7075b3e5b826" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
