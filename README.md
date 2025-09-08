<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css" integrity="sha512-2SwdPD6INVrV/lHTZbO2nodKhrnDdJK9/kg2XD1r9uGqPo1cUbujc+IYdlYdEErWNu69gVcYgdxlmVmzTWnetw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <title>Footer Example</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: #000;
      background: #fff;
    }
    footer {
      display: flex;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: 40px auto 60px;
      padding: 0 20px;
      gap: 40px;
      justify-content: flex-start;
    }

    /* Each footer column container */
    .footer-column {
      min-width: 140px;
      flex: 1 1 140px;
      display: flex;
      flex-direction: column;
    }

    /* The last column with sign-up text */
    .footer-signup {
      flex: 2 1 280px;
      max-width: 320px;
      font-size: 14px;
      line-height: 1.5;
    }

    /* Headings for columns */
    .footer-column h3 {
      margin: 0 0 16px 0;
      font-weight: 700;
      font-size: 16px;
    }

    /* Lists in columns */
    .footer-column ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }
    .footer-column li {
      margin-bottom: 10px;
      font-weight: 400;
      font-size: 14px;
      cursor: default;
      user-select: none;
    }

    /* Link style for READ MORE */
    .footer-signup a {
      color: #000;
      font-weight: 600;
      text-decoration: underline;
      cursor: pointer;
    }
    .footer-signup a:hover,
    .footer-signup a:focus {
      color: #444;
      outline: none;
    }

    /* Responsive adjustment */
    @media (max-width: 680px) {
      footer {
        flex-direction: column;
        gap: 30px;
        margin: 20px auto 40px;
      }
      .footer-column, .footer-signup {
        max-width: 100%;
        flex: none;
      }
    }
    .menu {
  display: flex;
  justify-content: space-between;
}

.menu-item {
  position: relative;
  padding: 10px 20px;
}

.toggle-btn {
  display: none;
  background: none;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
}

/* Dropdown content hidden by default */
.dropdown-content {
  display: none;
  position: absolute;
  top: 40px;
  left: 0;
  background: #f9f9f9;
  padding: 10px;
  border: 1px solid #ccc;
  z-index: 10;
}

/* Show dropdown when "active" */
.menu-item.active .dropdown-content {
  display: block;
}
.menu{
  display: none;
}
/* Media Query for smaller than 1020px */
@media (max-width: 1020px) {
  footer{
    display: none;
  }
  .menu {
    display: block;
    flex-direction: column;
  }

  .menu-item {
    border-bottom: 1px solid #ddd;
  }

  .toggle-btn {
    display: inline-block;
    float: right;
  }

  /* Hide dropdown content initially */
  .dropdown-content {
    position: static;
    border: none;
    background: transparent;
    padding: 10px 0 0 0;
  }
}
.section5{
  display: flex;
  justify-content: space-between;
  gap: 10px;
}
  @media (max-width: 560px) {
  .section5{
    display: block;
  }
}
  </style>
</head>
<body>
  <footer>
    <div class="footer-column">
      <h3>Shop</h3>
      <ul>
        <li>LADIES</li>
        <li>MEN</li>
        <li>KIDS</li>
        <li>HOME</li>
      </ul>
    </div>
    <div class="footer-column">
      <h3>Corporate Info</h3>
      <ul>
        <li>CAREER AT H&amp;M</li>
        <li>ABOUT H&amp;M GROUP</li>
        <li>SUSTAINABILITY H&amp;M GROUP</li>
        <li>PRESS</li>
        <li>INVESTOR RELATIONS</li>
        <li>CORPORATE GOVERNANCE</li>
      </ul>
    </div>
    <div class="footer-column">
      <h3>Help</h3>
      <ul>
        <li>CUSTOMER SERVICE</li>
        <li>MY H&amp;M</li>
        <li>FIND A STORE</li>
        <li>LEGAL &amp; PRIVACY</li>
        <li>CONTACT</li>
        <li>SECURE SHOPPING</li>
        <li>COOKIE NOTICE</li>
        <li>COOKIE SETTINGS</li>
      </ul>
    </div>
    <div class="footer-signup">
      <p>Sign up now and be the first to know about exclusive offers, latest fashion news &amp; style tips!</p>
      <p><a href="#" aria-label="Read more about exclusive offers, latest fashion news, and style tips">READ MORE</a></p>
    </div>
  </footer>
  <div class="menu">
  <div class="menu-item">
    <span class="title">SHOP</span>
    <button class="toggle-btn">+</button>
    <div class="dropdown-content">
      <!-- Your dropdown content here -->
      <p>LADIES</p>
      <p>MEN</p>
      <p>KIDS</p>
      <p>HOME</p>
    </div>
  </div>

  <div class="menu-item">
    <span class="title">CORPORATE INFO</span>
    <button class="toggle-btn">+</button>
    <div class="dropdown-content">
      <!-- Your dropdown content here -->
      <p>CAREER AT H&M</p>
      <p>SUSTAINABILITY H&M GROUP</p>
      <p>ABOUT H&M GROUP</p>
      <p>SUSTAINABILITY H&M GROUP</p>
      <p>PRESS</p>
      <p>INVESTOR RELATIONS</p>
      <p>CORPORATE GOVERNANCE</p>
    </div>
  </div>

  <div class="menu-item">
    <span class="title">HELP</span>
    <button class="toggle-btn">+</button>
    <div class="dropdown-content">
      <!-- Your dropdown content here -->
      <p>CUSTOMER SERVICE</p>
      <p>MY H&M</p>
      <p>FIND A STORE</p>
      <p>LEGAL & PRIVACY</p>
      <p>CONTACT</p>
      <p>SECURE SHOPPING</p>
      <p>COOKIE NOTICE</p>
      <p>COOKIE SETTINGS</p>
    </div>
  </div>
</div>
<div class="section4">
  <img src="images/438-4383499_free-hbo-logo-transparent-black-h-m-logo-removebg-preview.png" alt="" style="width: 70px; padding: 10px; padding-top: 50px;">
  <p style="padding: 10px;">INDIA (Rs.) <a href="" style="padding-left: 5PX;">CHANGE REGION</a></p>
</div>
<div class="section5" style="padding: 10px;">
  <div>
    <p>The content of this site is copyright-protected and is the property of H & M Hennes & Mauritz AB.</p>
  </div>
  <div>
    <ul style="list-style: none; display: flex; gap: 20px; padding: 10px;">
      <li><i class="fa-brands fa-instagram"></i></li>
      <li><i class="fa-brands fa-tiktok"></i></li>
      <li><i class="fa-brands fa-spotify"></i></li>
      <li><i class="fa-brands fa-youtube"></i></li>
      <li><i class="fa-brands fa-pinterest"></i></li>
      <li><i class="fa-brands fa-square-facebook"></i></li>
    </ul>
  </div>
</div>
<script>
  document.querySelectorAll('.toggle-btn').forEach(button => {
  button.addEventListener('click', () => {
    const menuItem = button.parentElement;
    menuItem.classList.toggle('active');
  });
});
</script>
</body>
</html>
