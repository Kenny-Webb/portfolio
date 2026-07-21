---
layout: default
title: GIS Portfolio
---

<style>
  .portfolio-intro {
    margin-bottom: 40px;
  }

  .project-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 24px;
    margin: 30px 0 70px;
  }

  .project-card {
    display: block;
    border: 1px solid #cccccc;
    padding: 16px;
    color: inherit;
    text-decoration: none;
    background: white;
  }

  .project-card:hover,
  .project-card:focus {
    border-color: #333333;
    text-decoration: none;
  }

  .project-card img {
    display: block;
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    margin-bottom: 15px;
  }

  .project-card h2 {
    margin: 0 0 8px;
    font-size: 1.3rem;
  }

  .project-card p {
    margin: 0;
  }

  .project-detail {
    padding: 50px 0;
    border-top: 1px solid #dddddd;
  }

  .project-detail img {
    display: block;
    width: 100%;
    height: auto;
    margin: 25px 0;
  }

  @media screen and (max-width: 650px) {
    .project-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="portfolio-intro">
  <h1>Your Name</h1>

  <p>
    I am a GIS student interested in spatial analysis, cartography
    and geographic data visualisation.
  </p>
</div>

<h2 id="projects">Projects</h2>

<div class="project-grid">

  <a class="project-card" href="#project-one">
    <img
      src="{{ '/BlackImage.png' | relative_url }}"
      alt="Map from Project One">
    <h2>Project One</h2>
    <p>A short one-sentence description of the project.</p>
  </a>

  <a class="project-card" href="#project-two">
    <img
      src="{{ '/Blackimage2.png' | relative_url }}"
      alt="Map from Project Two">
    <h2>Project Two</h2>
    <p>A short one-sentence description of the project.</p>
  </a>

</div>

<div class="project-detail" id="project-one">
  <h2>Project One</h2>

  <p>
    Write a short introduction explaining the question you investigated.
  </p>

  <img
    src="{{ '/assets/images/Blackimage2.png' | relative_url }}"
    alt="Main map from Project One">

  <h3>Methods</h3>

  <p>
    Explain the data, software and analysis you used.
  </p>

  <h3>Results</h3>

  <p>
    Explain what you found and what the map demonstrates.
  </p>

  <p><a href="#projects">Return to projects</a></p>
</div>

<div class="project-detail" id="project-two">
  <h2>Project Two</h2>

  <p>
    Write a short introduction explaining the project.
  </p>

  <img
    src="{{ '/assets/images/BlackImage.png' | relative_url }}"
    alt="Main map from Project Two">

  <h3>Methods</h3>

  <p>
    Explain the data, software and analysis you used.
  </p>

  <h3>Results</h3>

  <p>
    Explain the main findings.
  </p>

  <p><a href="#projects">Return to projects</a></p>
</div>
