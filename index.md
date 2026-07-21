---
layout: default
title: GIS Portfolio
---

<style>
  /* Widen Minima's default page layout */
  .wrapper {
    max-width: 1400px;
    width: 92%;
    padding-left: 20px;
    padding-right: 20px;
  }

  .page-content {
    padding-top: 40px;
  }

  .portfolio-intro {
    max-width: 900px;
    margin-bottom: 50px;
  }

  /* Three project cards in one row */
  .project-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
    margin: 30px 0 80px;
  }

  .project-card {
    display: block;
    overflow: hidden;
    border: 1px solid #cccccc;
    background: #ffffff;
    color: inherit;
    text-decoration: none;
  }

  .project-card:hover,
  .project-card:focus {
    border-color: #444444;
    text-decoration: none;
  }

  .project-card img {
    display: block;
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    margin: 0;
    background: #eeeeee;
  }

  .project-card-text {
    padding: 18px;
  }

  .project-card h2 {
    margin: 0 0 8px;
    font-size: 1.3rem;
  }

  .project-card p {
    margin: 0;
    color: #555555;
  }

  /* Detailed project sections */
  .project-detail {
    padding: 70px 0;
    border-top: 1px solid #dddddd;
    scroll-margin-top: 30px;
  }

  .project-detail h2,
  .project-detail h3,
  .project-detail p {
    max-width: 900px;
  }

  .project-detail img {
    display: block;
    max-width: 100%;
    width: auto;
    height: auto;
    margin: 30px auto 30px 0;
  }

  .return-link {
    margin-top: 35px;
  }

  /* Two columns on medium screens */
  @media screen and (max-width: 900px) {
    .project-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }
  }

  /* One column on phones */
  @media screen and (max-width: 600px) {
    .wrapper {
      width: 94%;
      padding-left: 10px;
      padding-right: 10px;
    }

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
      src="{{ '/assets/images/BlackImage.png' | relative_url }}"
      alt="Map from Project One">

    <div class="project-card-text">
      <h2>Project One</h2>
      <p>A short description of the first GIS project.</p>
    </div>
  </a>

  <a class="project-card" href="#project-two">
    <img
      src="{{ '/assets/images/Blackimage2.png' | relative_url }}"
      alt="Map from Project Two">

    <div class="project-card-text">
      <h2>Project Two</h2>
      <p>A short description of the second GIS project.</p>
    </div>
  </a>

  <a class="project-card" href="#project-three">
    <img
      src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
      alt="Map from Project Three">

    <div class="project-card-text">
      <h2>Project Three</h2>
      <p>A short description of the third GIS project.</p>
    </div>
  </a>

</div>

<div class="project-detail" id="project-one">
  <h2>Project One</h2>

  <p>
    Write a short introduction explaining the question or problem
    investigated in this project.
  </p>

  <img
    src="{{ '/assets/images/BlackImage.png' | relative_url }}"
    alt="Main map from Project One">

  <h3>Data and methods</h3>

  <p>
    Explain the datasets, GIS software and analytical methods used.
  </p>

  <h3>Results</h3>

  <p>
    Explain the main findings and what the map demonstrates.
  </p>

  <p class="return-link">
    <a href="#projects">Return to projects</a>
  </p>
</div>

<div class="project-detail" id="project-two">
  <h2>Project Two</h2>

  <p>
    Write a short introduction explaining the question or problem
    investigated in this project.
  </p>

  <img
    src="{{ '/assets/images/Blackimage2.png' | relative_url }}"
    alt="Main map from Project Two">

  <h3>Data and methods</h3>

  <p>
    Explain the datasets, GIS software and analytical methods used.
  </p>

  <h3>Results</h3>

  <p>
    Explain the main findings and what the map demonstrates.
  </p>

  <p class="return-link">
    <a href="#projects">Return to projects</a>
  </p>
</div>

<div class="project-detail" id="project-three">
  <h2>Project Three</h2>

  <p>
    Write a short introduction explaining the question or problem
    investigated in this project.
  </p>

  <img
    src="{{ '/assets/images/BlackImage3.png' | relative_url }}"
    alt="Main map from Project Three">

  <h3>Data and methods</h3>

  <p>
    Explain the datasets, GIS software and analytical methods used.
  </p>

  <h3>Results</h3>

  <p>
    Explain the main findings and what the map demonstrates.
  </p>

  <p class="return-link">
    <a href="#projects">Return to projects</a>
  </p>
</div>
