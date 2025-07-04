# Foton-Training
Foton Training (IGTR)
<!DOCTYPE html>
<html lang="id">
<head>
   <meta http-equiv="refresh" content="0; URL='Foton%20Training%20Center%20admin%20lgtr.index.html'" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FOTON Training Center</title>
  <!-- Bootstrap CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .navbar-brand {
      font-weight: bold;
      color: red;
    }
    .banner {
      background: url('https://via.placeholder.com/1200x300') no-repeat center center;
      background-size: cover;
      height: 300px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 2px 2px 4px #000;
    }
    .content-section {
      padding: 40px 0;
    }
    footer {
      background: #343a40;
      color: white;
      padding: 10px 0;
      text-align: center;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">FOTON Training Center</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#">My Courses</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Katalog Video</a></li>
          <li class="nav-item"><a class="nav-link" href="#">FAQ</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Jadwal Training</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Form Permintaan Training</a></li>
        </ul>
        <form class="d-flex">
          <input class="form-control me-2" type="text" placeholder="Username">
          <input class="form-control me-2" type="password" placeholder="Password">
          <button class="btn btn-outline-success" type="submit">Login</button>
        </form>
      </div>
    </div>
  </nav>

  <!-- Banner -->
  <div class="banner">
    <h1>Selamat Datang di FOTON Training Center</h1>
  </div>

  <!-- Main Content -->
  <div class="container content-section">
    <div class="row text-center">
      <div class="col-md-4">
        <div class="p-4 border rounded bg-light">
          <h4>Konten Utama</h4>
          <p>Pelatihan untuk meningkatkan keterampilan mekanik & teknisi dealer FOTON.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 border rounded bg-light">
          <h4>Artikel</h4>
          <p>Tulisan terbaru seputar teknologi kendaraan listrik dan operasional.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 border rounded bg-light">
          <h4>Form Permintaan</h4>
          <p>Isi form untuk permintaan training tambahan di lokasi dealer Anda.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <div class="container">
      &copy; 2025 FOTON Training (IGTR). All rights reserved.
    </div>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
<script>
  const form = document.querySelector("form");
  form.addEventListener("submit", function (e) {
    e.preventDefault(); // Hindari reload

    const username = form.querySelector("input[type='text']").value;
    const password = form.querySelector("input[type='password']").value;

    if (username === "admin" && password === "1234") {
      alert("Login berhasil! Selamat datang, " + username);
      // Bisa redirect ke halaman lain: window.location.href = "dashboard.html";
    } else {
      alert("Login gagal. Username atau password salah.");
    }
  });
</script>
<form id="loginForm">
  <input type="text" id="username" placeholder="Username">
  <input type="password" id="password" placeholder="Password">
  <button type="submit">Login</button>
</form>
