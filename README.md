# index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Water Hyacinth Sustainability Platform</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f7f6;
      color: #222;
    }
    header {
      background: #1b5e20;
      color: white;
      padding: 20px;
      text-align: center;
    }
    section {
      padding: 30px;
      max-width: 1100px;
      margin: auto;
    }
    h2 {
      color: #1b5e20;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 20px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    input, textarea, button {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
    }
    button {
      background: #2e7d32;
      color: white;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }
    button:hover {
      background: #1b5e20;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    footer {
      text-align: center;
      padding: 15px;
      background: #e0e0e0;
      margin-top: 40px;
    }
    canvas {
      max-width: 100%;
    }
  </style>
</head>

<body>

<header>
  <h1>🌿 Water Hyacinth to Sustainable Paper</h1>
  <p>Transforming invasive weeds into eco-friendly products</p>
</header>

<!-- 1. GEO-TAGGED REPORTING -->
<section>
  <h2>📍 Report Water Hyacinth Affected Area</h2>
  <div class="card">
    <input type="text" placeholder="Water body name">
    <textarea placeholder="Describe the problem"></textarea>
    <input type="file">
    <button onclick="alert('Geo-tagged report submitted (prototype)')">
      Submit Report
    </button>
    <p><small>* Location capture simulated for prototype</small></p>
  </div>
</section>

<!-- 2. PRODUCT TRACEABILITY -->
<section>
  <h2>♻️ Products from Recovered Water Hyacinth</h2>
  <div class="grid">
    <div class="card">
      <h3>Handmade Paper</h3>
      <p>Source: Chetti Lake</p>
      <p>₹120</p>
    </div>
    <div class="card">
      <h3>Eco Notebook</h3>
      <p>Source: Ariyalur Tank</p>
      <p>₹250</p>
    </div>
  </div>
</section>

<!-- 3. MARKETPLACE -->
<section>
  <h2>🛒 Eco-Friendly Marketplace</h2>
  <div class="card">
    <p>Support wetland restoration by buying sustainable products.</p>
    <button onclick="alert('Payment gateway integration – Phase 2')">
      Buy Now
    </button>
  </div>
</section>

<!-- 4. IMPACT DASHBOARD -->
<section>
  <h2>📊 Environmental Impact Dashboard</h2>
  <div class="card">
    <canvas id="impactChart"></canvas>
    <p style="text-align:center">Plastic usage reduced (kg)</p>
  </div>
</section>

<!-- 5. WORKSHOPS & NEWS -->
<section>
  <h2>📢 Workshops & Outreach</h2>
  <div class="card">
    <ul>
      <li>Paper-making workshop for school students – March</li>
      <li>Wetland conservation awareness program – April</li>
      <li>Eco-entrepreneurship training – May</li>
    </ul>
    <button onclick="alert('Workshop registration coming soon')">
      Register Interest
    </button>
  </div>
</section>

<footer>
  © 2026 | Sustainable Wetland Innovation | Hackathon Prototype
</footer>

<!-- CHART SCRIPT -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
  const ctx = document.getElementById('impactChart');
  new Chart(ctx, {
    type: 'line',
    data: {
      labels: ['Jan', 'Feb', 'Mar', 'Apr'],
      datasets: [{
        label: 'Plastic Reduced (kg)',
        data: [5, 12, 20, 32],
        borderColor: 'green',
        fill: false
      }]
    }
  });
</script>

</body>
</html>
