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
  image: profile-01.png
  image_circular: false
  more_info: >
    <div class="profile-dots" aria-label="Profile image selector">
      <button
        class="profile-dot active"
        type="button"
        data-image="/assets/img/profile-01.png"
        aria-label="Show profile image 1"
      ></button>
      <button
        class="profile-dot"
        type="button"
        data-image="/assets/img/profile-02.jpg"
        aria-label="Show profile image 2"
      ></button>
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
  /* Main profile heading */
  h1.post-title {
    font-size: 3.4rem !important;
    line-height: 1.1;
  }

  /* Profile image */
  .profile img {
    width: 100% !important;
    height: 430px !important;
    border-radius: 0 !important;
    object-fit: cover;
    object-position: center;
    transition: opacity 0.22s ease;
  }

  .profile img.profile-image-changing {
    opacity: 0.25;
  }

  /* Slideshow dots */
  .profile-dots {
    display: flex;
    justify-content: center;
    gap: 0.45rem;
    margin: 0.65rem 0 0.7rem;
  }

  .profile-dot {
    width: 9px;
    height: 9px;
    padding: 0;
    border: 1px solid var(--global-text-color-light);
    border-radius: 50%;
    background: transparent;
    cursor: pointer;
    transition:
      background-color 0.18s ease,
      border-color 0.18s ease,
      transform 0.18s ease;
  }

  .profile-dot:hover {
    border-color: var(--global-theme-color);
    transform: scale(1.12);
  }

  .profile-dot.active {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
  }

  /* Links below profile image */
  .profile-links {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.45rem;
  }

  .profile-links a {
    padding: 0.3rem 0.65rem;
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color) !important;
    font-size: 0.78rem;
    font-weight: 500;
    line-height: 1.2;
    text-decoration: none;
    transition:
      color 0.18s ease,
      border-color 0.18s ease,
      background-color 0.18s ease;
  }

  .profile-links a:hover {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
    color: var(--global-hover-text-color) !important;
    text-decoration: none;
  }

  /* Education, Experience, Awards and Expertise toggles */
  .cv-section {
    width: 100%;
    max-width: 350px;
    margin-top: 2rem;
  }

  details.cv-toggle,
  details.cv-toggle:last-of-type {
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
    padding: 0.8rem 0 0.1rem 1.45rem;
    color: var(--global-text-color);
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

  /* Institution logos */
  .institution-logos {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: clamp(2rem, 5vw, 4.5rem);
    width: 100%;
    margin: 2.2rem auto 0.7rem;
    padding: 1.2rem 0 0.6rem;
    border-top: 1px solid var(--global-divider-color);
  }

  .institution-logos a {
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
  }

  .institution-logos img {
    display: block;
    width: auto;
    object-fit: contain;
    transition:
      opacity 0.18s ease,
      transform 0.18s ease;
  }

  .institution-logos a:hover img {
    opacity: 0.78;
    transform: translateY(-2px);
  }

  .institution-logo-uvic {
    height: 42px;
  }

  .institution-logo-yonsei {
    height: 45px;
  }

  .institution-logo-purdue {
    height: 39px;
  }

  /* Left-side welcome fanfare */
  .welcome-fanfare {
    position: fixed;
    z-index: 2000;
    top: 4.5rem;
    left: 0;
    width: 190px;
    height: 230px;
    overflow: hidden;
    pointer-events: none;
  }

  .welcome-confetti {
    position: absolute;
    top: 45%;
    left: -15px;
    width: 7px;
    height: 13px;
    border-radius: 1px;
    opacity: 0;
    animation: welcome-confetti-burst 1.45s ease-out forwards;
  }

  @keyframes welcome-confetti-burst {
    0% {
      opacity: 0;
      transform: translate(0, 0) rotate(0deg) scale(0.7);
    }

    12% {
      opacity: 1;
    }

    100% {
      opacity: 0;
      transform:
        translate(var(--confetti-x), var(--confetti-y))
        rotate(var(--confetti-rotation))
        scale(1);
    }
  }

  /* Desktop profile layout */
  @media (min-width: 576px) {
    .profile {
      width: 26% !important;
      max-width: 530px;
      margin-left: 3rem !important;
      margin-bottom: 1.5rem !important;
      transform: translateY(-6.5rem);
    }
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    h1.post-title {
      font-size: 2.6rem !important;
    }

    .profile img {
      height: 360px !important;
    }

    .profile-links {
      margin-top: 0.5rem;
    }

    .profile-links a {
      padding: 0.25rem 0.5rem;
      font-size: 0.72rem;
    }

    .cv-section {
      margin-top: 1.5rem;
    }

    .cv-toggle summary {
      width: 220px;
    }

    .institution-logos {
      gap: 1.3rem;
      margin-top: 1.6rem;
      padding-top: 1rem;
    }

    .institution-logo-uvic {
      height: 28px;
    }

    .institution-logo-yonsei {
      height: 31px;
    }

    .institution-logo-purdue {
      height: 26px;
    }

    .welcome-fanfare {
      top: 3.5rem;
      width: 135px;
      height: 180px;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .welcome-fanfare {
      display: none;
    }

    .profile img,
    .institution-logos img,
    .profile-dot {
      transition: none;
    }
  }
</style>

Hi there! Welcome to my website. :)

I’m Gihyun Lee, a postdoctoral research associate at Purdue University, USA.

My research interests lie in functional and responsive coordination materials, particularly in understanding how molecular properties change upon incorporation into crystalline solids. Please take a look at my publication list in the tab in the upper right corner for more information.

Feel free to [email](mailto:lee5919@purdue.edu "lee5919@purdue.edu") me if you are interested in collaborating. You are always welcome!

<div class="cv-section">
  <details class="cv-toggle">
    <summary>Education</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        <strong>Ph.D. in Chemistry</strong><br>
        <span>University Name · 20XX–20XX</span><br>
        <span>Advisor: Professor Name</span>
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
        <span>Awarding organization · Year</span>
      </p>

      <p class="cv-entry">
        <strong>Award Name</strong><br>
        <span>Awarding organization · Year</span>
      </p>
    </div>
  </details>

  <details class="cv-toggle">
    <summary>Expertise</summary>

    <div class="cv-toggle-content">
      <p class="cv-entry">
        Metal–organic frameworks · Coordination chemistry · Functional crystalline solids
      </p>

      <p class="cv-entry">
        Single-crystal X-ray diffraction · Materials characterization · Ligand synthesis
      </p>
    </div>
  </details>
</div>

<div class="institution-logos">
  <a
    href="https://www.uvic.ca/"
    target="_blank"
    rel="noopener"
    aria-label="University of Victoria"
  >
    <img
      class="institution-logo-uvic"
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
      class="institution-logo-yonsei"
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
      class="institution-logo-purdue"
      src="/assets/img/purdue-logo.png"
      alt="Purdue University"
    >
  </a>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const profileImage = document.querySelector(".profile img");
    const profileDots = Array.from(document.querySelectorAll(".profile-dot"));

    if (profileImage && profileDots.length > 0) {
      profileDots.forEach(function (dot) {
        dot.addEventListener("click", function () {
          const nextImage = dot.dataset.image;

          if (!nextImage || dot.classList.contains("active")) {
            return;
          }

          profileImage.classList.add("profile-image-changing");

          const imageLoader = new Image();

          imageLoader.addEventListener("load", function () {
            profileImage.src = nextImage;
            profileImage.alt = dot.getAttribute("aria-label") || "Profile image";

            profileDots.forEach(function (item) {
              item.classList.remove("active");
            });

            dot.classList.add("active");

            window.setTimeout(function () {
              profileImage.classList.remove("profile-image-changing");
            }, 60);
          });

          imageLoader.src = nextImage;
        });
      });
    }

    if (
      window.matchMedia("(prefers-reduced-motion: reduce)").matches ||
      sessionStorage.getItem("profile-fanfare-shown") === "true"
    ) {
      return;
    }

    sessionStorage.setItem("profile-fanfare-shown", "true");

    const fanfare = document.createElement("div");
    fanfare.className = "welcome-fanfare";
    fanfare.setAttribute("aria-hidden", "true");

    const colors = ["#8c6a24", "#cfb991", "#f1d6dc", "#26231f", "#ffffff"];

    for (let index = 0; index < 34; index += 1) {
      const confetti = document.createElement("span");
      const angle = -78 + Math.random() * 156;
      const distance = 75 + Math.random() * 115;
      const radians = (angle * Math.PI) / 180;

      confetti.className = "welcome-confetti";
      confetti.style.backgroundColor =
        colors[Math.floor(Math.random() * colors.length)];
      confetti.style.animationDelay = `${Math.random() * 0.22}s`;
      confetti.style.setProperty(
        "--confetti-x",
        `${Math.cos(radians) * distance}px`,
      );
      confetti.style.setProperty(
        "--confetti-y",
        `${Math.sin(radians) * distance}px`,
      );
      confetti.style.setProperty(
        "--confetti-rotation",
        `${180 + Math.random() * 520}deg`,
      );

      fanfare.appendChild(confetti);
    }

    document.body.appendChild(fanfare);

    window.setTimeout(function () {
      fanfare.remove();
    }, 1900);
  });
</script>
