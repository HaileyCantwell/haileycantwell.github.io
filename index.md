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
      background-color: #fff7f0; /* Default Theme: Light Floral */
      color: #4d4d4d;
    }

    header {
      background: #f7d9d9; /* Soft Pink Header */
      color: #4d2c2c;
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
      border-left: 5px solid #f2a6a6; /* Floral Pink Border */
      padding-left: 10px;
    }

    .theme-toggle {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #f7d9d9;
      color: #4d2c2c;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
    }

    .dark-theme {
      background-color: #2e3532; /* Dark Green for Night */
      color: #f1f1f1;
    }

    .dark-theme header {
      background: #3a5a40; /* Forest Green Header */
      color: #e8f5e9;
    }

    .dark-theme .theme-toggle {
      background: #3a5a40;
      color: #e8f5e9;
    }

    .dark-theme .resume-section {
      border-left: 5px solid #74c69d; /* Soft Green Border */
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
    <p>Hello! I am Hailey Cantwell, a senior at Southern New Hampshire University with experience in Psychology with a concentration in child development and a minor in research.</p>
  </section>

  <section class="resume-section">
    <h2>Work Experience</h2>
    <p>Farmsteads of New England 8/2024-Current</p>
    <p>Psychology Major Ambassador - Southern New Hampshire University 8/2024-Current</p>
  </section>

  <section class="resume-section">
    <h2>Education</h2>
    <p>Southern New Hampshire University - Class 2025.</p>
  </section>

  <section class="resume-section">
    <h2>Skills</h2>
    <p>Research, analytical skills</p>
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
