<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>EmmyNetwork</title>
  <style>
    /* General Styling */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f9;
      color: #333;
      text-align: center;
    }

    header {
      padding: 2rem;
      background: #4caf50;
      color: white;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    p {
      font-size: 1.2rem;
    }

    main {
      padding: 1rem;
    }

    a {
      text-decoration: none;
      color: #1e90ff;
      font-weight: bold;
    }

    button {
      background: #ff5722;
      color: white;
      padding: 0.8rem 1.2rem;
      border: none;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 4px;
    }

    button:hover {
      background: #e64a19;
    }

    /* Styling for the Rainbow page */
    #rainbow-page {
      display: none;
    }

    /* Make Rainbow page visible */
    .show-rainbow #rainbow-page {
      display: block;
    }

    .show-rainbow #home-page {
      display: none;
    }
  </style>
</head>
<body>
  <!-- Home Page Content -->
  <div id="home-page">
    <header>
      <h1>Welcome to EmmyNetwork</h1>
      <p>We are a community making Minefort servers.</p>
    </header>
    <main>
      <h2>Explore Options:</h2>
      <ul>
        <li><a href="#" onclick="showRainbowPage()">Rainbow - Join our community!</a></li>
      </ul>
    </main>
  </div>

  <!-- Rainbow Page Content -->
  <div id="rainbow-page">
    <header>
      <h1>Join Our Community!</h1>
      <p>We’re building something amazing together. Be part of it.</p>
      <button onclick="window.location.href='https://example.com/join'">Join Now</button>
    </header>
    <button onclick="goBack()">Back to Home</button>
  </div>

  <script>
    // Function to show the Rainbow page
    function showRainbowPage() {
      document.body.classList.add('show-rainbow');
    }

    // Function to go back to the homepage
    function goBack() {
      document.body.classList.remove('show-rainbow');
    }
  </script>
</body>
</html>
