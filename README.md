
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Weight Loss Solutions - Amit Kumar</title>
  <style>
    /* General Styles */
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
      line-height: 1.6;
      overflow: hidden; /* Hide scrollbars until popup closes */
    }

    header {
      background: linear-gradient(135deg, #ff7e5f, #feb47b);
      color: white;
      text-align: center;
      padding: 50px 20px;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    .welcome-popup, .announcement-popup {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 1000;
    }

    .popup-content {
      background: white;
      padding: 30px;
      border-radius: 10px;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      animation: fadeIn 0.5s ease-in-out;
    }

    .popup-content h2 {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .popup-content button {
      background: #ff7e5f;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 1rem;
      border-radius: 5px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .popup-content button:hover {
      transform: scale(1.1);
    }

    .work-experience {
      background: #fff;
      padding: 30px;
      margin: 20px auto;
      max-width: 800px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      text-align: justify;
    }

    .feedback-slider {
      overflow: hidden;
      white-space: nowrap;
      padding: 20px 0;
      background: #fff;
      max-width: 1200px;
      margin: 0 auto;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .feedback-slider div {
      display: inline-block;
      width: 300px;
      margin-right: 20px;
      padding: 15px;
      background: #f9f9f9;
      border: 1px solid #ddd;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    .whatsapp-icon {
      position: fixed;
      bottom: 20px;
      right: 20px;
      z-index: 1001;
      animation: bounce 2s infinite;
    }

    .whatsapp-icon img {
      width: 60px;
      height: 60px;
      transition: transform 0.3s ease;
    }

    .whatsapp-icon img:hover {
      transform: scale(1.1);
    }

    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
      font-size: 0.9rem;
    }

    .disclaimer {
      text-align: center;
      color: red;
      font-weight: bold;
      animation: flash 1.5s infinite;
    }

    @keyframes flash {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.5; }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    /* Page Slide-Up Animation */
    .page-content {
      transform: translateY(100%);
      transition: transform 0.5s ease-in-out;
    }

    .page-content.active {
      transform: translateY(0);
    }
  </style>
</head>
<body>

  <!-- Welcome Popup -->
  <div class="welcome-popup" id="welcomePopup">
    <div class="popup-content">
      <h2>Welcome to Weight Loss Solutions!</h2>
      <p>We help people lose weight even if they suffer from PCOS, PCOD, Thyroid, Blood Pressure, and more.</p>
      <button onclick="closeWelcomePopup()">Thanks</button>
    </div>
  </div>

  <!-- Announcement Popup -->
  <div class="announcement-popup" id="announcementPopup" style="display: none;">
    <div class="popup-content">
      <h2>🎉 Special Announcement!</h2>
      <p>New Clients Get 2 Days Free Zoom Live Class Access!</p>
      <button onclick="closeAnnouncementPopup()">Got It</button>
    </div>
  </div>

  <!-- Main Content -->
  <div class="page-content" id="pageContent">
    <!-- Header Section -->
    <header>
      <h1>Amit Kumar's Weight Loss Program</h1>
      <p>Your Path to a Healthier You</p>
    </header>

    <!-- Work Experience Section -->
    <section class="work-experience">
      <h2>About My Work</h2>
      <p>
        With over 10 years of experience in weight management, I have helped thousands of clients achieve their fitness goals. 
        My personalized programs are designed to address specific health conditions like PCOS, PCOD, Thyroid, and Blood Pressure.
        I believe in a holistic approach that combines nutrition, exercise, and mental well-being to deliver sustainable results.
        Whether you're struggling with stubborn fat or hormonal imbalances, my tailored plans ensure safe and effective weight loss.
        I provide one-on-one consultations, live classes, and continuous support to keep you motivated.
        My mission is to empower individuals to take control of their health and lead happier, healthier lives.
      </p>
    </section>

    <!-- Feedback Slider -->
    <div class="feedback-slider">
      <div><strong>Riya Sharma:</strong> "Lost 12kg in 3 months! Best guidance ever."</div>
      <div><strong>Ajay Singh:</strong> "Helped me manage PCOS effectively."</div>
      <div><strong>Priya Patel:</strong> "Thyroid issues no longer hold me back!"</div>
      <div><strong>Rohan Mehta:</strong> "Amazing program, lost 15kg in 4 months."</div>
      <div><strong>Anjali Gupta:</strong> "Highly recommend this program."</div>
      <!-- Add more feedback here -->
    </div>

    <!-- Disclaimer -->
    <div class="disclaimer">
      Disclaimer: Results may vary from person to person depending on their physiology and efforts.
    </div>

    <!-- WhatsApp Icon -->
    <a href="https://wa.me/8210145599" target="_blank" class="whatsapp-icon">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/WhatsApp.svg/2048px-WhatsApp.svg.png" alt="WhatsApp">
    </a>

    <!-- Footer -->
    <footer>
      &copy; 2023 Amit Kumar. All Rights Reserved.
    </footer>
  </div>

  <script>
    // Close Welcome Popup and Show Announcement Popup
    function closeWelcomePopup() {
      document.getElementById('welcomePopup').style.display = 'none';
      document.getElementById('announcementPopup').style.display = 'flex';
    }

    // Close Announcement Popup and Show Page Content
    function closeAnnouncementPopup() {
      document.getElementById('announcementPopup').style.display = 'none';
      document.body.style.overflow = 'auto'; // Enable scrolling
      document.getElementById('pageContent').classList.add('active');
    }

    // Auto Slide Feedback
    const feedbackSlider = document.querySelector('.feedback-slider');
    let scrollPosition = 0;

    setInterval(() => {
      scrollPosition += 320; // Width of each feedback + margin
      if (scrollPosition > feedbackSlider.scrollWidth) {
        scrollPosition = 0;
      }
      feedbackSlider.scrollTo({
        left: scrollPosition,
        behavior: 'smooth'
      });
    }, 3000); // Change every 3 seconds
  </script>

</body>
</html>
