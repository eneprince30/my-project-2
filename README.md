<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>University of Calabar - Result Portal</title>
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link rel="stylesheet" href="form.css">
</head>
<body>

  <div class="card">
    <!-- Header Section -->
    <div class="card-header">
      <div class="logo-container">
        <!-- Replace src with actual logo link if needed -->
        <img src="https://unical.edu.ng/wp-content/uploads/2021/04/unical-logo.png" alt="University of Calabar Logo">
      </div>
      <h2>UNIVERSITY OF CALABAR</h2>
      <p class="subtitle">RESULT PORTAL</p>
    </div>

    <!-- Form Section -->
    <div class="card-body">
      <form action="#" method="POST">
        
        <!-- Matriculation Number -->
        <div class="form-group">
          <label for="matric">MATRICULATION NUMBER</label>
          <div class="input-wrapper">
            <i class="fa-solid fa-id-card input-icon"></i>
            <input type="text" id="matric" placeholder="e.g. CC/20/0001">
          </div>
        </div>

        <!-- JAMB Registration Number -->
        <div class="form-group">
          <label for="jamb">JAMB REGISTRATION NUMBER</label>
          <div class="input-wrapper">
            <i class="fa-solid fa-hashtag input-icon"></i>
            <input type="text" id="jamb" placeholder="e.g. 12345678AB">
          </div>
        </div>

        <!-- Access PIN -->
        <div class="form-group">
          <label for="pin">ACCESS PIN</label>
          <div class="input-wrapper">
            <i class="fa-solid fa-lock input-icon"></i>
            <input type="password" id="pin" placeholder="Enter your pin">
          </div>
        </div>

        <!-- Radio Selection Buttons -->
        <div class="student-type-group">
          <label class="btn-option">
            <input type="radio" name="student_type" value="new">
            <span><i class="fa-solid fa-user-plus"></i> NEW STUDENT</span>
          </label>
          <label class="btn-option">
            <input type="radio" name="student_type" value="returning">
            <span><i class="fa-solid fa-rotate-right"></i> RETURNING</span>
          </label>
        </div>

        <!-- Submit Button -->
        <button type="submit" class="login-btn">
          <i class="fa-solid fa-right-to-bracket"></i> LOGIN
        </button>

      </form>
    </div>

    <!-- Card Footer -->
    <div class="card-footer">
      <a href="#" class="footer-link green"><i class="fa-solid fa-key"></i> Don't have a pin? Get one here</a>
      <a href="#" class="footer-link gray"><i class="fa-solid fa-arrows-rotate"></i> Change Pin</a>
    </div>
  </div>

</body>
</html>


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
}

body {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: radial-gradient(circle at 80% 20%, #1d1b4b 0%, #12102e 50%, #0d1a2d 100%);
  padding: 20px;
}

/* Card Container */
.card {
  width: 100%;
  max-width: 380px;
  background-color: rgba(30, 27, 60, 0.85);
  border-radius: 20px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  overflow: hidden;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(10px);
}

/* Header Gradient */
.card-header {
  background: linear-gradient(135deg, #a200ff 0%, #00b493 100%);
  padding: 25px 20px 20px;
  text-align: center;
  color: #ffffff;
}

.logo-container {
  width: 70px;
  height: 70px;
  background-color: #ffffff;
  border-radius: 50%;
  margin: 0 auto 12px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

.logo-container img {
  width: 85%;
  height: 85%;
  object-fit: contain;
}

.card-header h2 {
  font-size: 15px;
  font-weight: 700;
  letter-spacing: 1.2px;
  margin-bottom: 4px;
}

.subtitle {
  font-size: 11px;
  letter-spacing: 1.5px;
  opacity: 0.9;
  font-weight: 500;
}

/* Form Body */
.card-body {
  padding: 24px 20px 15px;
}

.form-group {
  margin-bottom: 16px;
}

.form-group label {
  display: block;
  color: #a3a8c3;
  font-size: 10.5px;
  font-weight: 600;
  letter-spacing: 0.8px;
  margin-bottom: 6px;
}

.input-wrapper {
  position: relative;
  display: flex;
  align-items: center;
}

.input-icon {
  position: absolute;
  left: 14px;
  color: #6c7293;
  font-size: 13px;
}

.input-wrapper input {
  width: 100%;
  background-color: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: 8px;
  padding: 12px 12px 12px 38px;
  color: #ffffff;
  font-size: 13px;
  outline: none;
  transition: all 0.3s ease;
}

.input-wrapper input::placeholder {
  color: #5c6280;
}

.input-wrapper input:focus {
  border-color: #00b493;
  background-color: rgba(255, 255, 255, 0.08);
}

/* Student Type Radio Options */
.student-type-group {
  display: flex;
  gap: 10px;
  margin-top: 20px;
  margin-bottom: 20px;
}

.btn-option {
  flex: 1;
  cursor: pointer;
}

.btn-option input {
  display: none;
}

.btn-option span {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  padding: 10px 0;
  background-color: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: 8px;
  color: #a3a8c3;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.5px;
  transition: all 0.2s ease;
}

.btn-option input:checked + span {
  background-color: rgba(255, 255, 255, 0.15);
  border-color: #00b493;
  color: #ffffff;
}

/* Login Button */
.login-btn {
  width: 100%;
  padding: 12px;
  border: none;
  border-radius: 8px;
  background: linear-gradient(90deg, #8a00d4 0%, #00b493 100%);
  color: #ffffff;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 1px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  transition: opacity 0.3s ease, transform 0.1s ease;
}

.login-btn:hover {
  opacity: 0.92;
}

.login-btn:active {
  transform: scale(0.99);
}

/* Footer Section */
.card-footer {
  padding: 15px 20px;
  border-top: 1px solid rgba(255, 255, 255, 0.06);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-link {
  font-size: 11px;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 5px;
}

.footer-link.green {
  color: #00e6a8;
}

.footer-link.gray {
  color: #7b83a0;
}

.footer-link:hover {
  text-decoration: underline;
}
