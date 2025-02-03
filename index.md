
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
  <h1>Hailey Cantwell</h1>
  <p>Concord, NH | hailey.cantwell@snhu.edu </p>
</header>

<div class="content">
  <section class="resume-section">
    <div class="about-container">
      <div class="about-text">
        <h2>About Me</h2>
        <p>My name is Hailey Cantwell, a senior studying psychology with a concentration in child and adolescent development and a minor in research. I am an extremely hard worker, a critical thinker, and work very well in a fast-paced environment. I am someone who enjoys continuing to further my knowledge and understanding. Check out my LinkedIn profile: <a href="http://www.linkedin.com/in/hailey-c-7a7204132" target="_blank">Hailey Cantwell</a></p>
      </div>
      <div class="about-photo">
        <img src="462088368_9126027347429766_7566780716905499347_n.jpg" alt="Your Photo">
      </div>
    </div>
  </section>

  <section class="resume-section">
    <h2>Work Experience</h2>
    <p><strong>DSP (Direct Support Professional)</strong> - Farmsteads of New England, Inc. (Aug 2024 - Present)</p>
    <p>Support adults with intellectual and developmental disabilities in a residential setting</p>

    <p><strong> Psychology Major Ambassador</strong> - Southern New Hampshire University (Aug 2024 - Present)</p>
    <p>Develop posts and events to enhance first-year psychology students' academic and social experiences</p>
    <p><strong>Server/Bartender</strong> - The Barley House (Apr 2021 - Aug 2024)</p>
    <p>Ensure customer satisfaction, prepare drinks, manage service operations</p>
    
    <p><strong>Teacher's Assistant</strong> - Children’s Central Learning Center (Jun 2019 - Aug 2019)</p>
    <p>Worked with children from infants to PreK, assisting teachers and facilitating activities...</p>
  </section>

  <section class="resume-section">
    <h2>Education</h2>
    <p><strong>Bachelor's in Child and Adolescent Psychology</strong> - Southern New Hampshire University (Aug 2023 - May 2025)</p>
    <p><strong>Early Childhood & Special Education</strong> - Arcadia University (Aug 2018 - Dec 2020)</p>
  </section>

  <section class="resume-section">
    <h2>Volunteer Work</h2>
    <p><strong>Volunteer</strong> - 21st Century Afterschool Program (Sep 2024 - Dec 2024)</p>
    <p>Assisted teachers and students with classroom management and educational activities...</p>
    
    <p><strong>Volunteer Teacher's Assistant</strong> - Gemma Services (Sep 2019 - Mar 2020)</p>
    <p>Worked with students with emotional disturbances, assisting in small group lessons...</p>
    
  </section>

  <section class="resume-section">
    <h2>Skills</h2>
    <ul>
      <li>Patient Observation</li>
      <li>Early Childhood Education</li>
      <li>Behavioral Health</li>
      <li>Customer Service</li>
      <li>Time Management</li>
      <li>Communication Skills</li>
    </ul>
  </section>

  <section class="resume-section">
    <h2>My Work</h2>
    <p>Actively conducting a study on the potential relationship between parental stress and parenting type on elementary school-aged children's screen time and executive functioning. </p> 
    <p>Completing thesis study on potential risk factors that may exist between parents with substance addictions and childhood social media addiction.</p>
    <p>Conducted study to better understand the potential impacts between music and selective attention </p>
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
