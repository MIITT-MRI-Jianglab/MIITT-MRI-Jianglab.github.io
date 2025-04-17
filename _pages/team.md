---
layout: archive
title: "Meet Our Team"
permalink: /team/
author_profile: false
classes: wide #uses theme's full-width class

---
<style>
/* Team Grid Styles */
.team-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 4rem;
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem 0;
}

.team-member {
  display: grid;
  grid-template-columns: 250px 1fr;
  gap: 3rem;
  padding: 2rem;
  background: var(--global-bg-color);
  color: var(--global-text-color);
  border-radius: 15px;
  box-shadow: 0 5px 15px var(--global-border-color);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.team-member:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 25px var(--global-border-color);
}
.member-photo-container {
  width: 100px;
  height: 100px;
  border-radius: 10px;
  overflow: hidden;
  margin: 0 auto;
}

.member-photo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  aspect-ratio: 1/1;
  transition: transform 0.3s ease;
}

.team-member:hover .member-photo {
  transform: scale(1.02);
}

.member-info {
  padding-right: 2rem;
  display: flex;
  flex-direction: column;
  margin-bottom: 0rem;
}

.role {
  color: var(--global-text-color);
  font-size: 0.9rem;
  margin: 0rem 0;
  font-style: italic;
   margin-bottom: 0rem; /* Space between role and social links */
}

.social-links {
  order: 3; 
 /*display: flex;*/
  gap: 1.2rem;
  margin-top: 1rem;
  justify-content: flex-start;
}

.social-links a {
  color: var(--global-text-color);
  font-size: 1.5rem;
  transition: all 0.3s ease;
}

.social-links a:hover {
  transform: translateY(-3px);
}

/* Platform-specific hover colors */
.social-links a[href*="linkedin.com"]:hover { color: #0077b5; }
.social-links a[href*="github.com"]:hover { color: #181717; }
.social-links a[href*="twitter.com"]:hover { color: #1da1f2; }
.social-links a[href*="instagram.com"]:hover { color: #e1306c; }
.social-links a[href^="mailto:"]:hover { color: #ea4335; }

@media (max-width: 768px) {
  .team-member {
    grid-template-columns: 1fr;
    text-align: center;
    gap: 2rem;
  }
  .member-photo-container {
    width: 100px;
    height: 100px;
  }
  
  .member-photo {
    width: 100%;
    height: 100%;
    aspect-ratio: 1/1; /* Force square */
    object-fit: cover; /* Crop to fill */
    margin: 0 auto;
  }
  
  .member-info {
    padding-right: 0;
  }
  
  .social-links {
    justify-content: center;
  }
}
</style>


<div class="team-container">

  <!-- Team Member 1 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/jiayao-24-p.jpg' | relative_url }}" 
           alt="Jiayao Yang" 
           class="team-member__photo">
      
    </div>
    
    <div class="team-member__info">
      <h3 id="Jiayao-Yang">Jiayao Yang</h3>
      <p class="role"><em>PhD student in EECS</em></p>
      <div class="team-member__social">
        <!-- <a href="#"><i class="fab fa-linkedin"></i></a>*/ -->
        <a href="https://jyang000.github.io/"><i class="fab fa-globe"></i></a>
        <a href="jiayao@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in ECE, majoring in Signal & Image Processing and Machine Learning. I’m fortunate to be co-advised by Jon-Fredrik Nielsen and Yun Jiang. My current research explores new algorithms for multidimensional pulses design in magnetic resonance imaging (MRI) using optimization methods and their applications to reduced field-of-view imaging. I’m interested in developing new algorithms for MRI combining signal processing knowledge and machine learning. Outside of research, I enjoy drawing and painting.</p>
      </div>
    </div>
  </div>


   <!-- Team Member 2 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/hongze_profile_image.jpg' | relative_url }}" 
           alt="Hongze Yu" 
           class="team-member__photo">
      
    </div>
    
    <div class="team-member__info">
      <h3 id="Hongze-Yu">Hongze Yu</h3>
      <p class="role"><em>PhD student in EECS</em></p>
      <div class="team-member__social">
        <a href="[#](https://www.linkedin.com/in/hongze-yu-a2486721b/)"><i class="fab fa-linkedin"></i></a>
        <a href="https://hongzeyu0319.github.io/"><i class="fab fa-globe"></i></a>
        <a href="https://github.com/hongzeyu0319"><i class="fab fa-github"></i></a>
        <a href="hongze@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in Electrical and Computer Engineering, specializing in signal and image processing and machine learning. My current work focuses on accelerated MRI reconstruction using self‑supervised deep learning methods. I’m also interested in quantitative MRI, sampling‑trajectory optimization, and inverse problems more broadly. Outside of research, I enjoy cycling, tennis, and road trips.</p>
      </div>
    </div>
  </div>


   <!-- Team Member 3 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Christopher Keen" 
           class="team-member__photo">
     
    </div>
    
    <div class="team-member__info">
      <h3 id="Christopher-Keen">Christopher Keen</h3>
      <p class="role"><em>PhD student in BME</em></p>
       <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>MRF</p>
      </div>
    </div>
  </div>


   <!-- Team Member 4 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Tejinder Kaur" 
           class="team-member__photo">
     
    </div>
    
    <div class="team-member__info">
      <h3 id="Tejinder-Kaur">Tejinder Kaur</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
       <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>Clinical Applications</p>
      </div>
    </div>
  </div>


   <!-- Team Member 5 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/mike_profile.jpg' | relative_url }}" 
           alt="Michael Jaroszewicz" 
           class="team-member__photo">
     
    </div>
    
    <div class="team-member__info">
      <h3 id="Michael-Jaroszewicz">Michael Jaroszewicz</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
      <div class="team-member__social">
        <!-- <a href="#"><i class="fab fa-linkedin"></i></a> -->
       <!-- <a href="#"><i class="fab fa-github"></i></a> -->
        <a href="jaroszem@med.umich.edu"><i class="fas fa-envelope"></i></a>
         
      </div>
      <div class="bio">
        <p>I'm an NMR spectroscopist by training, with a background in developing pulse sequences to address sensitivity and resolution challenges in solid- and solution-state NMR. My current work focuses on applying similar principles to quantitative MRI, particularly in developing techniques for diffusion and T2 mapping to better study disease. This includes designing specialized RF pulse sequences and creating strategies for robust and efficient data acquisition. Outside of research, I am passionate about cooking and especially enjoy preparing dishes from various cuisines I've encountered while traveling and studying abroad.</p>
      </div>
    </div>
  </div>

  <!-- Team Member 6 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/profile_Catherine.jpg' | relative_url }}" 
           alt="Catherine Liang" 
           class="team-member__photo">
      
    </div>
    
    <div class="team-member__info">
      <h3 id="Catherine-Liang">Catherine Liang</h3>
      <p class="role"><em>Undergraduate Student in Biomedical Engineering</em></p>
      <div class="team-member__social">
       <a href="www.linkedin.com/in/catherine-liang-95406b208"><i class="fab fa-linkedin"></i></a>
       <!-- <a href="#"><i class="fab fa-github"></i></a> -->
        <a href="catliang@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>Catherine is an undergraduate student majoring in Biomedical Engineering with a minor in Computer Science. Her current project involves investigating the effects that different dMRI preprocessing methods have on ADC map generation (specifically for prostate scans). In her free time, she enjoys playing video games, watching anime, and drawing.</p>
      </div>
    </div>
  </div>
</div>

<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---
