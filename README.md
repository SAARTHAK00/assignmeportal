<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Saarthak Kudiyal - Assignments</title>
  <style>
    :root {
      --primary-color: #3F51B5;
      --secondary-color: #7986CB;
      --accent-color: #FF4081;
      --text-color: #424242;
      --bg-color: #E8EAF6;
      --card-bg: #ffffff;
    }

    body {
      font-family: 'Poppins', 'Arial', sans-serif;
      line-height: 1.7;
      color: var(--text-color);
      margin: 0;
      padding: 0;
      background-color: var(--bg-color);
    }

    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 0 20px;
    }

    header {
      background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
      color: white;
      padding: 40px 0;
      text-align: center;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
      letter-spacing: 1px;
    }

    header p {
      margin: 10px 0 0;
      font-size: 1.2rem;
      opacity: 0.9;
    }

    .student-profile {
      background-color: var(--card-bg);
      border-radius: 12px;
      padding: 25px;
      margin: -25px auto 30px;
      max-width: 800px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
      position: relative;
      border-left: 5px solid var(--accent-color);
    }

    .main-content {
      background-color: var(--card-bg);
      border-radius: 12px;
      padding: 30px;
      margin-bottom: 30px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
      text-align: center;
    }

    h2 {
      color: var(--primary-color);
      position: relative;
      padding-bottom: 10px;
      margin-top: 0;
    }

    h2::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 50px;
      height: 3px;
      background-color: var(--accent-color);
    }

    .assignment-button {
      display: inline-block;
      padding: 15px 25px;
      font-size: 1rem;
      font-weight: 600;
      color: white;
      background-color: var(--primary-color);
      border-radius: 10px;
      text-decoration: none;
      transition: background-color 0.3s;
      margin-top: 20px;
    }

    .assignment-button:hover {
      background-color: var(--secondary-color);
    }

    footer {
      background-color: var(--primary-color);
      color: white;
      text-align: center;
      padding: 15px 0;
      margin-top: 30px;
      border-radius: 12px;
    }

    #grade-bar {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 18px;
      background-color: #ffffff;
      border: 2px solid #3F51B5;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      font-family: 'Poppins', sans-serif;
      font-size: 15px;
      color: #3F51B5;
      font-weight: 600;
      z-index: 9999;
    }
  </style>
</head>
<body>
  <header>
    <div class="container">
      <h1>Saarthak Kudiyal</h1>
      <p>Information Management Systems</p>
    </div>
  </header>

  <div class="container">
    <section class="student-profile">
      <h2>About Me</h2>
      <p>
        <strong>Student ID:</strong> 2417632<br>
        <strong>University:</strong> Dong-A University<br>
        <strong>Department:</strong> Integrated Business Management
      </p>
    </section>

    <main class="main-content">
      <h2>Assignments</h2>
      <a href="https://drive.google.com/drive/folders/14iWDTLV-28TxzduObKtcng0zCyJuS3NV?usp=drive_link" class="assignment-button" target="_blank">📂 Open Assignments Folder</a>
    </main>
  </div>

  <div class="container">
    <footer>
      &copy; 2025 Saarthak Kudiyal - Dong-A University
    </footer>
  </div>

  <!-- Grade Display -->
  <div id="grade-bar">🎓 Grade: <span id="grade">Loading...</span>%</div>

  <!-- Grade Fetch Script -->
  <script>
    fetch("https://script.google.com/macros/s/AKfycbygySpoqdNcUVNZ8TuFwMKGP6Ofu9axR382C13prSA/dev/ecex")
      .then(response => {
        if (!response.ok) {
          throw new Error('Network response was not ok');
        }
        return response.text();
      })
      .then(grade => {
        document.getElementById("grade").innerText = grade;
      })
      .catch(error => {
        console.error("Grade fetch failed:", error);
        document.getElementById("grade").innerText = "Error";
      });
    
  </script>
  < fetch > </fetch>
</body>
</html>
