<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hailey Cantwell - Professional Resume</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #2b3a2e;
      color: #ffffff;
      margin: 0;
      padding: 0;
    }

    header {
      background: #3c5b43;
      color: #ffffff;
      padding: 20px;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .sidebar {
      position: fixed;
      left: 0;
      top: 0;
      height: 100%;
      width: 250px;
      background-color: #3c5b43;
      color: #ffffff;
      padding-top: 60px;
      transition: width 0.3s;
    }

    .sidebar.collapsed {
      width: 60px;
    }

    .sidebar h2 {
      text-align: center;
      font-size: 1.5em;
    }

    .sidebar ul {
      list-style-type: none;
      padding: 0;
    }

    .sidebar ul li a {
      color: #ffffff;
      text-decoration: none;
      padding: 10px;
      display: block;
    }

    .content {
      margin-left: 250px;
      padding: 20px;
      padding-top: 80px;
    }

    .profile {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 20px;
    }

    .profile img {
      border-radius: 50%;
      width: 150px;
      height: 150px;
      margin-bottom: 10px;
    }

    .toggle-btn {
      position: fixed;
      left: 250px;
      top: 20px;
      background-color: #3c5b43;
      color: #ffffff;
      border: none;
      padding: 10px;
      cursor: pointer;
      transition: left 0.3s;
      font-size: 1.2em;
    }

    .toggle-btn.collapsed {
      left: 60px;
    }
  </style>
</head>
<body>
  <div class="sidebar" id="sidebar">
    <h2>Repositories</h2>
    <ul>
      <li><a href="#">MAT434 Repository</a></li>
      <li><a href="#">Other Project 1</a></li>
      <li><a href="#">Other Project 2</a></li>
    </ul>
  </div>
  <button class="toggle-btn" id="toggle-btn">☰</button>
  <header>
    <div class="profile">
      <img src="profile.jpg" alt="Hailey Cantwell">
      <p>Hailey Cantwell</p>
      <p>Concord, NH</p>
      <p>hailey.cantwell@snhu.edu</p>
    </div>
  </header>
  <div class="content">
    <h2>About Me</h2>
    <p>I am a senior psychology major concentrating on child and adolescent development. I am passionate about research, learning, and working in fast-paced environments.</p>
  </div>
  <script>
    const sidebar = document.getElementById('sidebar');
    const toggleBtn = document.getElementById('toggle-btn');

    toggleBtn.addEventListener('click', () => {
      sidebar.classList.toggle('collapsed');
      toggleBtn.classList.toggle('collapsed');
    });
  </script>
</body>
</html>
