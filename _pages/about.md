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
    <div class="profile-carousel" aria-label="Profile photo gallery">
      <div class="profile-carousel-viewport">
        <img
          class="profile-carousel-image active"
          src="/assets/img/profile-01.png"
          alt="Gihyun Lee profile photo 1"
        >
        <img
          class="profile-carousel-image"
          src="/assets/img/profile-02.jpg"
          alt="Gihyun Lee profile photo 2"
        >

        <button
          class="profile-carousel-arrow profile-carousel-prev"
          type="button"
          aria-label="Previous photo"
        >
          ‹
        </button>

        <button
          class="profile-carousel-arrow profile-carousel-next"
          type="button"
          aria-label="Next photo"
        >
          ›
        </button>
      </div>

      <div class="profile-carousel-dots" aria-label="Select profile photo">
        <button
          class="profile-carousel-dot active"
          type="button"
          aria-label="Show photo 1"
          aria-current="true"
        ></button>
        <button
          class="profile-carousel-dot"
          type="button"
          aria-label="Show photo 2"
          aria-current="false"
        ></button>
      </div>
    </div>

    <div class="profile-links">
      <a href="/assets/pdf/Gihyun%20Lee_CV.pdf" target="_blank" aria-label="CV" title="Open CV">CV</a>
      <a href="https://scholar.google.com/citations?user=FmEf7ccAAAAJ" target="_blank" aria-label="Google Scholar" title="Google Scholar">Scholar</a>
      <a href="https://www.linkedin.com/in/leegh" target="_blank" aria-label="LinkedIn" title="LinkedIn">LinkedIn</a>
      <a href="mailto:lee5919@purdue.edu" aria-label="Email" title="Email">Email</a>
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
  /* Page title */
  h1.post-title {
    font-size: 3.4rem !important;
    line-height: 1.1;
  }

  /* Hide the original al-folio profile image after the carousel loads */
  .profile > img,
  .profile > figure,
  .profile > picture {
    display: none !important;
  }

  /* Profile carousel */
  .profile-carousel {
    position: relative;
    width: 100%;
  }

  .profile-carousel-viewport {
    position: relative;
    width: 100%;
    overflow: hidden;
    background-color: var(--global-card-bg-color);
    box-shadow: 0 0.2rem 0.75rem rgba(0, 0, 0, 0.12);
  }

  .profile-carousel-image {
    display: none;
    width: 100%;
    height: auto;
    border-radius: 0 !important;
    object-fit: cover;
  }

  .profile-carousel-image.active {
    display: block;
  }

  /* Carousel arrows */
  .profile-carousel-arrow {
    position: absolute;
    top: 50%;
    z-index: 2;
    display: flex;
    width: 2rem;
    height: 2.5rem;
    padding: 0;
    border: 0;
    align-items: center;
    justify-content: center;
    background-color: rgba(38, 35, 31, 0.72);
    color: #ffffff;
    cursor: pointer;
    font-family: Arial, sans-serif;
    font-size: 1.8rem;
    font-weight: 400;
    line-height: 1;
    opacity: 0;
    transform: translateY(-50%);
    transition:
      opacity 0.18s ease,
      background-color 0.18s ease;
  }

  .profile-carousel:hover .profile-carousel-arrow,
  .profile-carousel:focus-within .profile-carousel-arrow {
    opacity: 1;
  }

  .profile-carousel-arrow:hover,
  .profile-carousel-arrow:focus-visible {
    background-color: var(--global-theme-color);
    outline: none;
  }

  .profile-carousel-prev {
    left: 0.45rem;
  }

  .profile-carousel-next {
    right: 0.45rem;
  }

  /* Carousel dots */
  .profile-carousel-dots {
    display: flex;
    min-height: 1.5rem;
    margin-top: 0.5rem;
    align-items: center;
    justify-content: center;
    gap: 0.45rem;
  }

  .profile-carousel-dot {
    width: 0.48rem;
    height: 0.48rem;
    padding: 0;
    border: 1px solid var(--global-text-color-light);
    border-radius: 50%;
    background-color: transparent;
    cursor: pointer;
  }

  .profile-carousel-dot.active {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
  }

  /* Links below profile pictures */
  .profile-links {
    display: flex;
    flex-wrap: wrap;
    margin-top: 0.45rem;
    align-items: center;
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
  }

  .profile-links a:hover {
    border-color: var(--global-theme-color);
    background-color: var(--global-theme-color);
    color: #ffffff !important;
  }

  /* CV toggles */
  details.cv-toggle:first-of-type {
    margin-top: 2.25rem;
  }

  details.cv-toggle,
  details.cv-toggle:last-of-type {
    padding: 0.55rem 0;
    border: 0 !important;
  }

  .cv-toggle summary {
    display: flex;
    width: 250px;
    max-width: calc(100vw - 2rem);
    padding-bottom: 0.25rem;
    border-bottom: 1px solid var(--global-divider-color);
    align-items: center;
    color: var(--global-text-color);
    cursor: pointer;
    font-size: 1rem;
    font-weight: 600;
    list-style: none;
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
    content: "+";
    font-size: 1.1rem;
    font-weight: 700;
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

  .cv-entry span {
    color: var(--global-text-color-light);
  }

  /* Institution logos */
  .institution-logos {
    display: flex;
    width: 100%;
    margin: 1.8rem auto 0;
    padding: 1.25rem 0 0.65rem;
    border-top: 1px solid var(--global-divider-color);
    align-items: center;
    justify-content: center;
    gap: clamp(1.5rem, 5vw, 4.5rem);
  }

  .institution-logo-link {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .institution-logo {
    display: block;
    width: auto;
    object-fit: contain;
  }

  /* Visually balanced logo sizes */
  .institution-logo.uvic {
    height: 42px;
  }

  .institution-logo.yonsei {
    height: 48px;
  }

  .institution-logo.purdue {
    height: 44px;
  }

  /* Desktop layout */
  @media (min-width: 576px) {
    .profile {
      width: 26% !important;
      max-width: 530px;
      margin-bottom: 1.5rem !important;
      margin-left: 3rem !important;
      transform: translateY(-6.5rem);
    }
  }

  /* Mobile layout */
  @media (max-width: 575px) {
    h1.post-title {
      font-size: 2.5rem !important;
    }

    .profile-carousel-arrow {
      width: 1.8rem;
      height: 2.2rem;
      font-size: 1.5rem;
      opacity: 0.82;
    }

    .profile-links {
      margin-top: 0.35rem;
    }

    .profile-links a {
      padding: 0.25rem 0.5rem;
      font-size: 0.72rem;
    }

    .cv-toggle summary {
      width: 220px;
      max-width: 100%;
    }

    .institution-logos {
      flex-wrap: wrap;
      gap: 1.1rem 1.6rem;
    }

    .institution-logo.uvic {
      height: 32px;
    }

    .institution-logo.yonsei {
      height: 37px;
    }

    .institution-logo.purdue {
      height: 34px;
    }
  }
</style>

Hi there! Welcome to my website. :)

I’m Gihyun Lee, a postdoctoral research associate at Purdue University, USA.

My research interests lie in functional and responsive coordination materials, particularly in understanding how molecular properties change upon incorporation into crystalline solids. Please take a look at my publication list in the tab in the upper right corner for more information.

Feel free to [email](mailto:lee5919@purdue.edu "lee5919@purdue.edu") me if you are interested in collaborating. You are always welcome!

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
      Metal–organic frameworks · Coordination chemistry · Single-crystal X-ray diffraction
    </p>

    <p class="cv-entry">
      Functional ligands · Responsive crystalline materials · Structure–property relationships
    </p>
  </div>
</details>

<div class="institution-logos">
  <a
    class="institution-logo-link"
    href="https://www.uvic.ca/"
    target="_blank"
    rel="external nofollow noopener"
    aria-label="University of Victoria"
  >
    <img
      class="institution-logo uvic"
      src="/assets/img/uvic-logo.png"
      alt="University of Victoria"
    >
  </a>

  <a
    class="institution-logo-link"
    href="https://www.yonsei.ac.kr/"
    target="_blank"
    rel="external nofollow noopener"
    aria-label="Yonsei University"
  >
    <img
      class="institution-logo yonsei"
      src="/assets/img/yonsei-logo.png"
      alt="Yonsei University"
    >
  </a>

  <a
    class="institution-logo-link"
    href="https://www.purdue.edu/"
    target="_blank"
    rel="external nofollow noopener"
    aria-label="Purdue University"
  >
    <img
      class="institution-logo purdue"
      src="/assets/img/purdue-logo.png"
      alt="Purdue University"
    >
  </a>
</div>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    const profile = document.querySelector(".profile");
    const carousel = profile?.querySelector(".profile-carousel");

    if (!profile || !carousel) return;

    /*
     * al-folio still renders profile.image.
     * Hide that original image and place the custom carousel first.
     */
    const originalImages = Array.from(profile.querySelectorAll("img")).filter(
      (image) => !image.classList.contains("profile-carousel-image")
    );

    originalImages.forEach((image) => {
      const logo = image.closest(".institution-logo-link");

      if (!logo) {
        image.style.display = "none";
      }
    });

    profile.insertBefore(carousel, profile.firstChild);

    const slides = Array.from(
      carousel.querySelectorAll(".profile-carousel-image")
    );
    const dots = Array.from(
      carousel.querySelectorAll(".profile-carousel-dot")
    );
    const previousButton = carousel.querySelector(
      ".profile-carousel-prev"
    );
    const nextButton = carousel.querySelector(".profile-carousel-next");

    if (slides.length < 2) return;

    let currentIndex = 0;
    let touchStartX = 0;

    const showSlide = (index) => {
      currentIndex = (index + slides.length) % slides.length;

      slides.forEach((slide, slideIndex) => {
        slide.classList.toggle("active", slideIndex === currentIndex);
      });

      dots.forEach((dot, dotIndex) => {
        const active = dotIndex === currentIndex;

        dot.classList.toggle("active", active);
        dot.setAttribute("aria-current", active ? "true" : "false");
      });
    };

    previousButton?.addEventListener("click", () => {
      showSlide(currentIndex - 1);
    });

    nextButton?.addEventListener("click", () => {
      showSlide(currentIndex + 1);
    });

    dots.forEach((dot, index) => {
      dot.addEventListener("click", () => {
        showSlide(index);
      });
    });

    carousel.setAttribute("tabindex", "0");

    carousel.addEventListener("keydown", (event) => {
      if (event.key === "ArrowLeft") {
        showSlide(currentIndex - 1);
      }

      if (event.key === "ArrowRight") {
        showSlide(currentIndex + 1);
      }
    });

    carousel.addEventListener(
      "touchstart",
      (event) => {
        touchStartX = event.changedTouches[0].clientX;
      },
      { passive: true }
    );

    carousel.addEventListener(
      "touchend",
      (event) => {
        const touchEndX = event.changedTouches[0].clientX;
        const distance = touchEndX - touchStartX;

        if (Math.abs(distance) < 40) return;

        if (distance > 0) {
          showSlide(currentIndex - 1);
        } else {
          showSlide(currentIndex + 1);
        }
      },
      { passive: true }
    );

    showSlide(0);
  });
