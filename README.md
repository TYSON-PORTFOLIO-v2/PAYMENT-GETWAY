<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TYSON HACK - Premium Subscription Plans</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --primary: #dc2626;
      --primary-dark: #b91c1c;
      --primary-light: #fef2f2;
      --accent: #1e293b;
      --text: #334155;
      --text-light: #64748b;
      --white: #ffffff;
      --gray-light: #f8fafc;
      --border: #e2e8f0;
      --success: #10b981;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #fef2f2 0%, #fff 100%);
      color: var(--text);
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 20px 16px;
    }

    .container {
      max-width: 480px;
      width: 100%;
      background: var(--white);
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
      overflow: hidden;
      margin-bottom: 30px;
    }

    .header {
      background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
      color: var(--white);
      padding: 30px 24px;
      text-align: center;
      position: relative;
    }

    .logo {
      font-size: 28px;
      font-weight: 700;
      letter-spacing: -0.5px;
      margin-bottom: 8px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
    }

    .logo i {
      font-size: 24px;
    }

    .subtitle {
      font-size: 16px;
      font-weight: 400;
      opacity: 0.9;
      margin-bottom: 5px;
    }

    .content {
      padding: 30px 24px;
    }

    .section-title {
      font-size: 18px;
      font-weight: 600;
      color: var(--accent);
      margin-bottom: 20px;
      text-align: center;
    }

    .plans {
      display: flex;
      flex-direction: column;
      gap: 16px;
      margin-bottom: 30px;
    }

    .plan-card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 20px;
      transition: all 0.3s ease;
      cursor: pointer;
      position: relative;
      overflow: hidden;
    }

    .plan-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(220, 38, 38, 0.1);
      border-color: var(--primary);
    }

    .plan-card.selected {
      border-color: var(--primary);
      background: var(--primary-light);
    }

    .plan-card h3 {
      font-size: 18px;
      font-weight: 600;
      color: var(--accent);
      margin-bottom: 5px;
    }

    .plan-card .price {
      font-size: 24px;
      font-weight: 700;
      color: var(--primary);
      margin-bottom: 5px;
    }

    .plan-card .validity {
      font-size: 14px;
      color: var(--text-light);
      margin-bottom: 10px;
    }

    .plan-card .features {
      font-size: 13px;
      color: var(--text-light);
      margin-top: 10px;
    }

    .plan-card .features ul {
      list-style-type: none;
      padding-left: 0;
    }

    .plan-card .features li {
      margin-bottom: 5px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .plan-card .features i {
      color: var(--success);
      font-size: 12px;
    }

    .highlight-badge {
      position: absolute;
      top: 15px;
      right: 15px;
      background: var(--primary);
      color: white;
      padding: 4px 10px;
      border-radius: 20px;
      font-size: 11px;
      font-weight: 600;
    }

    .contact-section {
      text-align: center;
      margin-top: 30px;
      padding-top: 20px;
      border-top: 1px solid var(--border);
    }

    .contact-btn {
      background: var(--primary);
      color: var(--white);
      padding: 14px 24px;
      border-radius: 10px;
      font-size: 16px;
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: all 0.3s ease;
      box-shadow: 0 4px 12px rgba(220, 38, 38, 0.2);
    }

    .contact-btn:hover {
      background: var(--primary-dark);
      transform: translateY(-2px);
      box-shadow: 0 6px 16px rgba(220, 38, 38, 0.3);
    }

    .footer {
      padding: 20px 24px;
      text-align: center;
      font-size: 12px;
      color: var(--text-light);
      background: var(--gray-light);
      border-top: 1px solid var(--border);
    }

    .bottom-section {
      max-width: 480px;
      width: 100%;
      background: linear-gradient(135deg, var(--accent) 0%, #334155 100%);
      border-radius: 16px;
      padding: 30px 24px;
      color: var(--white);
      text-align: center;
      margin-bottom: 20px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
    }

    .bottom-section h3 {
      font-size: 20px;
      font-weight: 600;
      margin-bottom: 15px;
    }

    .bottom-section p {
      font-size: 15px;
      margin-bottom: 20px;
      opacity: 0.9;
      line-height: 1.6;
    }

    .join-btn {
      background: var(--white);
      color: var(--accent);
      padding: 14px 28px;
      border-radius: 10px;
      font-size: 15px;
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: all 0.3s ease;
      margin-bottom: 20px;
    }

    .join-btn:hover {
      background: var(--primary-light);
      transform: translateY(-2px);
    }

    .bottom-footer {
      font-size: 12px;
      opacity: 0.7;
      line-height: 1.5;
    }

    /* Modal Styles */
    .modal {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5);
      align-items: center;
      justify-content: center;
      z-index: 1000;
      padding: 20px;
    }

    .modal-content {
      background: var(--white);
      border-radius: 16px;
      padding: 30px;
      max-width: 440px;
      width: 100%;
      text-align: left;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
      position: relative;
    }

    .close {
      position: absolute;
      top: 20px;
      right: 20px;
      font-size: 24px;
      cursor: pointer;
      color: var(--text-light);
      transition: color 0.2s;
    }

    .close:hover {
      color: var(--primary);
    }

    .modal-title {
      font-size: 22px;
      font-weight: 600;
      color: var(--accent);
      margin-bottom: 5px;
    }

    .modal-subtitle {
      font-size: 16px;
      color: var(--text-light);
      margin-bottom: 20px;
    }

    .payment-details {
      background: var(--primary-light);
      border-radius: 10px;
      padding: 20px;
      margin-bottom: 20px;
    }

    .payment-details p {
      margin-bottom: 8px;
      display: flex;
      justify-content: space-between;
    }

    .payment-details strong {
      color: var(--accent);
    }

    .upi-section {
      background: var(--gray-light);
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 20px;
      text-align: center;
    }

    .upi-id {
      font-size: 18px;
      font-weight: 700;
      color: var(--primary);
      margin: 10px 0;
      padding: 10px;
      background: var(--white);
      border-radius: 8px;
      border: 1px dashed var(--primary);
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-weight: 500;
      color: var(--accent);
    }

    .form-group input {
      width: 100%;
      padding: 14px;
      border: 1px solid var(--border);
      border-radius: 8px;
      font-size: 15px;
      transition: border 0.3s;
    }

    .form-group input:focus {
      border-color: var(--primary);
      outline: none;
      box-shadow: 0 0 0 3px rgba(220, 38, 38, 0.1);
    }

    .submit-btn {
      background: var(--primary);
      color: var(--white);
      width: 100%;
      padding: 16px;
      border: none;
      border-radius: 10px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
    }

    .submit-btn:hover {
      background: var(--primary-dark);
      transform: translateY(-2px);
    }

    .note {
      font-size: 13px;
      color: var(--text-light);
      margin-top: 15px;
      line-height: 1.5;
    }

    .transaction-id {
      font-weight: 600;
      color: var(--primary);
    }

    /* Success Message */
    .success-message {
      display: none;
      background: var(--success);
      color: white;
      padding: 12px 20px;
      border-radius: 8px;
      margin-bottom: 20px;
      text-align: center;
    }

    /* Responsive */
    @media (max-width: 480px) {
      .container {
        border-radius: 16px;
      }
      
      .header {
        padding: 24px 20px;
      }
      
      .content {
        padding: 24px 20px;
      }
      
      .modal-content {
        padding: 24px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <div class="logo">
        <i class="fas fa-shield-alt"></i>
        TYSON HACK
      </div>
      <div class="subtitle">Premium Subscription Plans</div>
    </div>
    
    <div class="content">
      <h2 class="section-title">Select Your Plan</h2>
      
      <div class="plans">
        <div class="plan-card" data-plan="PRO PLAN" data-price="999" data-validity="7 Days">
          <div class="highlight-badge">MOST POPULAR</div>
          <h3>PRO PLAN</h3>
          <div class="price">₹999</div>
          <div class="validity">Valid for 7 Days</div>
          <div class="features">
            <ul>
              <li><i class="fas fa-check"></i> Full access to all features</li>
              <li><i class="fas fa-check"></i> Priority customer support</li>
              <li><i class="fas fa-check"></i> Advanced analytics</li>
            </ul>
          </div>
        </div>
        
        <div class="plan-card" data-plan="ULTIMATE PLAN" data-price="1499" data-validity="30 Days">
          <div class="highlight-badge">BEST VALUE</div>
          <h3>ULTIMATE PLAN</h3>
          <div class="price">₹1499</div>
          <div class="validity">Valid for 30 Days</div>
          <div class="features">
            <ul>
              <li><i class="fas fa-check"></i> All PRO features included</li>
              <li><i class="fas fa-check"></i> Exclusive premium tools</li>
              <li><i class="fas fa-check"></i> 24/7 dedicated support</li>
            </ul>
          </div>
        </div>
      </div>
      
      <div class="contact-section">
        <a href="https://t.me/TYSON_OWNER" target="_blank" class="contact-btn">
          <i class="fas fa-headset"></i> Contact Support
        </a>
      </div>
    </div>
    
    <div class="footer">
      © 2025 TYSON HACK. All rights reserved.
    </div>
  </div>

  <div class="bottom-section">
    <h3>Launch Your Prediction Journey</h3>
    <p>Join TYSON HACK and unlock the power of AI-driven insights for better decision making.</p>
    <a href="https://t.me/TYSON_OK_WIN_HACK" target="_blank" class="join-btn">
      <i class="fas fa-users"></i> Join Our Community
    </a>
    <div class="bottom-footer">
      TYSON HACK is designed for educational and informational purposes.<br>
      Use at your own discretion. © 2025 TYSON HACK.
    </div>
  </div>

  <!-- Payment Modal -->
  <div id="paymentModal" class="modal">
    <div class="modal-content">
      <span class="close">&times;</span>
      <h3 class="modal-title">Complete Your Payment</h3>
      <p class="modal-subtitle">Follow the instructions below to complete your purchase</p>
      
      <div class="success-message" id="successMessage">
        <i class="fas fa-check-circle"></i> Payment submitted successfully!
      </div>
      
      <div class="payment-details">
        <p><span>Selected Plan:</span> <strong id="modalPlan"></strong></p>
        <p><span>Amount:</span> <strong id="modalPrice"></strong></p>
        <p><span>Validity:</span> <strong id="modalValidity"></strong></p>
        <p><span>Transaction ID:</span> <strong class="transaction-id" id="transactionId"></strong></p>
      </div>
      
      <div class="upi-section">
        <p>Please use the following UPI ID to complete your payment:</p>
        <div class="upi-id" id="upiIdDisplay">legendxowner@ybl</div>
        <p>If the UPI app doesn't open automatically, please copy this ID and paste it in your payment app.</p>
      </div>
      
      <div class="form-group">
        <label for="utrInput">UTR Number <small>(After completing payment)</small></label>
        <input type="text" id="utrInput" placeholder="Enter your UTR number">
        <div class="note">Your UTR number is a 10-20 digit reference number provided by your bank after successful payment.</div>
      </div>
      
      <button class="submit-btn" onclick="submitPayment()">
        <i class="fas fa-paper-plane"></i> Submit Payment Details
      </button>
      
      <div class="note">
        <strong>Note:</strong> Your payment will be verified by our team within 24 hours. Please save your Transaction ID for reference.
      </div>
    </div>
  </div>

  <script>
    // DOM Elements
    const modal = document.getElementById('paymentModal');
    const closeBtn = document.querySelector('.close');
    const planCards = document.querySelectorAll('.plan-card');
    const modalPlan = document.getElementById('modalPlan');
    const modalPrice = document.getElementById('modalPrice');
    const modalValidity = document.getElementById('modalValidity');
    const utrInput = document.getElementById('utrInput');
    const upiIdDisplay = document.getElementById('upiIdDisplay');
    const transactionIdDisplay = document.getElementById('transactionId');
    const successMessage = document.getElementById('successMessage');

    // Constants
    const upiId = 'legendxowner@ybl';
    const merchantName = 'TYSON HACK';

    // Generate a transaction ID
    function generateTransactionId() {
      return 'TXN' + Math.random().toString(36).substr(2, 9).toUpperCase();
    }

    // Plan selection
    planCards.forEach(card => {
      card.addEventListener('click', () => {
        // Remove selected class from all cards
        planCards.forEach(c => c.classList.remove('selected'));
        // Add selected class to clicked card
        card.classList.add('selected');
        
        const plan = card.getAttribute('data-plan');
        const price = card.getAttribute('data-price');
        const validity = card.getAttribute('data-validity');
        const transactionId = generateTransactionId();

        // Update modal content
        modalPlan.textContent = plan;
        modalPrice.textContent = `₹${price}`;
        modalValidity.textContent = validity;
        upiIdDisplay.textContent = upiId;
        transactionIdDisplay.textContent = transactionId;

        // Reset form
        utrInput.value = '';
        successMessage.style.display = 'none';

        // Open UPI app
        const upiLink = `upi://pay?pa=${upiId}&pn=${encodeURIComponent(merchantName)}&am=${price}&cu=INR&tn=Payment for ${plan} - ${transactionId}`;
        window.location.href = upiLink;

        // Show modal
        modal.style.display = 'flex';
      });
    });

    // Close modal
    closeBtn.addEventListener('click', () => {
      modal.style.display = 'none';
      utrInput.value = '';
    });

    // Close modal when clicking outside
    window.addEventListener('click', (e) => {
      if (e.target === modal) {
        modal.style.display = 'none';
        utrInput.value = '';
      }
    });

    // Submit payment
    function submitPayment() {
      const plan = modalPlan.textContent;
      const price = modalPrice.textContent.replace('₹', '');
      const utr = utrInput.value.trim();
      const transactionId = transactionIdDisplay.textContent;

      // Validate UTR
      if (!utr || !/^[A-Za-z0-9]{10,20}$/.test(utr)) {
        alert('Please enter a valid UTR number (10–20 alphanumeric characters).');
        utrInput.focus();
        return;
      }

      // Show success message
      successMessage.style.display = 'block';
      
      // Prepare and send Telegram message
      const message = `New Payment Received!%0A%0ATransaction ID: ${transactionId}%0APlan: ${plan}%0APrice: ₹${price}%0AUTR: ${utr}%0A%0A~Please verify the payment. Thank you!`;
      const telegramUrl = `https://t.me/TYSON_OWNER?text=${encodeURIComponent(message)}`;
      window.open(telegramUrl, '_blank');

      // Reset form after delay
      setTimeout(() => {
        modal.style.display = 'none';
        utrInput.value = '';
        planCards.forEach(c => c.classList.remove('selected'));
      }, 3000);
    }
  </script>
</body>
</html>
