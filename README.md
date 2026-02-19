# Kuperson.github.io
Website for kin.lancelot
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>mckiza — Software Engineer & Designer</title>
  <meta name="description" content="Portfolio and projects by mckiza — software engineering, web development and design." />

  <!-- Open Graph / Twitter -->
  <meta property="og:title" content="mckiza — Software Engineer & Designer" />
  <meta property="og:description" content="Portfolio and projects by Kuperson — software engineering, web development and design." />
  <meta property="og:type" content="website" />
  <!-- Replace with a real image URL after you add /assets/og-image.png -->
  <meta property="og:image" content="https://mckiza.github.io/assets/og-image.png" />
  <meta name="twitter:card" content="summary_large_image" />

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <link href="assets/styles.css" rel="stylesheet" />

  <!-- Favicon: add your own favicon at /assets/favicon.ico -->
  <link rel="icon" href="/assets/favicon.ico" />

  <!-- Canonical (optional) -->
  <link rel="canonical" href="https://Kuperson.github.io/" />
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <a class="brand" href="/">Kuperson</a>

      <button class="nav-toggle" aria-expanded="false" aria-controls="primary-nav" id="navToggle">
        <span class="sr-only">Toggle navigation</span>
        ☰
      </button>

      <nav id="primary-nav" class="primary-nav" role="navigation" aria-label="Primary">
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#blog">Blog</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <h1>Hi — I'm Kuperson.<br /><span class="accent">I build web tools & delightful UI.</span></h1>
        <p class="lead">Software engineer, product-minded, with a focus on clean interfaces and reliable systems. I build open-source and client-facing projects.</p>
        <p>
          <a class="btn" href="#projects">See my work</a>
          <a class="btn ghost" href="#contact">Get in touch</a>
        </p>
      </div>
    </section>

    <section id="about" class="section container">
      <div class="grid about-grid">
        <div>
          <h2>About me</h2>
          <p>I focus on front-end engineering, performance, and accessible UX. I collaborate with designers and PMs to ship product features and open-source tools. I enjoy learning new web technologies and helping others through writing and talks.</p>
          <p><strong>Skills:</strong> JavaScript/TypeScript, React, Node.js, HTML, CSS, accessibility, design systems.</p>
        </div>
        <div class="profile-card">
          <!-- Replace placeholder avatar with your image at /assets/avatar.jpg -->
          <img alt="Kuperson avatar" src="/assets/avatar.jpg" class="avatar" />
          <div>
            <p><strong>Location:</strong> (Your city)</p>
            <p><strong>Available for:</strong> freelance, contract, open-source collaboration</p>
          </div>
        </div>
      </div>
    </section>

    <section id="projects" class="section projects container">
      <h2>Selected projects</h2>
      <div class="cards-grid">
        <article class="card">
          <h3><a href="https://github.com/Kuperson/example-project-1" target="_blank" rel="noopener">Project One</a></h3>
          <p>Short description of the project, tech used, and impact.</p>
          <p class="muted">React · TypeScript · Vercel</p>
        </article>

        <article class="card">
          <h3><a href="https://github.com/Kuperson/example-project-2" target="_blank" rel="noopener">Project Two</a></h3>
          <p>Short description of the project, tech used, and impact.</p>
          <p class="muted">Node · API · Docker</p>
        </article>

        <article class="card">
          <h3><a href="https://github.com/Kuperson/example-project-3" target="_blank" rel="noopener">Project Three</a></h3>
          <p>Short description of the project, tech used, and impact.</p>
          <p class="muted">Design System · Accessibility</p>
        </article>
      </div>
      <p class="more"><a href="https://github.com/Kuperson?tab=repositories" target="_blank" rel="noopener">More projects on GitHub →</a></p>
    </section>

    <section id="blog" class="section container">
      <h2>Latest posts</h2>
      <ul class="blog-list">
        <!-- If you add a blog, replace these with real links -->
        <li><a href="#">How I built a lightning-fast UI — Jan 2026</a></li>
        <li><a href="#">Designing accessible components — Dec 2025</a></li>
      </ul>
      <p class="more"><a href="/blog/">View all posts →</a></p>
    </section>

    <section id="contact" class="section contact container">
      <h2>Contact</h2>
      <p>If you'd like to work together or chat about open-source, email me at <a href="mailto:mckinnankuperson@gmail.com">mckinnankuperson@gmail.com</a> or find me on <a href="https://github.com/Kuperson" target="_blank" rel="noopener">GitHub</a>.</p>

      <div class="contact-grid">
        <div class="contact-card">
          <h3>Availability</h3>
          <p>Open for freelance and contract work. Available to start: (date)</p>
        </div>
        <div class="contact-card">
          <h3>Newsletter</h3>
          <p>Collect emails using a form service (e.g. Buttondown, ConvertKit) or add a simple mailing list.</p>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <p>© <span id="year"></span> Kuperson — <a href="https://github.com/mckiza" target="_blank" rel="noopener">GitHub</a> · <a href="/resume.pdf">Resume</a></p>
    </div>
  </footer>

  <script>
    // Set year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Mobile nav toggle
    const navToggle = document.getElementById('navToggle');
    const nav = document.getElementById('primary-nav');
    navToggle.addEventListener('click', () => {
      const expanded = navToggle.getAttribute('aria-expanded') === 'true' || false;
      navToggle.setAttribute('aria-expanded', !expanded);
      nav.classList.toggle('open');
    });
  </script>
</body>
</html>
