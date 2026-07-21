---
layout: default
title: GIS Portfolio
---

<style>
  :root {
    color-scheme: dark;
    --background: #121414;
    --surface: #191c1c;
    --surface-hover: #202424;
    --text: #e7e9e9;
    --muted: #b8bebe;
    --border: #363c3c;
    --accent: #6fb7b1;
    --accent-light: #9bd2cd;
  }

  * {
    box-sizing: border-box;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    margin: 0;
    background: var(--background);
    color: var(--text);
    font-family: Calibri, "Segoe UI", Arial, sans-serif;
  }

  /* Hide Minima's default header */
  .site-header {
    display: none;
  }

  .site-footer {
    background: var(--surface);
    border-color: var(--border);
    color: var(--muted);
  }

  .wrapper {
    width: 92%;
    max-width: 1400px;
    padding-right: 20px;
    padding-left: 20px;
  }

  .page-content {
    padding-top: 0;
  }

  a {
    color: var(--accent);
  }

  a:hover {
    color: var(--accent-light);
  }

  a:focus-visible,
  .project-card:focus-visible {
    outline: 3px solid var(--accent);
    outline-offset: 4px;
  }

  .skip-link {
    position: absolute;
    top: -100px;
    left: 20px;
    z-index: 1000;
    padding: 10px 14px;
    background: #ffffff;
    color: #111111;
    text-decoration: none;
  }

  .skip-link:focus {
    top: 20px;
  }

  /* Top navigation */
  .portfolio-nav {
    border-bottom: 1px solid var(--border);
    background: var(--surface);
  }

  .portfolio-nav-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 92%;
    max-width: 1400px;
    min-height: 68px;
    margin: 0 auto;
    padding: 0 20px;
  }

  .portfolio-title {
    color: #ffffff;
    font-size: 1.25rem;
    font-weight: 700;
    text-decoration: none;
  }

  .portfolio-title:hover {
    color: var(--accent-light);
    text-decoration: none;
  }

  .nav-links {
    display: flex;
    align-items: center;
    gap: 24px;
  }

  .nav-links a {
    font-weight: 600;
    text-decoration: none;
  }

  /* Main sections */
  .portfolio-main {
    width: 92%;
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 20px;
  }

  .section {
    padding: 60px 0;
    border-bottom: 1px solid var(--border);
  }

  .section h1,
  .section h2,
  .section h3 {
    color: #ffffff;
  }

  .section h1 {
    margin-bottom: 20px;
    font-size: clamp(2rem, 4vw, 3rem);
  }

  .section h2 {
    margin-bottom: 22px;
    font-size: 2rem;
  }

  .about-text {
    max-width: 850px;
    color: var(--muted);
    font-size: 1.08rem;
  }

  .about-text p:last-child {
    margin-bottom: 0;
  }

  /* Project grid */
  .project-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
    margin-top: 30px;
  }

  .project-card {
    display: block;
    overflow: hidden;
    border: 1px solid var(--border);
    border-radius: 5px;
    background: var(--surface);
    color: inherit;
    text-decoration: none;
  }

  .project-card:hover {
    border-color: var(--accent);
    background: var(--surface-hover);
    text-decoration: none;
  }

  .project-card img {
    display: block;
    width: 100%;
    aspect-ratio: 1 / 1;
    margin: 0;
    object-fit: cover;
    background: #242828;
  }

  .project-card-text {
    padding: 20px;
  }

  .project-card h3 {
    margin: 0 0 10px;
    font-size: 1.35rem;
  }

  .project-card p {
    margin: 0 0 16px;
    color: var(--muted);
  }

  /* Project tags */
  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .project-tags span {
    display: inline-block;
    padding: 5px 9px;
    border: 1px solid var(--accent);
    border-radius: 999px;
    color: var(--accent-light);
    font-size: 0.82rem;
  }

  /* Detailed project sections */
  .project-detail {
    padding: 75px 0;
    border-bottom: 1px solid var(--border);
    scroll-margin-top: 30px;
  }

  .project-detail h2,
  .project-detail h3,
  .project-detail p {
    max-width: 900px;
  }

  .project-detail h2,
  .project-detail h3 {
    color: #ffffff;
  }

  .project-detail p {
    color: var(--muted);
  }

  .project-detail .project-tags {
    margin-bottom: 24px;
  }

  .tools-line {
    margin: 22px 0;
    padding-left: 14px;
    border-left: 3px solid var(--accent);
  }

  .tools-line strong {
    color: var(--text);
  }

  .project-detail img {
    display: block;
    max-width: 100%;
    width: auto;
    height: auto;
    margin: 32px auto 32px 0;
    border: 1px solid var(--border);
  }

  .return-link {
    margin-top: 35px;
  }

  @media screen and (max-width: 900px) {
    .project-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }
  }

  @media screen and (max-width: 600px) {
    .portfolio-nav-inner,
    .portfolio-main {
      width: 94%;
      padding-right: 10px;
      padding-left: 10px;
    }

    .portfolio-nav-inner {
      align-items: flex-start;
      flex-direction: column;
      justify-content: center;
      gap: 8px;
      padding-top: 14px;
      padding-bottom: 14px;
    }

    .nav-links {
      gap: 18px;
    }

    .project-grid {
      grid-template-columns: 1fr;
    }

    .section {
      padding: 45px 0;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    html {
      scroll-behavior: auto;
    }
  }
</style>

<a class="skip-link" href="#main-content">Skip to main content</a>

<nav class="portfolio-nav" aria-label="Main navigation">
  <div class="portfolio-nav-inner">

    <a class="portfolio-title" href="#main-content">
      Your Name — GIS Portfolio
    </a>

    <div class="nav-links">
      <a href="https://www.linkedin.com/in/your-linkedin-name">
        LinkedIn
      </a>

      <a href="mailto:your-email@example.com">
        Email
      </a>
    </div>

  </div>
</nav>

<main class="portfolio-main" id="main-content">

  <section class="section" aria-labelledby="about-heading">
    <h1 id="about-heading">About</h1>

    <div class="about-text">
      <p>
        I am a GIS student interested in spatial analysis, cartography
        and geographic data visualisation.
      </p>

      <p>
        This portfolio presents selected projects completed during my studies,
        with an emphasis on clear spatial analysis and effective visual
        communication.
      </p>
    </div>
  </section>

  <section class="section" aria-labelledby="projects-heading">
    <h2 id="projects-heading">Projects</h2>

    <div class="project-grid">

      <a class="project-card" href="#project-one">
        <img
          src="{{ '/assets/images/BlackImage.png' | relative_url }}"
          alt="Describe the map shown for Project One">

        <div class="project-card-text">
          <h3>Project One</h3>

          <p>
            A concise description of the project's purpose and main outcome.
          </p>

          <div class="project-tags" aria-label="Project One tools and techniques">
            <span>QGIS</span>
            <span>Spatial analysis</span>
            <span>Cartography</span>
          </div>
        </div>
      </a>

      <a class="project-card" href="#project-two">
        <img
          src="{{ '/assets/images/BlackImage2.png' | relative_url }}"
          alt="Describe the map shown for Project Two">

        <div class="project-card-text">
          <h3>Project Two</h3>

          <p>
            A concise description of the project's purpose and main outcome.
          </p>

          <div class="project-tags" aria-label="Project Two tools and techniques">
            <span>ArcGIS Pro</span>
            <span>Data visualisation</span>
            <span>GIS analysis</span>
          </div>
        </div>
      </a>

      <a class="project-card" href="#project-three">
        <img
          src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
          alt="Describe the map shown for Project Three">

        <div class="project-card-text">
          <h3>Project Three</h3>

          <p>
            A concise description of the project's purpose and main outcome.
          </p>

          <div class="project-tags" aria-label="Project Three tools and techniques">
            <span>Mapping</span>
            <span>Spatial research</span>
            <span>GIS</span>
          </div>
        </div>
      </a>

    </div>
  </section>

  <section class="project-detail" id="project-one" aria-labelledby="project-one-heading">
    <h2 id="project-one-heading">Project One</h2>

    <div class="project-tags" aria-label="Project One tools and techniques">
      <span>QGIS</span>
      <span>Spatial analysis</span>
      <span>Cartography</span>
    </div>

    <p>
      Explain the question, problem or geographic area investigated in
      this project.
    </p>

    <p class="tools-line">
      <strong>Tools and techniques:</strong>
      QGIS, spatial analysis and cartographic design.
    </p>

    <img
      src="{{ '/assets/images/BlackImage.png' | relative_url }}"
      alt="Describe the final map and the geographic information it displays">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe how the final result was produced.
    </p>

    <h3>Results</h3>

    <p>
      Explain the main findings, important spatial patterns and what
      the map demonstrates.
    </p>

    <p class="return-link">
      <a href="#projects-heading">Return to projects</a>
    </p>
  </section>

  <section class="project-detail" id="project-two" aria-labelledby="project-two-heading">
    <h2 id="project-two-heading">Project Two</h2>

    <div class="project-tags" aria-label="Project Two tools and techniques">
      <span>ArcGIS Pro</span>
      <span>Data visualisation</span>
      <span>GIS analysis</span>
    </div>

    <p>
      Explain the question, problem or geographic area investigated in
      this project.
    </p>

    <p class="tools-line">
      <strong>Tools and techniques:</strong>
      ArcGIS Pro, GIS analysis and data visualisation.
    </p>

    <img
      src="{{ '/assets/images/BlackImage2.png' | relative_url }}"
      alt="Describe the final map and the geographic information it displays">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe how the final result was produced.
    </p>

    <h3>Results</h3>

    <p>
      Explain the main findings, important spatial patterns and what
      the map demonstrates.
    </p>

    <p class="return-link">
      <a href="#projects-heading">Return to projects</a>
    </p>
  </section>

  <section class="project-detail" id="project-three" aria-labelledby="project-three-heading">
    <h2 id="project-three-heading">Project Three</h2>

    <div class="project-tags" aria-label="Project Three tools and techniques">
      <span>Mapping</span>
      <span>Spatial research</span>
      <span>GIS</span>
    </div>

    <p>
      Explain the question, problem or geographic area investigated in
      this project.
    </p>

    <p class="tools-line">
      <strong>Tools and techniques:</strong>
      GIS mapping, spatial research and geographic data management.
    </p>

    <img
      src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
      alt="Describe the final map and the geographic information it displays">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe how the final result was produced.
    </p>

    <h3>Results</h3>

    <p>
      Explain the main findings, important spatial patterns and what
      the map demonstrates.
    </p>

    <p class="return-link">
      <a href="#projects-heading">Return to projects</a>
    </p>
  </section>

</main>
