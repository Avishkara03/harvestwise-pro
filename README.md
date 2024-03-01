<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HarvestWisePro</title>
  <style>
    body {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
  </style>
</head>
<body>
  <div id="page1">
    <canvas id="logoCanvas" width="300" height="200"></canvas>
    <script>
      const canvas = document.getElementById('logoCanvas');
      const ctx = canvas.getContext('2d');

      ctx.fillStyle = 'goldenrod';
      ctx.beginPath();
      ctx.arc(50, 100, 30, 0, 2 * Math.PI);
      ctx.fill();

      ctx.strokeStyle = 'deepgreen';
      ctx.lineWidth = 5;
      ctx.beginPath();
      ctx.moveTo(40, 100);
      ctx.lineTo(55, 115);
      ctx.lineTo(75, 85);
      ctx.stroke();
      ctx.font = 'bold 20px Arial';
      ctx.fillStyle = 'black';
      ctx.fillText('HarvestWise Pro', 90, 110);

      ctx.font = '14px Arial';
      ctx.fillStyle = 'black';
      ctx.fillText('Cultivating Time Off Growing Well-Being', 90, 130);
    </script>
    <a href="javascript:void(0);" onclick="showPage('page2')">Next</a>
  </div>

  <div id="page2" style="display:none;">
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f4f4f4;
      }

      header {
        background-color: #ece7f1;
        color: #fff;
        padding: 10px;
        text-align: center;
      }

      section {
        padding: 24px;
      }

      h1 {
        color: #333333;
      }
       p {
        color: #555;
        font-size: 18px;
      }

      .cta-button {
        display: inline-block;
        padding: 10px 20px;
        background-color: #4285f4;
        color: #fff;
        text-decoration: none;
        font-size: 16px;
        border-radius: 5px;
      }
    </style>

    <header>
      <h1>Harvest Wise Pro</h1>
      <p>Where Expertise Meets Innovation</p>
    </header>

    <section>
      <h2>Welcome to HarvestWise Pro</h2>
      <p>Revolutionize your business with our advanced harvest management solutions.</p>
      <a href="#contact" class="cta-button">Get Started</a>
    </section>
    <section>
      <h2>Features</h2>
      <ul>
        <li>1: Crop Management.</li>
        <li>2: Inventory Management.</li>
        <li>3: Weather Integration.</li>
        <li>4: Financial Tracking.</li>
        <li>5: Marketplace Integration.</li>
        <li>6: Collaboration Tools.</li>
        <li>7: Customer support.</li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <p>Have questions or want to learn more? Contact us below:</p>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <textarea id="message" name="message" rows="4" placeholder="Your message..." required></textarea>

        <button type="submit" class="cta-button">Submit</button>
      </form>
    </section>

    <footer>
      <p>&copy; 2024 HarvestWise Pro. All rights reserved.</p>
    </footer>
  </div>
  <script>
    function showPage(pageId) {
      document.getElementById('page1').style.display = 'none';
      document.getElementById('page2').style.display = 'block';
    }
  </script>
</body>
</html>

