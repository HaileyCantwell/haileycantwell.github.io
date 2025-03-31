<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hailey Cantwell ~ Professional Portfolio </title>
  <!-- Theme Customization -->
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background-color: #f0f0f0; /* Light Background for Clean Look */
      color: #2b3a2e;
      overflow-x: hidden;
    }

    header {
      background: #2a4531;
      color: #FDFBD4;
      padding: 10px;
      text-align: center;
      position: fixed;
      top: 0;
      left: 250px;
      width: calc(100% - 250px);
      z-index: 1000;
      transition: left 0.3s, width 0.3s;
    }

    .content {
      padding: 20px;
      margin-left: 250px;
      padding-top: 80px;
      transition: margin-left 0.3s;
    }

    .resume-section {
      margin-bottom: 20px;
      background: white;
      padding: 15px;
      border-radius: 8px;
      border-left: 5px solid #4a6b4a;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      width: 250px;
      background-color: #2a4531;
      padding-top: 20px;
      color: #FDFBD4;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      transition: width 0.3s;
      overflow-y: auto;
    }

    .sidebar.collapsed {
      width: 0;
      overflow: hidden;
    }

    .toggle-btn {
      position: fixed;
      top: 20px;
      left: 10px;
      background-color: #4a6b4a;
      color: white;
      border: none;
      padding: 12px 18px;
      cursor: pointer;
      border-radius: 8px;
      font-size: 18px;
      z-index: 1001;
    }

    .sidebar h2 {
      text-align: center;
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
      background-color: #4a6b4a;
    }

    .profile-info {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 15px;
    }

    .profile-info img {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 15px;
    }

    .profile-info h1, .profile-info p {
      text-align: center;
      margin: 5px 0;
    }
  </style>
</head>
<body>

<!-- Sidebar -->
<nav id="sidebar" class="sidebar">
  <div class="profile-info">
    <img src="462088368_9126027347429766_7566780716905499347_n.jpg" alt="Hailey Cantwell">
    <h1>Hailey Cantwell</h1>
    <p>Concord, NH</p>
    <p>hailey.cantwell@snhu.edu</p>
  </div>
  <h2>Repositories</h2>
  <ul>
    <li><a href="https://haileycantwell.github.io/MAT434/" target="_blank">MAT434 Repository</a></li>
    <li><a href="https://github.com/haileycantwell/OtherRepo1" target="_blank">Other Repository 1</a></li>
    <li><a href="https://github.com/haileycantwell/OtherRepo2" target="_blank">Other Repository 2</a></li>
  </ul>
</nav>

<button id="toggle-btn" class="toggle-btn">☰ Menu</button>

<header>
  <h1>Hailey Cantwell - Professional Portfolio</h1>
</header>

<div class="content" id="main-content">
  <section class="resume-section">
    <h2>About Me</h2>
    <p>I am a senior studying psychology with a concentration in child and adolescent development and a minor in research. I am a critical thinker who thrives in fast-paced environments. I enjoy expanding my knowledge and applying it to real-world projects. Check out my LinkedIn profile: <a href="http://www.linkedin.com/in/hailey-c-7a7204132" target="_blank">Hailey Cantwell</a></p>
  </section>
  <section class="resume-section">
    <h2>Projects</h2>
    <p>Explore the various projects I've completed throughout my coursework and independent research.</p>
  </section>
</div>

<script>
  const sidebar = document.getElementById('sidebar');
  const toggleBtn = document.getElementById('toggle-btn');
  const content = document.getElementById('main-content');
  const header = document.querySelector('header');

  toggleBtn.addEventListener('click', () => {
    sidebar.classList.toggle('collapsed');
    if (sidebar.classList.contains('collapsed')) {
      content.style.marginLeft = '0';
      header.style.left = '0';
      header.style.width = '100%';
    } else {
      content.style.marginLeft = '250px';
      header.style.left = '250px';
      header.style.width = 'calc(100% - 250px)';
    }
  });
</script>

</body>
</html>
