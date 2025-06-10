
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
      margin: 20px 10px 0;
    }

    .assignment-button:hover {
      background-color: var(--secondary-color);
    }

    .hif-lumen-button {
      background-color: #FF9800;
    }

    .hif-lumen-button:hover {
      background-color: #F57C00;
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

    /* Modal Styles */
    .modal {
      display: none;
      position: fixed;
      z-index: 10000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0,0,0,0.6);
    }

    .modal-content {
      background-color: var(--card-bg);
      margin: 15% auto;
      padding: 30px;
      border-radius: 12px;
      width: 300px;
      text-align: center;
      box-shadow: 0 5px 20px rgba(0,0,0,0.2);
      animation: modalIn 0.3s ease;
    }

    @keyframes modalIn {
      from {transform: translateY(-50px); opacity: 0;}
      to {transform: translateY(0); opacity: 1;}
    }

    .modal h3 {
      color: var(--primary-color);
      margin-top: 0;
    }

    .modal input {
      width: 100%;
      padding: 12px;
      margin: 15px 0;
      border: 1px solid #ddd;
      border-radius: 6px;
      box-sizing: border-box;
      font-size: 16px;
      text-align: center;
    }

    .modal-buttons {
      display: flex;
      justify-content: space-between;
      margin-top: 20px;
    }

    .modal-button {
      padding: 10px 20px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-weight: 600;
      transition: all 0.3s;
      flex: 0 0 48%;
    }

    .cancel-button {
      background-color: #e0e0e0;
      color: #555;
    }

    .cancel-button:hover {
      background-color: #d0d0d0;
    }

    .submit-button {
      background-color: var(--accent-color);
      color: white;
    }

    .submit-button:hover {
      background-color: #e91e63;
    }

    .error-message {
      color: #f44336;
      margin-top: 10px;
      font-size: 14px;
      display: none;
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
      <a href="https://drive.google.com/drive/folders/14iWDTLV-28TxzduObKtcng0zCyJuS3NV?usp=drive_link" class="Virtual Library-button" target="_blank">📂 Open r</a>
      <a href="#" class="assignment-button hif-lumen-button" id="hifLumenBtn">🔒 Hif Lumen</a>
      <a href="https://2417735.github.io/crypterror/" class="assignment-button" id="pressEnterBtn" target="_blank">🛠️ Press Enter</a>
    </main>
  </div>

  <div class="container">
    <footer>
      &copy; 2025 Saarthak Kudiyal - Dong-A University
    </footer>
  </div>

  <div id="grade-bar">🎓 Grade: <span id="grade">Loading...</span>%</div>

  <!-- Password Modal -->
  <div id="passwordModal" class="modal">
    <div class="modal-content">
      <h3>Protected Link</h3>
      <p>Please enter the passcode to access Hif Lumen</p>
      <input type="password" id="passwordInput" placeholder="Enter passcode">
      <div id="errorMessage" class="error-message">Incorrect passcode. Please try again.</div>
      <div class="modal-buttons">
        <button class="modal-button cancel-button" id="cancelBtn">Cancel</button>
        <button class="modal-button submit-button" id="submitBtn">Submit</button>
      </div>
    </div>
  </div>

  <!-- Scripts -->
  <script>
    // Grade fetch script
    fetch("https://script.google.com/macros/s/AKfycbygySpoqdNcUVNZ8TuFwMKGP6Ofu9axR382C13prSA/dev/ecex")
      .then(response => {
        if (!response.ok) throw new Error('Network response was not ok');
        return response.text();
      })
      .then(grade => {
        document.getElementById("grade").innerText = grade;
      })
      .catch(error => {
        console.error("Grade fetch failed:", error);
        document.getElementById("grade").innerText = "Error";
      });

    // Hif Lumen password protection
    document.addEventListener('DOMContentLoaded', function() {
      const modal = document.getElementById('passwordModal');
      const hifLumenBtn = document.getElementById('hifLumenBtn');
      const cancelBtn = document.getElementById('cancelBtn');
      const submitBtn = document.getElementById('submitBtn');
      const passwordInput = document.getElementById('passwordInput');
      const errorMessage = document.getElementById('errorMessage');

      const correctPasscode = '1234';
      const protectedUrl = 'https://chatgpt.com/share/682c90ea-bcec-8001-a6ad-3ddf11eb3ddf';

      hifLumenBtn.addEventListener('click', function(e) {
        e.preventDefault();
        modal.style.display = 'block';
        passwordInput.value = '';
        errorMessage.style.display = 'none';
      });

      cancelBtn.addEventListener('click', function() {
        modal.style.display = 'none';
      });

      submitBtn.addEventListener('click', function() {
        checkPassword();
      });

      passwordInput.addEventListener('keyup', function(e) {
        if (e.key === 'Enter') checkPassword();
      });

      window.addEventListener('click', function(e) {
        if (e.target === modal) modal.style.display = 'none';
      });

      function checkPassword() {
        if (passwordInput.value === correctPasscode) {
          window.open(protectedUrl, '_blank');
          modal.style.display = 'none';
        } else {
          errorMessage.style.display = 'block';
          passwordInput.value = '';
          passwordInput.focus();
        }
      }
    });
  </script>
</body>
</html>
