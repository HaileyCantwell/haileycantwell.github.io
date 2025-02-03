
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
      color: #d4d7b6; /* Soft Neutral Text */
    }

    header {
      background: #3e5c41; /* Deep Forest Green */
      color: #e8f5e9;
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
      border-left: 5px solid #5a7d5a; /* Muted Green Border */
      padding-left: 10px;
    }

    .theme-toggle {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #3e5c41;
      color: #e8f5e9;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
    }

    .dark-theme {
      background-color: #1e2a24; /* Even Darker Green */
      color: #c3c7a6;
    }

    .dark-theme header {
      background: #2b3a2e;
      color: #e8f5e9;
    }

    .dark-theme .theme-toggle {
      background: #2b3a2e;
      color: #e8f5e9;
    }

    .dark-theme .resume-section {
      border-left: 5px solid #5a7d5a; /* Softer Green Border */
    }
  </style>
</head>
<body>

<header>
  <h1>My Resume</h1>
</header>

<div class="content">
  <section class="resume-section">
    <h2>About Me</h2>
    <p>Hello! I am [Your Name], a [Your Profession] with experience in [Your Expertise].</p>
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
