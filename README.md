<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Jovi Sicat - Portfolio</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />

  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url('images/pexels-greennature-167684.jpeg') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
      margin: 0;
      padding-top: 70px;
    }

    .navbar {
      background-color: rgba(0, 0, 0, 0.85) !important;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    }

    .navbar-nav .nav-link {
      font-weight: 500;
      transition: color 0.3s;
    }

    .navbar-nav .nav-link:hover {
      color: #ffc107;
    }

    .profile-photo-container {
      text-align: center;
      margin-top: 30px;
    }

    .profile-photo {
      width: 160px;
      height: 160px;
      object-fit: cover;
      border-radius: 50%;
      border: 5px solid #fff;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.6);
      transition: transform 0.3s ease;
    }

    .profile-photo:hover {
      transform: scale(1.05);
    }

    .hero {
      padding: 100px 20px;
      text-align: center;
    }

    .hero h1 {
      font-size: 3rem;
      font-weight: 700;
    }

    .hero p {
      font-size: 1.2rem;
      font-style: italic;
      color: #ddd;
    }

    section {
      padding: 60px 20px;
    }

    #project,
    #contact {
      background-color: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(4px);
    }

    #project .card {
      background-color: rgba(0, 0, 0, 0.6);
      color: white;
      border: none;
      transition: transform 0.3s;
    }

    #project .card:hover {
      transform: translateY(-10px);
    }

    #about .container {
      background-color: rgba(0, 0, 0, 0.75);
      border-radius: 15px;
      padding: 40px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
    }

    #about p {
      font-size: 1.1rem;
      line-height: 1.7;
      color: #eee;
    }

    #about span {
      color: #0d6efd;
      font-weight: 600;
    }

    #about .highlight-yellow {
      color: #ffc107;
    }

    .tools-container {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      margin-top: 15px;
    }

    .tool-icon {
      width: 55px;
      height: 55px;
      transition: transform 0.3s;
      filter: drop-shadow(0 0 5px rgba(0, 0, 0, 0.5));
    }

    .tool-icon:hover {
      transform: scale(1.2);
    }

    #contact a {
      transition: color 0.3s, transform 0.3s;
      color: white;
    }

    #contact a:hover {
      color: #ffc107;
      transform: scale(1.2);
    }

    footer {
      background-color: rgba(0, 0, 0, 0.85);
    }

    .btn-outline-light {
      border-color: #ffc107;
      color: #ffc107;
    }

    .btn-outline-light:hover {
      background-color: #ffc107;
      color: #000;
    }
  </style>
</head>

<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#"></a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
  <ul class="navbar-nav">
    <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
    <li class="nav-item"><a class="nav-link" href="#project">Project</a></li>
    <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
  </ul>
</div>
    </div>
  </nav>

  <!-- Profile Photo -->
  <div class="profile-photo-container">
    <img src="images/headerphoto.jpg" alt="Jovi Sicat" class="profile-photo" />
  </div>

  <!-- Hero Section -->
  <div class="hero">
    <h1>Hi, I'm Jovi Sicat</h1>
    <p>"Data is the new oil, and I am the refinery."</p>
  </div>

<!-- Project Section -->
<section id="project">
  <div class="container text-center">
    <h2 class="mb-5">Projects</h2>
    <div class="row justify-content-center g-4">

      <!-- Project Card 1 -->
      <div class="col-md-6 col-lg-4">
        <div class="card h-100 p-0">
          <img src="images/project1.png" class="card-img-top" alt="Barangay Permit Request System" onclick="zoomImage(this.src)" data-bs-toggle="modal" data-bs-target="#zoomModal">
          <div class="card-body d-flex flex-column">
            <h5 class="card-title">Barangay Permit Request System</h5>
            <p class="card-text">A command-line system for handling permit requests. Uses user authentication via <code>users.txt</code> and stores data in <code>permits.csv</code>.</p>
            <button class="btn btn-outline-light mt-auto" onclick="zoomImage('images/project1.png')" data-bs-toggle="modal" data-bs-target="#zoomModal">
              Zoom Image
            </button>
          </div>
        </div>
      </div>

      <!-- Project Card 2 -->
      <div class="col-md-6 col-lg-4">
        <div class="card h-100 p-0">
          <img src="images/gymwebsite.png" class="card-img-top" alt="Fitness Gym Website" onclick="zoomImage(this.src)" data-bs-toggle="modal" data-bs-target="#zoomModal">
          <div class="card-body d-flex flex-column">
            <h5 class="card-title">Fitness Gym Website</h5>
            <p class="card-text">A Figma-designed landing page for FlexFit Gym. Emphasizes exclusivity with premium features like members-only classes and personal coaching.</p>
            <button class="btn btn-outline-light mt-auto" onclick="zoomImage('images/gymwebsite.png')" data-bs-toggle="modal" data-bs-target="#zoomModal">
              Zoom Image
            </button>
          </div>
        </div>
      </div>

      <!-- Project Card 3 -->
      <div class="col-md-6 col-lg-4">
        <div class="card h-100 p-0">
          <img src="images/Basic Hospital Management System.png" class="card-img-top" alt="Basic Hospital Management System" onclick="zoomImage(this.src)" data-bs-toggle="modal" data-bs-target="#zoomModal">
          <div class="card-body d-flex flex-column">
            <h5 class="card-title">Basic Hospital Management System</h5>
            <p class="card-text">Python-based tool that evaluates a patient's condition and suggests medical actions like ICU or surgery. Simulates hospital triage with logic conditions.</p>
            <button class="btn btn-outline-light mt-auto" onclick="zoomImage('images/Basic Hospital Management System.png')" data-bs-toggle="modal" data-bs-target="#zoomModal">
              Zoom Image
            </button>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- Zoom Modal -->
