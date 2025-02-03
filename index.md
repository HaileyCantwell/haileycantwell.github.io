<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Resume</title>
  <!-- Theme Customization -->
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background-color: #2b3a2e; /* Dark Earthy Green */
      color: #333333; /* Darker, Readable Text */
    }

    header {
      background: #2a4531; /* Darker Forest Green */
      color: #ffffff;
      padding: 20px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .content {
      padding: 20px;
    }

    .resume-section {
      margin-bottom: 20px;
      border-left: 5px solid #4a6b4a; /* Muted Green Border */
      padding-left: 10px;
    }

    .about-container {
      display: flex;
      align-items: center;
    }

    .about-text {
      flex: 1;
      padding-right: 20px;
    }

    .about-photo img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
    }

    .theme-toggle {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #2a4531;
      color: #e8f5e9;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
    }

    .dark-theme {
      background-color: #1e2a24; /* Even Darker Green */
      color: #ffffff;
    }

    .dark-theme header {
      background: #1c3224;
      color: #ffffff;
    }

    .dark-theme .theme-toggle {
      background: #1c3224;
      color: #e8f5e9;
    }

    .dark-theme .resume-section {
      border-left: 5px solid #4a6b4a; /* Softer Green Border */
    }
  </style>
</head>
<body>

<header>
  <h1>My Resume</h1>
</header>

<div class="content">
  <section class="resume-section">
    <div class="about-container">
      <div class="about-text">
        <h2>About Me</h2>
        <p>Hello! I am [Your Name], a [Your Profession] with experience in [Your Expertise].</p>
      </div>
      <div class="about-photo">
        <img src="your-photo.jpg" alt="Your Photo">
      </div>
    </div>
  </section>

  <section class="resume-section">
    <h2>Work Experience</h2>
    <p>Include your work experience here.</p>
  </section>

  <section class="resume-section">
    <h2>Education</h2>
    <p>List your educational background here.</p>
  </section>

  <section class="resume-section">
    <h2>Skills</h2>
    <p>Highlight your skills here.</p>
  </section>
</div>

<button class="theme-toggle" onclick="toggleTheme()">Switch Theme</button>

<script>
  function toggleTheme() {
    document.body.classList.toggle('dark-theme');
  }
</script>

</body>
</html>
