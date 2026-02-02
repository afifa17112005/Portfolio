# Ex01 Portfolio
## Date: 02/02/2026

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

#index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Afifa A | Portfolio</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #f4f6f8;
        }

        header {
            background-color: #0a4d68;
            color: white;
            padding: 20px;
            text-align: center;
        }

        header a {
            color: #ffd166;
            text-decoration: none;
            margin: 0 10px;
        }

        .tabs {
            background-color: #003049;
            text-align: center;
        }

        .tabs button {
            background: none;
            border: none;
            color: white;
            padding: 14px 20px;
            font-size: 16px;
            cursor: pointer;
        }

        .tabs button:hover {
            background-color: #1d3557;
        }

        .content {
            display: none;
            padding: 25px;
            background-color: white;
            margin: 20px;
            border-radius: 6px;
        }

        .active {
            display: block;
        }

        h2 {
            color: #0a4d68;
        }

        ul {
            line-height: 1.8;
        }
    </style>
</head>
<body>

<header>
    <h1>AFIFA A</h1>
    <p>Pre-final Year Computer Science Engineering Student</p>
    <p>
        Chennai | +91 93445 29859 | aneessafifa17@gmail.com <br>
        <a href="#">LinkedIn</a> | <a href="#">GitHub</a>
    </p>
</header>

<!-- Tabs -->
<div class="tabs">
    <button onclick="openTab('profile')">Profile</button>
    <button onclick="openTab('experience')">Experience & Education</button>
    <button onclick="openTab('projects')">Projects & Certifications</button>
</div>

<!-- Profile Tab -->
<div id="profile" class="content active">
    <h2>Profile</h2>
    <p>
        Pre-final year Computer Science Engineering student with a strong foundation in
        AI, Cloud Computing, and Networking. Experienced through internships in
        AI-driven data science and web development, with practical projects in IoT
        and cloud infrastructure. Earned 20+ Google Cloud Skill Badges and currently
        preparing for CCNA certification.
    </p>

    <h2>Skills & Abilities</h2>
    <ul>
        <li>Networking: Subnetting, Routing, Switching, TCP/IP</li>
        <li>Cloud & DevOps: Google Cloud, Terraform, Pub/Sub, Load Balancing</li>
        <li>Programming: Python, C</li>
        <li>Web Development: HTML, CSS, JavaScript (Basics)</li>
        <li>Machine Learning & IoT Fundamentals</li>
        <li>Strong analytical and problem-solving skills</li>
    </ul>
</div>

<!-- Experience & Education Tab -->
<div id="experience" class="content">
    <h2>Experience</h2>

    <h3>AI & Data Science Intern – Arjun Vision Tech</h3>
    <p><b>Dec 2024 – Feb 2025</b></p>
    <ul>
        <li>Worked on data preprocessing, model building, and evaluation</li>
        <li>Explored deep learning and generative AI tools</li>
        <li>Enhanced analytical and real-world problem-solving skills</li>
    </ul>

    <h3>Web Development Trainee – DLK Technologies Pvt Ltd</h3>
    <p><b>Jun 2024 – Jul 2024</b></p>
    <ul>
        <li>Built responsive websites using HTML, CSS, JavaScript</li>
        <li>Learned backend integration and web architecture basics</li>
        <li>Improved understanding of industry practices</li>
    </ul>

    <h2>Education</h2>
    <ul>
        <li>
            <b>B.E – Computer Science and Engineering</b><br>
            Saveetha Engineering College (2023 – 2027)<br>
            CGPA: 8.4
        </li>
        <li>
            <b>Higher Secondary (12th)</b><br>
            Bharathidhasanar Matric Hr. Sec. School – 2023<br>
            Score: 89.66%
        </li>
    </ul>
</div>

<!-- Projects & Certifications Tab -->
<div id="projects" class="content">
    <h2>Projects</h2>

    <h3>Smart Parking System</h3>
    <ul>
        <li>Technologies: Python, MySQL, HTML, CSS, IoT, Sensors</li>
        <li>Automated real-time slot detection to reduce congestion</li>
    </ul>

    <h3>Heart Disease Prediction System</h3>
    <ul>
        <li>Technologies: Python, Scikit-learn, Pandas, NumPy</li>
        <li>Built ML model to predict heart disease risk with improved accuracy</li>
    </ul>

    <h2>Certifications</h2>
    <ul>
        <li>Google Cloud Skills Boost – 20+ badges (Cloud, AI, Security)</li>
        <li>Coursera – Natural Language Processing</li>
        <li>Google – Prompt Design in Vertex AI</li>
        <li>Infosys – Deep Learning Fundamentals</li>
    </ul>
</div>

<script>
    function openTab(tabId) {
        var contents = document.getElementsByClassName("content");
        for (var i = 0; i < contents.length; i++) {
            contents[i].style.display = "none";
        }
        document.getElementById(tabId).style.display = "block";
    }
</script>

</body>
</html>
```

#style.css

```
/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background-color: #191B1F;
    background-image: url("https://www.transparenttextures.com/patterns/asfalt-light.png");
    background-repeat: repeat;
    color: #E6E8EB;
    line-height: 1.6;
}

/* Navigation */
header {
    background: #14161A;
    padding: 15px 30px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 10;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav .logo {
    font-size: 1.5em;
    color: #3ABEFF;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    color: #E6E8EB;
    text-decoration: none;
    font-weight: bold;
}

nav ul li a:hover {
    color: #4DD9FF;
}

/* Home Section */
.home-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 100px 30px;
    min-height: 100vh;
}

.about-text {
    width: 50%;
}

.profile-pic {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    background-color: #3ABEFF;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    box-shadow: 0 0 25px rgba(58, 190, 255, 0.6);
}

.profile-pic img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Projects Section */
.projects-section {
    padding: 100px 30px;
    text-align: center;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    margin-top: 30px;
}

.project-card {
    padding: 20px;
    border-radius: 10px;
    background-color: #2A2E35;
    color: #E6E8EB;
    min-height: 150px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card h3 {
    color: #3ABEFF;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(77, 217, 255, 0.35);
}

/* Skills Section */
.skills-section {
    padding: 100px 30px;
}

.skill {
    margin-bottom: 20px;
}

.bar {
    background: #14161A;
    border-radius: 5px;
    overflow: hidden;
    height: 20px;
}

.fill {
    height: 100%;
    text-align: right;
    padding-right: 5px;
    color: #14161A;
    font-size: 12px;
    font-weight: bold;
}

.python { width: 85%; background: #3ABEFF; }
.c { width: 80%; background: #1F4FD8; color: #E6E8EB; }
.html { width: 95%; background: #4DD9FF; }
.css { width: 90%; background: #3ABEFF; }
.js { width: 85%; background: #1F4FD8; color: #E6E8EB; }
.react { width: 75%; background: #4DD9FF; }

```
## OUTPUT

#Home Page
<img width="1919" height="912" alt="Screenshot 2026-02-02 140342" src="https://github.com/user-attachments/assets/006df170-6e18-434b-adaa-98db529423a3" />


#Projects Page
<img width="1901" height="921" alt="Screenshot 2026-02-02 140439" src="https://github.com/user-attachments/assets/b566ae3e-2818-4a5f-9d1a-da39444e47d4" />



#Experience Page
<img width="1916" height="930" alt="Screenshot 2026-02-02 140355" src="https://github.com/user-attachments/assets/8f406f6d-eeaa-4b36-adf8-04192b8734fc" />

<img width="1879" height="897" alt="Screenshot 2026-02-02 140408" src="https://github.com/user-attachments/assets/cfc2420a-19e8-4e71-8b44-5e6631ecd43c" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
