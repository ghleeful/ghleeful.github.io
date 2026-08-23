---
layout: about
title: Profile
permalink: /
subtitle: >
  <b>Postdoctoral Research Associate</b> at
  <a href="https://www.purdue.edu/" rel="external nofollow noopener" target="_blank">Purdue University</a>,
  Department of Chemistry

profile:
  align: right
  image: prof_pic01.jpg
  image_circular: false
  more_info: >
    <div id="profile-carousel" class="carousel slide profile-carousel" data-bs-ride="false">

      <div class="carousel-inner">
        <div class="carousel-item active">
          <img
            src="/assets/img/prof_pic01.jpg"
            alt="Gihyun Lee profile photograph 1"
          >
        </div>

        <div class="carousel-item">
          <img
            src="/assets/img/prof_pic02.jpg"
            alt="Gihyun Lee profile photograph 2"
          >
        </div>
      </div>

      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#profile-carousel"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Profile photograph 1"
        ></button>

        <button
          type="button"
          data-bs-target="#profile-carousel"
          data-bs-slide-to="1"
          aria-label="Profile photograph 2"
        ></button>
      </div>
    </div>

    <div class="profile-links">
      <a
        href="/assets/pdf/Gihyun%20Lee_CV.pdf"
        target="_blank"
        rel="noopener"
        aria-label="CV"
        title="Open CV"
      >CV</a>

      <a
        href="https://scholar.google.com/citations?user=FmEf7ccAAAAJ"
        target="_blank"
        rel="noopener"
        aria-label="Google Scholar"
        title="Google Scholar"
      >Scholar</a>

      <a
        href="https://www.linkedin.com/in/leegh"
        target="_blank"
        rel="noopener"
        aria-label="LinkedIn"
        title="LinkedIn"
      >LinkedIn</a>

      <a
        href="mailto:lee5919@purdue.edu"
        aria-label="Email"
        title="Email"
      >Email</a>
    </div>

selected_papers: false
social: false

announcements:
  enabled: false
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

<style>
  /* =========================================================
     Profile title
     ========================================================= */

  h1.post-title {
    font-size: 3.5rem !important;
    font-weight: 400;
    line-height: 1.08;
  }

  /* =========================================================
     Profile photograph carousel
     ========================================================= */

  /* Hide the single image generated automatically by al-folio */
  .profile > picture,
  .profile > figure,
  .profile > img {
    display: none !important;
  }

  .profile-carousel {
    position: relative;
    width: 100%;
  }

  .profile-carousel .carousel-inner,
  .profile-carousel .carousel-item {
    width: 100%;
    height: 500px;
  }

  .profile-carousel .carousel-item img {
    display: block;
    width: 100%;
    height: 500px;
    border-radius: 0 !important;
    object-fit: cover;
    object-position: center;
  }

  /* Remove previous and next arrows */
  .profile-carousel .carousel-control-prev,
  .profile-carousel .carousel-control-next {
    display: none !important;
  }

  /* Dots below the photographs */
  .profile-carousel .carousel-indicators {
    position: static;
    display: flex;
    justify-content: center;
    gap: 0.45rem;
    margin: 0.75rem 0 0;
  }

  .profile-carousel .carousel-indicators [data-bs-target] {
    width: 9px;
    height: 9px;
    margin: 0;
    padding: 0;
    border: 1px solid var(--global-text-color-light);
    border-radius: 50%;
    background-color: transparent;
    opacity: 1;
  }

  .profile-carousel .carousel-indicators .active {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
  }

  /* =========================================================
     Buttons below the profile photographs
     ========================================================= */

  .profile-links {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.45rem;
    margin-top: 0.75rem;
  }

  .profile-links a {
    padding: 0.3rem 0.65rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.78rem;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
  }

  .profile-links a:hover {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
    color: var(--global-hover-text-color) !important;
    text-decoration: none;
  }

  /* =========================================================
     Education, Experience, Awards, and Expertise toggles
     ========================================================= */

  .profile-sections {
    width: 250px;
    max-width: 100%;
    margin-top: 2rem;
  }

  details.cv-toggle {
    margin: 0;
    padding: 0.55rem 0;
    border: 0 !important;
  }

  .cv-toggle summary {
    display: flex;
    align-items: center;
    width: 250px;
    max-width: 100%;
    padding-bottom: 0.25rem;
    border-bottom: 1px solid var(--global-divider-color);
    list-style: none;
    cursor: pointer;
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 600;
  }

  .cv-toggle summary::-webkit-details-marker {
    display: none;
  }

  .cv-toggle summary::marker {
    content: "";
  }

  .cv-toggle summary::before {
    width: 1.2rem;
    margin-right: 0.25rem;
    color: var(--global-theme-color);
    font-size: 1.1rem;
    font-weight: 700;
    content: "+";
  }

  .cv-toggle[open] summary::before {
    content: "−";
  }

  .cv-toggle-content {
    padding: 0.8rem 0 0.1rem 1.2rem;
    font-size: 0.92rem;
    line-height: 1.5;
  }

  .cv-entry {
    margin: 0 0 0.9rem;
  }

  .cv-entry:last-child {
    margin-bottom: 0.3rem;
  }

  .cv-entry span {
    color: var(--global-text-color-light);
  }

  /* =========================================================
     University logos
     ========================================================= */

  .affiliation-logos {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 4.5rem;
    width: 100%;
    margin-top: 2.5rem;
    padding: 1.3rem 0 1rem;
    border-top: 1px solid var(--global-divider-color);
  }

  .affiliation-logos a {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .affiliation-logos img {
    display: block;
    width: auto;
    object-fit: contain;
  }

  /* Optical sizes are intentionally different */
  .affiliation-logo-uvic {
    height: 42px;
  }

  .affiliation-logo-yonsei {
    height: 49px;
  }

  .affiliation-logo-purdue {
    height: 44px;
  }

  /* =========================================================
     Desktop profile positioning
     ========================================================= */

  @media (min-width: 576px) {
    .profile {
      width: 26% !important;
      max-width: 530px;
      margin-left: 3rem !important;
      margin-bottom: 1.5rem !important;
      transform: translateY(-6.5rem);
    }
  }

  /* =========================================================
     Mobile layout
     ========================================================= */

  @media (max-width: 575px) {
    h1.post-title {
      font-size: 2.55rem !important;
    }

    .profile-carousel .carousel-inner,
    .profile-carousel .carousel-item,
    .profile-carousel .carousel-item img {
      height: 390px;
    }

    .profile-links {
      margin-top: 0.6rem;
    }

    .profile-links a {
      padding: 0.25rem 0.5rem;
      font-size: 0.72rem;
    }

    .profile-sections {
      width: 220px;
    }

    .cv-toggle summary {
      width: 220px;
    }

    .affiliation-logos {
      flex-wrap: wrap;
      gap: 1.6rem 2.2rem;
      margin-top: 2rem;
      padding: 1rem 0 0.75rem;
    }

    .affiliation-logo-uvic {
      height: 31px;
    }

    .affiliation-logo-yonsei {
      height: 36px;
    }

    .affiliation-logo-purdue {
      height: 33px;
    }
  }
</style>

Hi there! Welcome to my website. :)

