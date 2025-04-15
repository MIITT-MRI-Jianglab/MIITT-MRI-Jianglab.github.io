---
layout: archive
title: "Meet Our Team"
permalink: /team/
author_profile: false
classes: wide #uses theme's full-width class

---
<style>
/* Existing styles */
.archive .team-container {
  display: grid !important;
  grid-template-columns: 1fr !important;
  gap: 4rem !important;
  max-width: 1200px !important;
  margin: 0 auto !important;
  padding: 2rem 0 !important;
}

.team-member {
  display: grid;
  grid-template-columns: 250px 1fr;
  gap: 3rem;
  padding: 2rem;
  background: #fff;
  border-radius: 15px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

/* NEW: Grid hover effect */
.team-member:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 25px rgba(0,0,0,0.15);
}

.team-member__photo {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 10px;
  transition: transform 0.3s ease;
}

/* NEW: Photo hover effect */
.team-member:hover .team-member__photo {
  transform: scale(1.02);
}

.team-member__social {
  margin-top: 1.5rem;
  text-align: center;
}

.team-member__info {
  padding-right: 2rem;
}

/* Enhanced Social Icon Hover Effects */
.team-member__social a {
  color: #333;
  font-size: 1.5rem;
  margin: 0 0.8rem;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  display: inline-block;
}

.team-member__social a:hover {
  color: #0077b5; /* LinkedIn blue */
  transform: translateY(-3px) scale(1.15);
  text-shadow: 0 2px 8px rgba(0,119,181,0.2);
}

/* Different colors for different socials */
.team-member__social a[href*="github.com"]:hover {
  color: #181717; /* GitHub black */
}

.team-member__social a[href*="twitter.com"]:hover {
  color: #1DA1F2; /* Twitter blue */
}

.team-member__social a[href^="mailto:"]:hover {
  color: #EA4335; /* Gmail red */
}

@media (max-width: 768px) {
  .team-member {
    grid-template-columns: 1fr;
    text-align: center;
  }
  
  .team-member__photo {
    height: 200px;
    width: 200px !important;
    margin: 0 auto;
  }
  
  .team-member__info {
    padding-right: 0;
  }
}
</style>

<div class="team-container">

  <!-- Team Member 1 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Jiayao Yang" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Jiayao-Yang">Jiayao Yang</h3>
      <p class="role"><em>PhD student in EECS</em></p>
      <div class="bio">
        <p>RF Pulse Design</p>
      </div>
    </div>
  </div>


   <!-- Team Member 2 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Hong Yu" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Hongze-Yu">Hongze Yu</h3>
      <p class="role"><em>PhD student in EECS</em></p>
      <div class="bio">
        <p>DL/ML</p>
      </div>
    </div>
  </div>


   <!-- Team Member 3 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Chris Keen" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Chris-Keen">Chris Keen</h3>
      <p class="role"><em>PhD student in BME</em></p>
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
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Tejinder-Kaur">Tejinder Kaur</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
      <div class="bio">
        <p>Clinical Applications</p>
      </div>
    </div>
  </div>


   <!-- Team Member 5 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Michael Jaroszewicz" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Michael-Jaroszewicz">Michael Jaroszewicz</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
      <div class="bio">
        <p>Diffusion</p>
      </div>
    </div>
  </div>

  <!-- Team Member 6 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/assets/images/team/john-doe.jpg' | relative_url }}" 
           alt="Catherine Liang" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Catherine-Liang">Catherine Liang</h3>
      <p class="role"><em>Undergraduate student in BME</em></p>
      <div class="bio">
        <p>AI</p>
      </div>
    </div>
  </div>






</div>


<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---
