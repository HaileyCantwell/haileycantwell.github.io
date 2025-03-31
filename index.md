<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hailey Cantwell - Resume</title>
  <!-- Theme Customization -->
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background-color: #2b3a2e; /* Dark Earthy Green */
      color: #000000; /* Darker, Readable Text */
      transition: margin-left 0.3s;
    }

    header {
      background: #2a4531; /* Darker Forest Green */
      color: #FDFBD4;
      padding: 20px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .content {
      padding: 20px;
      margin-left: 260px; /* Adjusted to make space for the sidebar */
      transition: margin-left 0.3s;
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

    /* Sidebar Styles */
    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      width: 250px;
      background-color: #2a4531; /* Darker Forest Green */
      padding-top: 20px;
      color: #FDFBD4;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      transition: width 0.3s;
      overflow-x: hidden;
    }

    .sidebar h2 {
      text-align: center;
      font-size: 1.5em;
      margin-bottom: 20px;
    }

    .sidebar ul {
      list-style-type: none;
      padding: 0;
    }

    .sidebar ul li {
      padding: 10px;
      text-align: center;
    }

    .sidebar ul li a {
      color: #FDFBD4;
      text-decoration: none;
      display: block;
      padding: 10px;
      border-radius: 5px;
      transition: background 0.3s;
    }

    .sidebar ul li a:hover {
      background-color: #4a6b4a; /* Muted Green */
    }

    .sidebar.collapsed {
      width: 60px;
    }

    .content.collapsed {
      margin-left: 60px;
    }

    .toggle-btn {
      position: fixed;
      top: 20px;
      left: 260px;
      background-color: #2a4531;
      color: #FDFBD4;
      border: none;
      padding: 10px;
      cursor: pointer;
      transition: left 0.3s;
    }

    .toggle-btn.collapsed {
      left: 60px;
    }
  </style>
</head>
<body>

<!-- Side Navigation Bar -->
<nav id="sidebar" class="sidebar">
  <h2>Repositories</h2>
  <ul>
    <li><a href="https://haileycantwell.github.io/MAT434/" target="_blank">MAT434 Repository</a></li>
    <li><a href="https://github.com/haileycantwell/OtherRepo1" target="_blank">Other Repository 1</a></li>
    <li><a href="https://github.com/haileycantwell/OtherRepo2" target="_blank">Other Repository 2</a></li>
  </ul>
</nav>

<button id="toggle-btn" class="toggle-btn">☰</button>

<header>
  <h1>Hailey Cantwell</h1>
  <p>Concord, NH | hailey.cantwell@snhu.edu </p>
</header>

<div class="content" id="main-content">
  <section class="resume-section">
    <div class="about-container">
      <div class="about-text">
        <h2>About Me</h2>
        <p>My name is Hailey Cantwell, a senior studying psychology with a concentration in child and adolescent development and a minor in research. I am an extremely hard worker, a critical thinker, and I work very well in a fast-paced environment. I am someone who enjoys continuing to further my knowledge and understanding. Check out my LinkedIn profile: <a href="http://www.linkedin.com/in/hailey-c-7a7204132" target="_blank">Hailey Cantwell</a></p>
      </div>
      <div class="about-photo">
        <img src="462088368_9126027347429766_7566780716905499347_n.jpg" alt="Your Photo">
      </div>
    </div>
  </section>
</div>

<!-- JavaScript for Toggle Button -->
<script>
  const sidebar = document.getElementById('sidebar');
  const content = document.getElementById('main-content');
  const toggleBtn = document.getElementById('toggle-btn');

  toggleBtn.addEventListener('click', () => {
    sidebar.classList.toggle('collapsed');
    content.classList.toggle('collapsed');
    toggleBtn.classList.toggle('collapsed');
  });
</script>

</body>
</html>
