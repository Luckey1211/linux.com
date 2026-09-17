<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Microsoft Hackathon 2026</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333;
    }
    header {
      background-color: #0078d4;
      color: #fff;
      padding: 2.5rem 1rem;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.2rem;
    }
    main {
      padding: 2rem;
      max-width: 750px;
      margin: 2rem auto;
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }
    h2 {
      color: #0078d4;
      border-bottom: 2px solid #eee;
      padding-bottom: 8px;
      margin-top: 2rem;
    }
    .details-list {
      list-style: none;
      padding: 0;
      margin: 0;
    }
    .details-list li {
      padding: 12px 0;
      border-bottom: 1px solid #eee;
      display: flex;
      justify-content: space-between;
    }
    .label {
      font-weight: 600;
      color: #555;
    }
    .value {
      font-weight: 500;
      color: #222;
    }
    .prizes {
      display: flex;
      gap: 15px;
      margin-top: 1rem;
      flex-wrap: wrap;
    }
    .prize-card {
      flex: 1;
      min-width: 180px;
      padding: 1.2rem;
      background: #f9f9fb;
      border: 1px solid #e0e0e0;
      border-radius: 8px;
      text-align: center;
    }
    .prize-card.gold { border-top: 4px solid #d4af37; }
    .prize-card.silver { border-top: 4px solid #a8a8a8; }
    .prize-card.bronze { border-top: 4px solid #cd7f32; }
    .prize-title {
      font-size: 1.1rem;
      font-weight: bold;
      margin-bottom: 6px;
    }
    .prize-amount {
      font-size: 1.4rem;
      font-weight: bold;
      color: #107c10;
      margin-bottom: 6px;
    }
    .prize-extra {
      font-size: 0.9rem;
      color: #666;
    }
    /* Form Styles */
    .form-group {
      margin-bottom: 1.2rem;
    }
    .form-group label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
      color: #444;
    }
    .form-group input, .form-group select {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
      font-size: 1rem;
    }
    .payment-box {
      background: #eef6fc;
      border: 1px dashed #0078d4;
      padding: 15px;
      border-radius: 6px;
      margin-bottom: 1.5rem;
    }
    .submit-btn {
      display: block;
      width: 100%;
      padding: 1rem;
      background-color: #107c10;
      color: #fff;
      border: none;
      border-radius: 6px;
      font-size: 1.2rem;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.2s;
    }
    .submit-btn:hover {
      background-color: #0b5a0b;
    }
    .success-msg {
      display: none;
      background: #d4edda;
      color: #155724;
      padding: 15px;
      border-radius: 5px;
      margin-top: 15px;
      text-align: center;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <header>
    <h1>Microsoft Hackathon 2026</h1>
  </header>

  <main>
    <h2>Event Details</h2>
    <ul class="details-list">
      <li><span class="label">Date:</span> <span class="value">20 September 2026</span></li>
      <li><span class="label">Center / Location:</span> <span class="value">Dehradun</span></li>
      <li><span class="label">Registration Fee:</span> <span class="value">₹100</span></li>
      <li><span class="label">ID Card Release:</span> <span class="value">24 Hours before the event</span></li>
      <li><span class="label">Perks:</span> <span class="value">Certificate of Participation for all</span></li>
    </ul>

    <h2>Prize Pool</h2>
    <div class="prizes">
      <div class="prize-card gold">
        <div class="prize-title">1st Prize</div>
        <div class="prize-amount">₹1,60,000</div>
        <div class="prize-extra">+ Certificate of Merit</div>
      </div>
      <div class="prize-card silver">
        <div class="prize-title">2nd Prize</div>
        <div class="prize-amount">₹1,00,000</div>
        <div class="prize-extra">+ Certificate of Merit</div>
      </div>
      <div class="prize-card bronze">
        <div class="prize-title">3rd Prize</div>
        <div class="prize-amount">₹50,000</div>
        <div class="prize-extra">+ Certificate of Merit</div>
      </div>
    </div>

    <h2>Register for Hackathon</h2>
    <form id="regForm" onsubmit="event.preventDefault(); document.getElementById('success').style.display = 'block';">
      <div class="form-group">
        <label>Full Name</label>
        <input type="text" placeholder="Enter your full name" required>
      </div>

      <div class="form-group">
        <label>Email Address</label>
        <input type="email" placeholder="example@mail.com" required>
      </div>

      <div class="form-group">
        <label>Phone / WhatsApp Number</label>
        <input type="tel" placeholder="+91 XXXXX XXXXX" required>
      </div>

      <div class="form-group">
        <label>College / Organization</label>
        <input type="text" placeholder="Enter college or company name" required>
      </div>

      <div class="payment-box">
        <strong>Fee Payment: ₹100</strong>
        <p style="margin: 6px 0 0; font-size: 0.9rem; color: #555;">
          UPI ID: <strong>your-upi-id@okhdfcbank</strong> (Yahan apni UPI ID replace karein)
        </p>
      </div>

      <div class="form-group">
        <label>UPI Transaction ID / UTR</label>
        <input type="text" placeholder="Enter 12-digit transaction ID" required>
      </div>

      <button type="submit" class="submit-btn">Complete Registration (₹100)</button>
    </form>

    <div id="success" class="success-msg">
      Registration submitted successfully! Your ID card will be issued 24 hours prior to the event.
    </div>
  </main>

</body>
</html>
