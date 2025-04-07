<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Professional Service Page</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #ffffff, #f0f0f0);
    }
    header {
      background-color: #0066cc;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .container {
      padding: 2rem;
    }
    .services {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
    }
    .card {
      background: #ffffff;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      padding: 1rem;
      width: 250px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }
    .card:hover {
      transform: scale(1.05);
    }
    .card h3 {
      margin-top: 0;
    }
    .hidden {
      display: none;
    }
    .details {
      background-color: #fff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      margin-top: 2rem;
    }
    .form-control {
      margin: 0.5rem 0;
    }
    .form-control input {
      width: 100%;
      padding: 0.5rem;
      border-radius: 4px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #0066cc;
      color: white;
      padding: 0.7rem 1.5rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 1rem;
    }
    footer {
      position: fixed;
      bottom: 20px;
      right: 20px;
    }
    .whatsapp-button {
      background-color: #25D366;
      color: white;
      padding: 10px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <header>
    <h1>Saurav Paswan - Professional Services</h1>
  </header>
  <div class="container">
    <div class="services">
      <div class="card" onclick="showDetails('app')">
        <h3>App Development</h3>
        <p>Build mobile apps for Android & iOS</p>
      </div>
      <div class="card" onclick="showDetails('web')">
        <h3>Web Development</h3>
        <p>Responsive, Modern Websites</p>
      </div>
      <div class="card" onclick="showDetails('ai')">
        <h3>AI Solutions</h3>
        <p>Custom AI-powered tools & apps</p>
      </div>
      <div class="card" onclick="showDetails('tools')">
        <h3>Tool Development</h3>
        <p>Unique utilities for personal or business use</p>
      </div>
    </div><div class="details hidden" id="detailSection">
  <h2 id="serviceTitle"></h2>
  <p id="serviceDescription"></p>
  <p id="servicePrice"></p>
  <div class="form-control">
    <label>Name:</label>
    <input type="text" id="name" required>
  </div>
  <div class="form-control">
    <label>Email:</label>
    <input type="email" id="email" required>
  </div>
  <div class="form-control">
    <label>Phone:</label>
    <input type="text" id="phone" required>
  </div>
  <button onclick="sendWhatsApp()">Book Now on WhatsApp</button>
</div>

  </div>  <footer>
    <a class="whatsapp-button" href="tel:7559347682">Customer Support</a>
  </footer>  <script>
    const services = {
      app: {
        title: "App Development",
        description: "We build modern, scalable mobile applications for Android and iOS.",
        price: "Basic: ₹3000 | Medium: ₹6000 | High: ₹10,000+"
      },
      web: {
        title: "Web Development",
        description: "Custom websites for businesses, portfolios and startups.",
        price: "Basic: ₹2000 | Medium: ₹5000 | High: ₹9000+"
      },
      ai: {
        title: "AI Solutions",
        description: "Build intelligent bots, AI tools and automations.",
        price: "Basic: ₹4000 | Medium: ₹8000 | High: ₹15000+"
      },
      tools: {
        title: "Tool Development",
        description: "Need a special software or script? We build tools for automation & utility.",
        price: "Basic: ₹1000 | Medium: ₹3000 | High: ₹7000+"
      }
    };

    function showDetails(type) {
      const detail = services[type];
      document.getElementById("detailSection").classList.remove("hidden");
      document.getElementById("serviceTitle").innerText = detail.title;
      document.getElementById("serviceDescription").innerText = detail.description;
      document.getElementById("servicePrice").innerText = "Pricing: " + detail.price;
    }

    function sendWhatsApp() {
      const name = document.getElementById("name").value;
      const email = document.getElementById("email").value;
      const phone = document.getElementById("phone").value;
      const service = document.getElementById("serviceTitle").innerText;

      const message = `Hello, my name is ${name}. I'm interested in ${service}.\nEmail: ${email}\nPhone: ${phone}`;
      const url = `https://wa.me/917559347682?text=${encodeURIComponent(message)}`;

      window.open(url, '_blank');
    }
  </script></body>
</html><!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Professional Service Page</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #ffffff, #f0f0f0);
    }
    header {
      background-color: #0066cc;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .container {
      padding: 2rem;
    }
    .services {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
    }
    .card {
      background: #ffffff;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      padding: 1rem;
      width: 250px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }
    .card:hover {
      transform: scale(1.05);
    }
    .card h3 {
      margin-top: 0;
    }
    .hidden {
      display: none;
    }
    .details {
      background-color: #fff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      margin-top: 2rem;
    }
    .form-control {
      margin: 0.5rem 0;
    }
    .form-control input {
      width: 100%;
      padding: 0.5rem;
      border-radius: 4px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #0066cc;
      color: white;
      padding: 0.7rem 1.5rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 1rem;
    }
    footer {
      position: fixed;
      bottom: 20px;
      right: 20px;
    }
    .whatsapp-button {
      background-color: #25D366;
      color: white;
      padding: 10px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <header>
    <h1>Saurav Paswan - Professional Services</h1>
  </header>
  <div class="container">
    <div class="services">
      <div class="card" onclick="showDetails('app')">
        <h3>App Development</h3>
        <p>Build mobile apps for Android & iOS</p>
      </div>
      <div class="card" onclick="showDetails('web')">
        <h3>Web Development</h3>
        <p>Responsive, Modern Websites</p>
      </div>
      <div class="card" onclick="showDetails('ai')">
        <h3>AI Solutions</h3>
        <p>Custom AI-powered tools & apps</p>
      </div>
      <div class="card" onclick="showDetails('tools')">
        <h3>Tool Development</h3>
        <p>Unique utilities for personal or business use</p>
      </div>
    </div><div class="details hidden" id="detailSection">
  <h2 id="serviceTitle"></h2>
  <p id="serviceDescription"></p>
  <p id="servicePrice"></p>
  <div class="form-control">
    <label>Name:</label>
    <input type="text" id="name" required>
  </div>
  <div class="form-control">
    <label>Email:</label>
    <input type="email" id="email" required>
  </div>
  <div class="form-control">
    <label>Phone:</label>
    <input type="text" id="phone" required>
  </div>
  <button onclick="sendWhatsApp()">Book Now on WhatsApp</button>
</div>

  </div>  <footer>
    <a class="whatsapp-button" href="tel:7559347682">Customer Support</a>
  </footer>  <script>
    const services = {
      app: {
        title: "App Development",
        description: "We build modern, scalable mobile applications for Android and iOS.",
        price: "Basic: ₹3000 | Medium: ₹6000 | High: ₹10,000+"
      },
      web: {
        title: "Web Development",
        description: "Custom websites for businesses, portfolios and startups.",
        price: "Basic: ₹2000 | Medium: ₹5000 | High: ₹9000+"
      },
      ai: {
        title: "AI Solutions",
        description: "Build intelligent bots, AI tools and automations.",
        price: "Basic: ₹4000 | Medium: ₹8000 | High: ₹15000+"
      },
      tools: {
        title: "Tool Development",
        description: "Need a special software or script? We build tools for automation & utility.",
        price: "Basic: ₹1000 | Medium: ₹3000 | High: ₹7000+"
      }
    };

    function showDetails(type) {
      const detail = services[type];
      document.getElementById("detailSection").classList.remove("hidden");
      document.getElementById("serviceTitle").innerText = detail.title;
      document.getElementById("serviceDescription").innerText = detail.description;
      document.getElementById("servicePrice").innerText = "Pricing: " + detail.price;
    }

    function sendWhatsApp() {
      const name = document.getElementById("name").value;
      const email = document.getElementById("email").value;
      const phone = document.getElementById("phone").value;
      const service = document.getElementById("serviceTitle").innerText;

      const message = `Hello, my name is ${name}. I'm interested in ${service}.\nEmail: ${email}\nPhone: ${phone}`;
      const url = `https://wa.me/917559347682?text=${encodeURIComponent(message)}`;

      window.open(url, '_blank');
    }
  </script></body>
</html>
