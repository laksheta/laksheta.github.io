---
permalink: /
title: "About Me"
author_profile: true
classes: wide
redirect_from: 
  - /about/
  - /about.html
---

I’m a Master of Engineering student specializing in Power Electronics and Control Systems. I’ve gained extensive experience in Solid-State Transformer (SST) modeling, particularly with Modular Multilevel Converters (MMC) and Dual Active Bridge (DAB) converters. In addition, I’ve explored Hardware-in-the-Loop (HIL) simulations and conducted hardware testing. Currently, my research focuses on developing fault-tolerant control strategies for DAB converters and building SST models using Typhoon HIL.

<style>
  /* 1. Force the page content to occupy the full width of the container */
  .page {
    padding-right: 0 !important;
  }
  
  .page__content {
    width: 100% !important;
    max-width: 100% !important;
  }

  /* 2. Photo Dump Styling */
  .work-dump {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 30px;
  }
  
  .work-dump img {
    /* Changed to 25% (4 images per row) since the page is now wider */
    width: calc(25% - 10px); 
    height: 200px;
    object-fit: cover;
    border-radius: 4px;
    background-color: #f0f0f0;
  }

  /* Mobile adjustment */
  @media (max-width: 800px) {
    .work-dump img {
      width: calc(50% - 10px); /* 2 per row on mobile */
    }
  }
</style>

<div class="work-dump">
  <img src="/images/about/1.JPG" alt="">
  <img src="/images/about/2.jpg" alt="">
  <img src="/images/about/3.jpg" alt="">
  <img src="/images/about/4.jpg" alt="">
  <img src="/images/about/5.jpg" alt="">
  <img src="/images/about/6.jpg" alt="">
  <img src="/images/about/7.jpg" alt="">
  <img src="/images/about/8.jpg" alt="">
</div>