<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Susith R | AI & Data Science</title>
  <meta name="description" content="Innovative AI solutions and data-driven development">
  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <!-- Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --text: #1a1a1a;
      --text-light: #666666;
      --background: #ffffff;
      --card-bg: #f9f9f9;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--background);
      color: var(--text);
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* Navigation */
    nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      padding: 2rem 4rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 100;
      background: var(--background);
    }

    .logo {
      font-weight: 700;
      font-size: 1.25rem;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--text);
      font-weight: 500;
      transition: color 0.3s ease;
    }

    .nav-links a:hover {
      color: var(--text-light);
    }

    /* Header */
    header {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 4rem;
      margin-top: 80px;
      max-width: 1200px;
      margin-left: auto;
      margin-right: auto;
    }

    .header-content {
      max-width: 800px;
    }

    header h1 {
      font-size: 3.5rem;
      font-weight: 700;
      margin-bottom: 1.5rem;
      line-height: 1.1;
    }

    header p {
      font-size: 1.25rem;
      color: var(--text-light);
      margin-bottom: 2rem;
      max-width: 600px;
    }

    /* Sections */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 4rem;
    }

    section {
      padding: 8rem 0;
    }

    .section-title {
      margin-bottom: 4rem;
    }

    .section-title h2 {
      font-size: 2rem;
      font-weight: 600;
    }

    /* About Section */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 3rem;
      align-items: center;
    }

    @media (min-width: 992px) {
      .about-grid {
        grid-template-columns: 1fr 1fr;
      }
    }

    .profile-img {
      width: 100%;
      max-width: 500px;
      border-radius: 8px;
    }

    .about-content h3 {
      font-size: 1.5rem;
      margin-bottom: 1.5rem;
      font-weight: 600;
    }

    .about-content p {
      margin-bottom: 1.5rem;
      font-size: 1rem;
      line-height: 1.7;
      color: var(--text-light);
    }

    .education-item {
      margin-bottom: 1.5rem;
    }

    .education-item h4 {
      font-weight: 600;
      margin-bottom: 0.25rem;
    }

    .education-item p {
      color: var(--text-light);
      margin-bottom: 0.25rem;
    }

    /* Skills Section */
    .skills-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 2rem;
    }

    .skill-category {
      margin-bottom: 2rem;
    }

    .skill-category h3 {
      font-size: 1.25rem;
      margin-bottom: 1.5rem;
      font-weight: 600;
    }

    .skill-item {
      margin-bottom: 1rem;
    }

    .skill-name {
      font-weight: 500;
      margin-bottom: 0.5rem;
    }

    /* Projects Section */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
      gap: 2rem;
    }

    .project-card {
      background: var(--card-bg);
      border-radius: 8px;
      overflow: hidden;
    }

    .project-image {
      height: 250px;
      overflow: hidden;
    }

    .project-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .project-content {
      padding: 2rem;
    }

    .project-content h3 {
      font-size: 1.25rem;
      margin-bottom: 0.75rem;
      font-weight: 600;
    }

    .project-content p {
      color: var(--text-light);
      margin-bottom: 1.5rem;
    }

    .project-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .tag {
      background: var(--text-light);
      color: white;
      padding: 0.25rem 0.75rem;
      border-radius: 20px;
      font-size: 0.8rem;
      font-weight: 500;
    }

    /* Contact Section */
    .contact-container {
      display: grid;
      grid-template-columns: 1fr;
      gap: 3rem;
    }

    @media (min-width: 992px) {
      .contact-container {
        grid-template-columns: 1fr 1fr;
      }
    }

    .contact-info h3 {
      font-size: 1.5rem;
      margin-bottom: 2rem;
      font-weight: 600;
    }

    .contact-detail {
      display: flex;
      align-items: center;
      margin-bottom: 1.5rem;
    }

    .contact-icon {
      width: 40px;
      height: 40px;
      background: var(--text);
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 1rem;
    }

    .contact-detail p:first-child {
      font-weight: 500;
      margin-bottom: 0.25rem;
    }

    .contact-detail p:last-child {
      color: var(--text-light);
    }

    .contact-form {
      background: var(--card-bg);
      padding: 2.5rem;
      border-radius: 8px;
    }

    .form-group {
      margin-bottom: 1.5rem;
    }

    .form-control {
      width: 100%;
      padding: 0.875rem;
      border: 1px solid #e0e0e0;
      border-radius: 8px;
      background: var(--background);
      font-family: 'Inter', sans-serif;
    }

    textarea.form-control {
      min-height: 150px;
    }

    .submit-btn {
      background: var(--text);
      color: white;
      border: none;
      padding: 0.875rem 2rem;
      border-radius: 8px;
      font-family: 'Inter', sans-serif;
      font-weight: 600;
      cursor: pointer;
    }

    /* Footer */
    footer {
      background: var(--card-bg);
      padding: 4rem 0;
      text-align: center;
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin: 2rem 0;
    }

    .social-link {
      width: 40px;
      height: 40px;
      background: var(--text);
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1rem;
    }

    .copyright {
      color: var(--text-light);
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <!-- Navigation -->
  <nav>
    <div class="logo">Susith R</div>
    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Work</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Header -->
  <header>
    <div class="header-content">
      <h1>I'm Susith R.</h1>
      <h1>A Data Scientist & AI Developer</h1>
      <p>I'm probably the most passionate data scientist you will ever get to work with. If you have a great project that needs amazing AI solutions, I'm your guy.</p>
    </div>
  </header>

  <!-- About Section -->
  <section id="about">
    <div class="container">
      <div class="section-title">
        <h2>About Me</h2>
      </div>
      <div class="about-grid">
        <div class="about-content">
          <h3>Innovative Problem Solver</h3>
          <p>
            I specialize in building AI-powered applications that bridge the gap between complex data science 
            and user-friendly interfaces. My approach combines cutting-edge machine learning with elegant 
            full-stack development.
          </p>
          <p>
            With expertise in Python, TensorFlow, and modern web technologies, I create solutions that are 
            both technically robust and visually compelling.
          </p>
          
          <h3>Education</h3>
          <div class="education-item">
            <h4>V.S.B Engineering College, Karur</h4>
            <p>B.Tech in Artificial Intelligence & Data Science</p>
            <p>CGPA: 7.5 (Current)</p>
          </div>
          <div class="education-item">
            <h4>Govt. Model Higher Secondary School</h4>
            <p>Higher Secondary Certificate</p>
            <p>Percentage: 79.3%</p>
          </div>
        </div>
        <div style="display: flex; justify-content: center;">
          <img 
            src="https://images.unsplash.com/photo-1571171637578-41bc2dd41cd2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" 
            alt="Profile" 
            class="profile-img"
          />
        </div>
      </div>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <div class="container">
      <div class="section-title">
        <h2>Technical Expertise</h2>
      </div>
      <div class="skills-container">
        <div class="skill-category">
          <h3>AI/ML</h3>
          <div class="skill-item">
            <div class="skill-name">TensorFlow/Keras</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Computer Vision</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Natural Language Processing</div>
          </div>
        </div>
        
        <div class="skill-category">
          <h3>Development</h3>
          <div class="skill-item">
            <div class="skill-name">Python</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Java</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">JavaScript</div>
          </div>
        </div>
        
        <div class="skill-category">
          <h3>Web Technologies</h3>
          <div class="skill-item">
            <div class="skill-name">React</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Node.js</div>
          </div>
          <div class="skill-item">
            <div class="skill-name">REST APIs</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects">
    <div class="container">
      <div class="section-title">
        <h2>Featured Work</h2>
      </div>
      <div class="projects-grid">
        <div class="project-card">
          <div class="project-image">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="Student Database" />
          </div>
          <div class="project-content">
            <h3>Student Management AI</h3>
            <p>
              An intelligent system combining database management with predictive analytics to optimize 
              educational outcomes and student engagement.
            </p>
            <div class="project-tags">
              <span class="tag">Python</span>
              <span class="tag">TensorFlow</span>
              <span class="tag">React</span>
            </div>
          </div>
        </div>
        
        <div class="project-card">
          <div class="project-image">
            <img src="https://images.unsplash.com/photo-1512941937669-90a1b58e7e9c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="Drowsiness Detection" />
          </div>
          <div class="project-content">
            <h3>VisionGuard</h3>
            <p>
              Real-time computer vision system that detects driver fatigue using advanced facial recognition 
              algorithms and alert mechanisms.
            </p>
            <div class="project-tags">
              <span class="tag">OpenCV</span>
              <span class="tag">Dlib</span>
              <span class="tag">Flask</span>
            </div>
          </div>
        </div>
        
        <div class="project-card">
          <div class="project-image">
            <img src="https://images.unsplash.com/photo-1614680376573-df3480f0c6ff?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="AI Chatbot" />
          </div>
          <div class="project-content">
            <h3>EduBot</h3>
            <p>
              Context-aware educational assistant using NLP to provide personalized learning resources and 
              deadline management for students.
            </p>
            <div class="project-tags">
              <span class="tag">NLTK</span>
              <span class="tag">Transformers</span>
              <span class="tag">React</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <div class="container">
      <div class="section-title">
        <h2>Contact</h2>
      </div>
      <div class="contact-container">
        <div class="contact-info">
          <h3>Get in Touch</h3>
          <div class="contact-detail">
            <div class="contact-icon">
              <i class="fas fa-envelope"></i>
            </div>
            <div>
              <p>Email</p>
              <p>susithsusith43@gmail.com</p>
            </div>
          </div>
          <div class="contact-detail">
            <div class="contact-icon">
              <i class="fas fa-phone"></i>
            </div>
            <div>
              <p>Phone</p>
              <p>+91 6369578484</p>
            </div>
          </div>
          <div class="contact-detail">
            <div class="contact-icon">
              <i class="fas fa-map-marker-alt"></i>
            </div>
            <div>
              <p>Location</p>
              <p>Karur, Tamil Nadu, India</p>
            </div>
          </div>
        </div>
        <div class="contact-form">
          <form action="https://formspree.io/f/mqapdelq" method="POST">
            <div class="form-group">
              <input type="text" name="name" class="form-control" placeholder="Your Name" required>
            </div>
            <div class="form-group">
              <input type="email" name="email" class="form-control" placeholder="Your Email" required>
            </div>
            <div class="form-group">
              <textarea name="message" class="form-control" placeholder="Your Message" required></textarea>
            </div>
            <button type="submit" class="submit-btn">
              Send Message <i class="fas fa-paper-plane" style="margin-left: 8px;"></i>
            </button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <h3>Susith R</h3>
      <p style="margin: 1rem 0;">Building intelligent systems at the intersection of AI and design</p>
      <div class="social-links">
        <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
        <a href="#" class="social-link"><i class="fab fa-github"></i></a>
        <a href="#" class="social-link"><i class="fab fa-twitter"></i></a>
      </div>
      <p class="copyright">&copy; <script>document.write(new Date().getFullYear())</script> All rights reserved</p>
    </div>
  </footer>
</body>
</html>