I’m Gihyun Lee, a postdoctoral research associate at Purdue University, USA.

My research interests lie in functional and responsive coordination materials, particularly in understanding how molecular properties change upon incorporation into crystalline solids. Please take a look at my publication list in the tab in the upper right corner for more information.

Feel free to [email](mailto:lee5919@purdue.edu "lee5919@purdue.edu") me if you are interested in collaborating. You are always welcome!

<div class="profile-sections">
  <details class="cv-toggle">
    <summary>Education</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        <strong>Ph.D. in Chemistry</strong><br>
        <span>Yonsei University · 20XX–20XX</span><br>
        <span>Advisor: Professor Moonhyun Oh</span>
      </p>

      <p class="cv-entry">
        <strong>M.S. in Chemistry</strong><br>
        <span>University Name · 20XX–20XX</span>
      </p>

      <p class="cv-entry">
        <strong>B.S. in Chemistry</strong><br>
        <span>University Name · 20XX–20XX</span>
      </p>
    </div>
  </details>

  <details class="cv-toggle">
    <summary>Experience</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        <strong>Postdoctoral Research Associate</strong><br>
        <span>Purdue University · 20XX–Present</span>
      </p>

      <p class="cv-entry">
        <strong>Previous Position</strong><br>
        <span>Institution Name · 20XX–20XX</span>
      </p>
    </div>
  </details>

  <details class="cv-toggle">
    <summary>Selected Awards</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        <strong>Award Name</strong><br>
        <span>Organization · Year</span>
      </p>

      <p class="cv-entry">
        <strong>Award Name</strong><br>
        <span>Organization · Year</span>
      </p>
    </div>
  </details>

  <details class="cv-toggle">
    <summary>Expertise</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        Metal–organic frameworks, coordination chemistry, ligand synthesis,
        single-crystal X-ray diffraction, responsive crystalline materials,
        and structure–property relationships.
      </p>
    </div>
  </details>
</div>

<div class="affiliation-logos">
  <a
    href="https://www.uvic.ca/"
    target="_blank"
    rel="noopener"
    aria-label="University of Victoria"
  >
    <img
      class="affiliation-logo-uvic"
      src="/assets/img/uvic-logo.png"
      alt="University of Victoria"
    >
  </a>

  <a
    href="https://www.yonsei.ac.kr/"
    target="_blank"
    rel="noopener"
    aria-label="Yonsei University"
  >
    <img
      class="affiliation-logo-yonsei"
      src="/assets/img/yonsei-logo.png"
      alt="Yonsei University"
    >
  </a>

  <a
    href="https://www.purdue.edu/"
    target="_blank"
    rel="noopener"
    aria-label="Purdue University"
  >
    <img
      class="affiliation-logo-purdue"
      src="/assets/img/purdue-logo.png"
      alt="Purdue University"
    >
  </a>
</div>

<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.9.3/dist/confetti.browser.min.js"></script>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) {
      return;
    }

    confetti({
      particleCount: 80,
      angle: 55,
      spread: 65,
      startVelocity: 42,
      gravity: 0.9,
      ticks: 180,
      origin: {
        x: 0,
        y: 0.85,
      },
      colors: ["#8c6a24", "#cfb991", "#f5f3ee", "#ffffff"],
      disableForReducedMotion: true,
    });
  });
</script>
