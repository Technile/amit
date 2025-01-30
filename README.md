<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Weight Loss Solutions - Amit Kumar</title>
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
      line-height: 1.6;
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

    .welcome-popup {
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
    }

    .announcement {
      background: #fff3cd;
      color: #856404;
      text-align: center;
      padding: 15px;
      font-size: 1.1rem;
      margin-top: 20px;
    }

    .feedback-slider {
      overflow: hidden;
      white-space: nowrap;
      padding: 20px 0;
      background: #fff;
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
    }

    .whatsapp-icon {
      position: fixed;
      bottom: 20px;
      right: 20px;
      z-index: 1001;
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

    /* Responsive Design */
    @media (max-width: 768px) {
      header h1 {
        font-size: 2rem;
      }

      header p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>

  <!-- Welcome Popup -->
  <div class="welcome-popup" id="welcomePopup">
    <div class="popup-content">
      <h2>Welcome to Weight Loss Solutions!</h2>
      <p>We help people lose weight even if they suffer from PCOS, PCOD, Thyroid, Blood Pressure, and more.</p>
      <button onclick="closePopup()">Thanks</button>
    </div>
  </div>

  <!-- Header Section -->
  <header>
    <h1>Amit Kumar's Weight Loss Program</h1>
    <p>Your Path to a Healthier You</p>
  </header>

  <!-- Announcement -->
  <div class="announcement">
    🎉 New Clients Get 2 Days Free Zoom Live Class Access!
  </div>

  <!-- Feedback Slider -->
  <div class="feedback-slider">
    <div>Feedback 1: "Great program, lost 10kg!"</div>
    <div>Feedback 2: "Helped me manage PCOS effectively."</div>
    <div>Feedback 3: "Best guidance for thyroid patients."</div>
    <div>Feedback 4: "Highly recommend this program."</div>
    <div>Feedback 5: "Life-changing experience!"</div>
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

  <script>
    // Close Welcome Popup
    function closePopup() {
      document.getElementById('welcomePopup').style.display = 'none';
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