</script>
<!-- Subtle corner confetti -->
<canvas id="profile-confetti" aria-hidden="true"></canvas>

<style>
  #profile-confetti {
    position: fixed;
    inset: 0;
    z-index: 9999;
    width: 100%;
    height: 100%;
    pointer-events: none;
  }

  @media (prefers-reduced-motion: reduce) {
    #profile-confetti {
      display: none;
    }
  }
</style>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    if (
      window.matchMedia("(prefers-reduced-motion: reduce)").matches ||
      sessionStorage.getItem("profileConfettiShown")
    ) {
      return;
    }

    sessionStorage.setItem("profileConfettiShown", "true");

    const canvas = document.getElementById("profile-confetti");
    const context = canvas.getContext("2d");
    const colors = ["#8c6a24", "#cfb991", "#26231f", "#f5f3ee"];
    const particles = [];
    const particleCount = window.innerWidth < 576 ? 36 : 70;
    const duration = 1400;
    const startTime = performance.now();

    function resizeCanvas() {
      const ratio = window.devicePixelRatio || 1;

      canvas.width = window.innerWidth * ratio;
      canvas.height = window.innerHeight * ratio;
      canvas.style.width = `${window.innerWidth}px`;
      canvas.style.height = `${window.innerHeight}px`;

      context.setTransform(ratio, 0, 0, ratio, 0, 0);
    }

    function createParticle(side) {
      const direction = side === "left" ? 1 : -1;

      return {
        x: side === "left" ? -8 : window.innerWidth + 8,
        y: Math.random() * 55,
        vx: direction * (2.5 + Math.random() * 5),
        vy: 1.5 + Math.random() * 4,
        gravity: 0.065 + Math.random() * 0.035,
        rotation: Math.random() * Math.PI,
        rotationSpeed: (Math.random() - 0.5) * 0.22,
        width: 4 + Math.random() * 6,
        height: 2 + Math.random() * 4,
        color: colors[Math.floor(Math.random() * colors.length)],
        opacity: 0.8 + Math.random() * 0.2,
      };
    }

    resizeCanvas();

    for (let index = 0; index < particleCount; index += 1) {
      particles.push(createParticle(index % 2 === 0 ? "left" : "right"));
    }

    function animate(currentTime) {
      const elapsed = currentTime - startTime;
      const progress = Math.min(elapsed / duration, 1);

      context.clearRect(0, 0, window.innerWidth, window.innerHeight);

      particles.forEach(function (particle) {
        particle.x += particle.vx;
        particle.y += particle.vy;
        particle.vy += particle.gravity;
        particle.rotation += particle.rotationSpeed;

        context.save();
        context.globalAlpha = particle.opacity * (1 - progress);
        context.translate(particle.x, particle.y);
        context.rotate(particle.rotation);
        context.fillStyle = particle.color;
        context.fillRect(
          -particle.width / 2,
          -particle.height / 2,
          particle.width,
          particle.height,
        );
        context.restore();
      });

      if (progress < 1) {
        requestAnimationFrame(animate);
      } else {
        canvas.remove();
      }
    }

    requestAnimationFrame(animate);
    window.addEventListener("resize", resizeCanvas);
  });
</script>
