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

.member-photo {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 10px;
  transition: transform 0.3s ease;
}

.team-member:hover .member-photo {
  transform: scale(1.02);
}

.member-info {
  padding-right: 2rem;
}

.role {
  color: var(--global-text-color);
  font-size: 1.1rem;
  margin: 0.8rem 0;
  font-style: italic;
}

.social-links {
  display: flex;
  gap: 1.5rem;
  margin-top: 1.5rem;
  justify-content: center;
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
  
  .member-photo {
    height: 200px;
    width: 200px;
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
           alt="Christopher Keen" 
           class="team-member__photo">
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Christopher-Keen">Christopher Keen</h3>
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
      <img src="{{ '/images/mike_profile.jpg' | relative_url }}" 
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
      <div class="team-member__social">
        <a href="#"><i class="fab fa-linkedin"></i></a>
        <a href="#"><i class="fab fa-github"></i></a>
        <a href="#"><i class="fas fa-envelope"></i></a>
      </div>
    </div>
    
    <div class="team-member__info">
      <h3 id="Catherine-Liang">Catherine Liang</h3>
      <p class="role"><em>Undergraduate Student in Biomedical Engineering</em></p>
      <div class="bio">
        <p>Catherine is an undergraduate student majoring in Biomedical Engineering with a minor in Computer Science. Her current project involves investigating the effects that different dMRI preprocessing methods have on ADC map generation (specifically for prostate scans). In her free time, she enjoys playing video games, watching anime, and drawing.</p>
      </div>
    </div>
  </div>
</div>

<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---