<div class="modal fade" id="zoomModal" tabindex="-1" aria-labelledby="zoomModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered modal-lg">
    <div class="modal-content bg-dark">
      <div class="modal-header border-0">
        <h5 class="modal-title text-white" id="zoomModalLabel">Zoomed Image</h5>
        <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body text-center">
        <img id="zoomedImage" src="" alt="Zoomed Project" class="img-fluid rounded shadow" />
      </div>
    </div>
  </div>
</div>


  <!-- About Section -->
<section id="about">
  <div class="container text-center">
    <h2 class="mb-4">About Me</h2>
    <div class="row align-items-center">
      <div class="col-md-7 text-start">
        <p>
          Hey there! 👋 I'm <strong>Jovi Sicat</strong>, a curious and creative <span>Data Analyst</span> with a passion for transforming raw numbers into meaningful insights. 
        </p>
        <p>
          I thrive at the intersection of <em>data storytelling</em> and <em>problem-solving</em>, using languages like <strong>Python</strong> and <strong>C++</strong> to uncover patterns, streamline processes, and build smart solutions.
        </p>
        <p>
          Whether it's crafting dashboards, analyzing trends, or coding efficient systems, I'm all about delivering <span class="highlight-yellow">impact-driven results</span>. Let's connect and turn complex data into clear direction.
        </p>
      </div>
      <div class="col-md-5 mt-4 mt-md-0 text-start">
        <h4>Tools I Use:</h4>
        <div class="tools-container">
          <img src="images/python.png" alt="Python" title="Python" class="tool-icon" />
          <img src="images/c++.png" alt="C++" title="C++" class="tool-icon" />
          <img src="images/bootstrap.png" alt="Bootstrap" title="Bootstrap" class="tool-icon" />
          <img src="images/html.png" alt="HTML" title="HTML" class="tool-icon" />
        </div>
      </div>
    </div>
  </div>
</section>


<!-- Contact Section -->
<section id="contact" class="py-5">
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-lg-8 text-center">
        <h2 class="mb-4">Contact Me</h2>
        <p class="mb-4 fs-5">Let's connect! Reach out via social media or send me an email.</p>
        <div class="card bg-dark text-white p-4 shadow-lg border-0">
          <div class="d-flex flex-column flex-md-row justify-content-center gap-4 fs-3">
            <a href="https://www.facebook.com/yourprofile" target="_blank" aria-label="Facebook" class="text-white">
              <i class="fab fa-facebook-f"></i>
            </a>
            <a href="https://twitter.com/yourhandle" target="_blank" aria-label="X" class="text-white">
              <i class="fab fa-x-twitter"></i>
            </a>
            <a href="https://www.instagram.com/yourusername" target="_blank" aria-label="Instagram" class="text-white">
              <i class="fab fa-instagram"></i>
            </a>
          </div>
          <div class="mt-4">
            <a href="mailto:jovisicat@email.com" class="btn btn-outline-light">
              Send me an email
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>



  <!-- Footer -->
  <footer class="text-center py-4">
    <div class="container">
      <p class="mb-0">© 2025 Jovi Sicat. All rights reserved.</p>
    </div>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
  <script>
  function zoomImage(src) {
    document.getElementById('zoomedImage').src = src;
  }
</script>
</body>

</html>
