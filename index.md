---
layout: default
title: GIS Portfolio
---

<style>
  :root {
    color-scheme: dark;
  }

  * {
    box-sizing: border-box;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    background: #121212;
    color: #e8e8e8;
    font-family: Calibri, "Segoe UI", Arial, sans-serif;
  }

  a {
    color: #8fc7ff;
  }

  a:hover {
    color: #c5e2ff;
  }

  a:focus-visible,
  .project-card:focus-visible {
    outline: 3px solid #8fc7ff;
    outline-offset: 4px;
  }

  .wrapper {
    max-width: 1400px;
    width: 92%;
    padding-left: 20px;
    padding-right: 20px;
  }

  .page-content {
    padding-top: 0;
  }

  .site-header,
  .site-footer {
    background: #181818;
    border-color: #333333;
  }

  .site-title,
  .site-title:visited {
    color: #f4f4f4;
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

  .portfolio-header {
    padding: 70px 0 55px;
    border-bottom: 1px solid #333333;
  }

  .portfolio-header h1 {
    margin-bottom: 12px;
    color: #ffffff;
    font-size: clamp(2.4rem, 5vw, 4rem);
    line-height: 1.1;
  }

  .portfolio-header p {
    max-width: 850px;
    margin-bottom: 18px;
    color: #cccccc;
    font-size: 1.15rem;
  }

  .contact-links {
    display: flex;
    flex-wrap: wrap;
    gap: 18px;
    margin-top: 22px;
  }

  .contact-links a {
    font-weight: 600;
  }

  .section {
    padding: 65px 0;
    border-bottom: 1px solid #333333;
  }

  .section h2 {
    margin-bottom: 22px;
    color: #ffffff;
    font-size: 2rem;
  }

  .section-intro {
    max-width: 900px;
    color: #cccccc;
  }

  .about-text {
    max-width: 900px;
  }

  .skills-list {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin: 24px 0 0;
    padding: 0;
    list-style: none;
  }

  .skills-list li,
  .project-tags span {
    display: inline-block;
    padding: 7px 12px;
    border: 1px solid #555555;
    border-radius: 999px;
    background: #1d1d1d;
    color: #dddddd;
    font-size: 0.95rem;
  }

  .project-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
    margin-top: 32px;
  }

  .project-card {
    display: block;
    overflow: hidden;
    border: 1px solid #3f3f3f;
    border-radius: 6px;
    background: #1a1a1a;
    color: inherit;
    text-decoration: none;
  }

  .project-card:hover {
    border-color: #888888;
    text-decoration: none;
  }

  .project-card img {
    display: block;
    width: 100%;
    aspect-ratio: 1 / 1;
    margin: 0;
    object-fit: cover;
    background: #242424;
  }

  .project-card-text {
    padding: 20px;
  }

  .project-card h3 {
    margin: 0 0 10px;
    color: #ffffff;
    font-size: 1.35rem;
  }

  .project-card p {
    margin: 0 0 16px;
    color: #c8c8c8;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .project-tags span {
    padding: 5px 9px;
    font-size: 0.82rem;
  }

  .project-detail {
    padding: 75px 0;
    border-bottom: 1px solid #333333;
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
    color: #d0d0d0;
  }

  .project-detail img {
    display: block;
    max-width: 100%;
    width: auto;
    height: auto;
    margin: 32px auto 32px 0;
    border: 1px solid #444444;
  }

  .return-link {
    margin-top: 35px;
  }

  .accessibility-note {
    max-width: 900px;
    color: #bdbdbd;
    font-size: 0.95rem;
  }

  @media screen and (max-width: 900px) {
    .project-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }
  }

  @media screen and (max-width: 600px) {
    .wrapper {
      width: 94%;
      padding-left: 10px;
      padding-right: 10px;
    }

    .portfolio-header {
      padding-top: 45px;
    }

    .project-grid {
      grid-template-columns: 1fr;
    }

    .contact-links {
      flex-direction: column;
      gap: 10px;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    html {
      scroll-behavior: auto;
    }
  }
</style>

<a class="skip-link" href="#main-content">Skip to main content</a>

<header class="portfolio-header">
  <h1>Your Name</h1>

  <p>
    GIS student interested in spatial analysis, cartography,
    geographic data visualisation and evidence-based spatial research.
  </p>

  <nav class="contact-links" aria-label="Contact links">
    <a href="https://www.linkedin.com/in/your-linkedin-name">
      LinkedIn
    </a>

    <a href="mailto:your-email@example.com">
      Email
    </a>
  </nav>
</header>

<main id="main-content">

  <section class="section" aria-labelledby="about-heading">
    <h2 id="about-heading">About</h2>

    <div class="about-text">
      <p>
        I am a GIS student developing experience in spatial analysis,
        cartographic design and geographic data visualisation.
        This portfolio presents selected projects completed during my studies.
      </p>

      <p>
        My work focuses on using geographic information to investigate
        spatial patterns, communicate findings clearly and support
        evidence-based decision-making.
      </p>
    </div>
  </section>

  <section class="section" aria-labelledby="skills-heading">
    <h2 id="skills-heading">Skills</h2>

    <p class="section-intro">
      Software, analytical methods and technical areas demonstrated across
      my projects.
    </p>

    <ul class="skills-list">
      <li>QGIS</li>
      <li>ArcGIS Pro</li>
      <li>Spatial analysis</li>
      <li>Cartographic design</li>
      <li>Data visualisation</li>
      <li>Remote sensing</li>
      <li>Geographic data management</li>
      <li>Map production</li>
    </ul>
  </section>

  <section class="section" aria-labelledby="projects-heading">
    <h2 id="projects-heading">Projects</h2>

    <p class="section-intro">
      Select a project to move to its full description, methods and results.
    </p>

    <div class="project-grid">

      <a class="project-card" href="#project-one">
        <img
          src="{{ '/assets/images/BlackImage.png' | relative_url }}"
          alt="Preview map from Project One">

        <div class="project-card-text">
          <h3>Project One</h3>

          <p>
            A short description explaining the purpose and main outcome
            of the first GIS project.
          </p>

          <div class="project-tags" aria-label="Project One tags">
            <span>Spatial analysis</span>
            <span>Cartography</span>
            <span>QGIS</span>
          </div>
        </div>
      </a>

      <a class="project-card" href="#project-two">
        <img
          src="{{ '/assets/images/BlackImage2.png' | relative_url }}"
          alt="Preview map from Project Two">

        <div class="project-card-text">
          <h3>Project Two</h3>

          <p>
            A short description explaining the purpose and main outcome
            of the second GIS project.
          </p>

          <div class="project-tags" aria-label="Project Two tags">
            <span>Data visualisation</span>
            <span>GIS analysis</span>
            <span>ArcGIS Pro</span>
          </div>
        </div>
      </a>

      <a class="project-card" href="#project-three">
        <img
          src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
          alt="Preview map from Project Three">

        <div class="project-card-text">
          <h3>Project Three</h3>

          <p>
            A short description explaining the purpose and main outcome
            of the third GIS project.
          </p>

          <div class="project-tags" aria-label="Project Three tags">
            <span>Mapping</span>
            <span>Research</span>
            <span>GIS</span>
          </div>
        </div>
      </a>

    </div>
  </section>

  <section class="project-detail" id="project-one" aria-labelledby="project-one-heading">
    <h2 id="project-one-heading">Project One</h2>

    <div class="project-tags" aria-label="Project One tags">
      <span>Spatial analysis</span>
      <span>Cartography</span>
      <span>QGIS</span>
    </div>

    <p>
      Write a short introduction explaining the question, problem or
      geographic area investigated in this project.
    </p>

    <img
      src="{{ '/assets/images/BlackImage.png' | relative_url }}"
      alt="Final map produced for Project One">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe the process clearly enough for a visitor to understand
      how the final result was produced.
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

    <div class="project-tags" aria-label="Project Two tags">
      <span>Data visualisation</span>
      <span>GIS analysis</span>
      <span>ArcGIS Pro</span>
    </div>

    <p>
      Write a short introduction explaining the question, problem or
      geographic area investigated in this project.
    </p>

    <img
      src="{{ '/assets/images/BlackImage2.png' | relative_url }}"
      alt="Final map produced for Project Two">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe the process clearly enough for a visitor to understand
      how the final result was produced.
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

    <div class="project-tags" aria-label="Project Three tags">
      <span>Mapping</span>
      <span>Research</span>
      <span>GIS</span>
    </div>

    <p>
      Write a short introduction explaining the question, problem or
      geographic area investigated in this project.
    </p>

    <img
      src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
      alt="Final map produced for Project Three">

    <h3>Data and methods</h3>

    <p>
      Explain the datasets, GIS software and analytical methods used.
      Describe the process clearly enough for a visitor to understand
      how the final result was produced.
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

  <section class="section" aria-labelledby="accessibility-heading">
    <h2 id="accessibility-heading">Accessibility</h2>

    <p class="accessibility-note">
      This website uses descriptive image text, keyboard-visible focus
      indicators, high-contrast colours and a responsive layout. Project
      maps should also include readable labels, legends and colour choices
      that remain understandable for users with colour-vision deficiencies.
    </p>
  </section>

</main>
