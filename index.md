
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
      padding-top: 100px;
      color: white;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      transition: width 0.3s;
      overflow-x: hidden;
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
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 10px;
    }

    .profile-info a {
      color: #C0E4C8;
      text-decoration: none;
      display: block;
      margin: 5px 0;
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
      color: #C0E4C8;
    }

    a.mint-link {
      color: #C0E4C8;
      text-decoration: none;
      transition: color 0.3s;
    }

    a.mint-link:hover {
      color: #FDFBD4;
    }

    /* 📱 Responsive Mobile Tweaks */
    @media (max-width: 768px) {
      .sidebar {
        width: 0;
      }

      .content {
        margin-left: 0;
        padding-top: 100px;
      }

      .toggle-btn {
        left: 10px;
      }

      header h1 {
        font-size: 1.5em;
      }

      header h3 {
        font-size: 1em;
      }
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
      <p><strong>Data Analysis: Technology Use and Mental Health:</strong> View the complete R Markdown project output.  
        <a href="<a href="https://haileycantwell.github.io/MAT434/Final%20Project/final_proj.html" class="mint-link" target="_blank">View Report</a>
      </p>
    </div>

    <button class="collapsible">Research</button>
    <div class="collapsible-content">
      <p><strong>Completed Thesis - "Inherited Vulnerability":</strong> Exploring intergenerational addiction and technology-related compulsive behaviors.  
        <a href="https://github.com/HaileyCantwell/haileycantwell.github.io/raw/main/SiteFiles/Inherited%20Vulnerability.pdf" class="mint-link" target="_blank">View Thesis (PDF)</a>
      </p>
      <p><strong>Independent Study - "Parenting Under Pressure":</strong> Research on parenting stress, screen time, and child behavior.  
        <a href="https://github.com/HaileyCantwell/haileycantwell.github.io/raw/main/SiteFiles/Parenting%20Under%20Pressure.pdf" class="mint-link" target="_blank">View Independent Study (PDF)</a>
      </p>
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

