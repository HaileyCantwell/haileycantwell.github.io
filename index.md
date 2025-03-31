<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hailey Cantwell - Professional Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(120deg, #d9e4dd, #f0f0f0);
      color: #2b3a2e;
      overflow-x: hidden;
    }

    header {
      background: #2a4531;
      color: #FDFBD4;
      padding: 20px;
      text-align: center;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .content {
      padding: 20px;
      margin-left: 250px;
      padding-top: 120px;
      transition: margin-left 0.3s;
      max-width: 1200px;
      margin: auto;
    }

    .resume-section {
      background: white;
      padding: 20px;
      border-radius: 8px;
      border-left: 5px solid #4a6b4a;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      margin-bottom: 20px;
    }

    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      width: 250px;
      background-color: #2a4531;
      padding-top: 20px;
      color: white;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      transition: width 0.3s;
      overflow: hidden;
      z-index: 1001;
    }

    .sidebar.collapsed {
      width: 0;
    }

    .profile-info {
      text-align: center;
      padding: 10px;
    }

    .profile-info img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 10px;
    }

    .profile-info a {
      color: #C0E4C8;
      text-decoration: none;
      display: block;
      transition: color 0.3s;
    }

    .profile-info a:hover {
      color: #FDFBD4;
    }

    .toggle-btn {
      position: fixed;
      top: 20px;
      left: 260px;
      background-color: #4a6b4a;
      color: white;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      border-radius: 5px;
      z-index: 1002;
      transition: left 0.3s;
    }

    .toggle-btn.collapsed {
      left: 10px;
    }

    .collapsible {
      cursor: pointer;
      padding: 10px;
      border: none;
      outline: none;
      width: 100%;
      text-align: left;
      background-color: #4a6b4a;
      color: white;
      border-radius: 5px;
      margin-top: 10px;
    }

    .collapsible-content {
      padding: 10px;
      display: none;
    }

    .active {
      display: block;
    }

    h3.mint-color {
      color: #C0E4C8; /* Mint Color */
    }

    a.mint-link {
      color: #C0E4C8; /* Mint Color */
      text-decoration: none;
      transition: color 0.3s;
    }

    a.mint-link:hover {
      color: #FDFBD4;
    }
  </style>
</head>
<body>

<!-- Sidebar -->
<nav id="sidebar" class="sidebar">
  <div class="profile-info">
    <img src="462088368_9126027347429766_7566780716905499347_n.jpg" alt="Hailey Cantwell">
    <h2>Hailey Cantwell</h2>
    <p>Concord, NH</p>
    <p>Southern New Hampshire University</p>
    <p>Bachelor's in Child and Adolescent Psychology</p>
    <p><a href="mailto:hailey.cantwell@snhu.edu">Email Me</a></p>
    <p><a href="https://www.linkedin.com/in/hailey-c-7a7204132" target="_blank">LinkedIn Profile</a></p>
  </div>
</nav>

<button id="toggle-btn" class="toggle-btn">☰ Menu</button>

<header>
  <h1>Hailey Cantwell - Professional Portfolio</h1>
  <h3 class="mint-color">Welcome to Hailey Cantwell's GitHub Page!</h3>
</header>

<div class="content">
  <section class="resume-section">
    <h2>About Me</h2>
    <p>Hello! I'm Hailey Cantwell, a senior studying psychology with a concentration in child and adolescent development and a minor in research. I am passionate about understanding and improving the lives of children through research and evidence-based practices.</p>
  </section>

  <section class="resume-section">
    <h2>Projects & Research</h2>
    <button class="collapsible">Projects</button>
    <div class="collapsible-content">
      <p><strong>MAT434 Spaceship Repository:</strong> Explore my coursework for MAT434, including research, analysis, and statistical models. <a href="https://github.com/HaileyCantwell/MAT434.git" class="mint-link" target="_blank">Visit Repository</a></p>
    </div>

    <button class="collapsible">Research</button>
    <div class="collapsible-content">
      <p><strong>Research on Parenting Styles & Screen Time:</strong> Exploring relationships between parenting styles, parental stress, and children's screen time habits.</p>
      <p><strong>Thesis: Intergenerational Addiction & Technology:</strong> Investigating the impact of intergenerational addiction on children's technology-related compulsive behaviors.</p>
    </div>
  </section>
</div>

<script>
  const sidebar = document.getElementById('sidebar');
  const toggleBtn = document.getElementById('toggle-btn');
  const collapsibles = document.querySelectorAll('.collapsible');

  toggleBtn.addEventListener('click', () => {
    sidebar.classList.toggle('collapsed');
    toggleBtn.classList.toggle('collapsed');
  });

  collapsibles.forEach(button => {
    button.addEventListener('click', () => {
      const content = button.nextElementSibling;
      content.classList.toggle('active');
    });
  });
</script>

</body>
</html>
