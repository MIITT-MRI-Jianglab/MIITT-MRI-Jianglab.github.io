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
  .team-member__photo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 8px; /* Match container radius */
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
 display: flex;
  gap: 1.2rem;
  margin-top: 1rem;
  justify-content: flex-start;
    transition: all 0.3s ease; /* Add transition */

}

.social-links a {
  color: var(--global-text-color);
  font-size: 1.5rem;
  transition: all 0.3s ease;
}

.social-links a:hover {
  transform: translateY(-3px);
    opacity: 0.9; /* Added for better visual feedback */

}

/* Platform-specific hover colors */
.social-links a[href*="linkedin.com"]:hover { color: #0077b5 !important; }
.social-links a[href*="github.com"]:hover { color: #181717 !important; }
.social-links a[href*="mailto:"]:hover { color: #ea4335 !important; }
.social-links a:hover .fa-globe { 
  color: #34e68a !important; /* Brighter green on hover */
  transform: scale(1.1); 
}

  /* Alumni Section */
.alumni-section {
  margin: 4rem 0;
  padding-top: 3rem;
  border-top: 2px solid var(--global-border-color);
}

.alumni-heading {
  text-align: center;
  margin-bottom: 2rem;
  color: var(--global-text-color);
}

.alumni-list {
  display: grid;
  gap: 1.5rem;
  max-width: 1200px;
  margin: 0 auto;
}

.alumni-member {
  padding: 1.2rem;
  background: var(--global-bg-color);
  border-radius: 8px;
  box-shadow: 0 2px 8px var(--global-border-color);
}

.alumni-name {
  margin: 0;
  font-size: 1.1rem;
  color: var(--global-text-color);
}

.alumni-details {
  color: #666;
  font-size: 0.9rem;
  margin: 0.5rem 0 0;
}

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

  .alumni-list {
    grid-template-columns: 1fr;
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
        <!-- <a href="https://jyang000.github.io/"><i class="fab fa-link"></i></a> -->
        <a href="https://jyang000.github.io/"><i class="fas fa-fw fa-link " aria-hidden="true"></i></a>
        <a href="mailto:jiayao@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in ECE, majoring in Signal & Image Processing and Machine Learning. I’m fortunate to be co-advised by Jon-Fredrik Nielsen and Yun Jiang. My current research explores new algorithms for multidimensional pulses design in magnetic resonance imaging (MRI) using optimization methods and their applications to reduced field-of-view imaging. I’m interested in developing new algorithms for MRI combining signal processing knowledge and machine learning. Outside of research, I enjoy drawing and painting.</p>
      </div>
    </div>
  </div>


   <!-- Team Member 2 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{'/images/hongze_profile_image.png' | relative_url }}" 
           alt="Hongze Yu" 
           class="team-member__photo">
      
    </div>
    
    <div class="team-member__info">
      <h3 id="Hongze-Yu">Hongze Yu</h3>
      <p class="role"><em>PhD student in EECS</em></p>
      <div class="team-member__social">
        <a href="https://www.linkedin.com/in/hongze-yu-a2486721b/"><i class="fab fa-linkedin"></i></a>
    <!--    <a href="https://hongzeyu0319.github.io/"><i class="fab fa-globe"></i></a>-->
       <a href="https://hongzeyu0319.github.io/"><i class="fas fa-fw fa-link " aria-hidden="true"></i></a>
        <a href="https://github.com/hongzeyu0319"><i class="fab fa-github"></i></a>
        <a href="mailto:hongze@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in Electrical and Computer Engineering, specializing in signal and image processing and machine learning. My current work focuses on accelerated MRI reconstruction using self‑supervised deep learning methods. I’m also interested in quantitative MRI, sampling‑trajectory optimization, and inverse problems more broadly. Outside of research, I enjoy cycling, tennis, and road trips.</p>
      </div>
    </div>
  </div>


   <!-- Team Member 3 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/chris_profile.jpg' | relative_url }}" 
           alt="Christopher Keen" 
           class="team-member__photo">
     
    </div>
    
    <div class="team-member__info">
      <h3 id="Christopher-Keen">Christopher Keen</h3>
      <p class="role"><em>PhD student in BME</em></p>
       <div class="team-member__social">
       <!-- <a href="#"><i class="fab fa-linkedin"></i></a> -->
       <!-- <a href="#"><i class="fab fa-github"></i></a> -->
        <a href="mailto:cekeen@med.umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>I’m a PhD student in Biomedical engineering, specializing in magnetic resonance fingerprinting (MRF). My work is focussed on improving the accuracy and quality MRF T1 and T2 maps and applying this technology to the diagnosis and management of abdominal and pelvic cancers. This includes MRF pulse sequence optimization and application in the prostate at 0.55T to improve MRI-guided biopsy procedures. When I’m not in the lab, I enjoy escaping the city to go camping, hiking, and skiing in the mountains.</p>
      </div>
    </div>
  </div>


   <!-- Team Member 4 -->
  <div class="team-member">
    <div class="team-member__left">
      <img src="{{ '/images/Headshot_Tejinder.jpg' | relative_url }}" 
           alt="Tejinder Kaur" 
           class="team-member__photo">
     
    </div>
    
    <div class="team-member__info">
      <h3 id="Tejinder-Kaur">Tejinder Kaur</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
       <div class="team-member__social">
        <!-- <a href="#"><i class="fab fa-linkedin"></i></a> -->
        <!-- <a href="#"><i class="fab fa-github"></i></a> -->
        <a href="https://www.researchgate.net/profile/Tejinder-Kaur-28"><i class="fas fa-fw fa-link " aria-hidden="true"></i></a>
        <a href="mailto:kaurte@med.umich.edu"><i class="fas fa-envelope"></i></a> 
      </div>
      <div class="bio">
        <p>I’m an MD in Radiodiagnosis and currently working as a postdoctoral clinical research fellow. My work focuses on MRI-guided interventions at mid-field and the use of MRI fingerprinting in prostate imaging. I’m particularly interested in advancing techniques in prostate imaging to improve diagnostic accuracy. Outside of work, I enjoy reading and playing table tennis.</p>
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
        <a href="mailto:jaroszem@med.umich.edu"><i class="fas fa-envelope"></i></a>
         
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
       <a href="https://www.linkedin.com/in/catherine-liang-95406b208"><i class="fab fa-linkedin"></i></a>
       <!-- <a href="#"><i class="fab fa-github"></i></a> -->
        <a href="mailto:catliang@umich.edu"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="bio">
        <p>Catherine is an undergraduate student majoring in Biomedical Engineering with a minor in Computer Science. Her current project involves investigating the effects that different dMRI preprocessing methods have on ADC map generation (specifically for prostate scans). In her free time, she enjoys playing video games, watching anime, and drawing.</p>
      </div>
    </div>
  </div>


  <div class="alumni-section">
  <h2 class="alumni-heading">Lab Alumni</h2>
  <div class="alumni-list">
    
    <div class="alumni-member">
      <div class="alumni-name">John Smith</div>
      <div class="alumni-details">
        <div>PhD Student (2018-2022)</div>
        <div>Now: Research Scientist at XYZ Corp</div>
      </div>
    </div>

    <div class="alumni-member">
      <div class="alumni-name">Jane Doe</div>
      <div class="alumni-details">
        <div>Postdoc (2019-2021)</div>
        <div>Now: Assistant Professor at ABC University</div>
        <!-- <div class="social-links" style="margin-top: 0.8rem;"> -->
        <!--  <a href="#"><i class="fab fa-linkedin"></i></a> -->
        <!--  <a href="#"><i class="fas fa-envelope"></i></a> -->
        </div>
      </div>
    </div>

  </div>
</div>
</div>

<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---
