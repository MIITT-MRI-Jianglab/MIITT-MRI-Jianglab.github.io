---
layout: archive
title: "Meet Our Team"
permalink: /team/
author_profile: false
classes: wide
---

<style>
/* ===== THEME VARIABLES ===== */
/*:root {
  --global-bg-color: #ffffff;
  --global-text-color: #333333;
  --global-border-color: rgba(0, 0, 0, 0.08);
}

@media (prefers-color-scheme: dark) {
  :root {
    --global-bg-color: #1a1a1a;
    --global-text-color: #e0e0e0;
    --global-border-color: rgba(255, 255, 255, 0.08);
  }
}
*/
/* ===== TEAM GRID ===== */
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

.team-member__photo-container {
  width: 250px;
  height: 250px;
  border-radius: 8px;
  overflow: hidden;
  margin: 0 auto;
}

.team-member__photo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.team-member:hover .team-member__photo {
  transform: scale(1.02);
}

.team-member__info h3 {
  font-size: 1.25rem;
  margin: 0; /* Changed from margin-bottom: 0.2rem */
  padding-top: 0.2rem; /* Optional: Fine-tune if needed */
}

.role {
  color: var(--global-text-color);
  font-size: 0.85rem;
  margin: 0.2rem 0;
  font-style: italic;
}

.social-links {
  display: flex;
  gap: 0.8rem;
  margin-top: 0.3rem;
}

.social-links a {
  color: var(--global-text-color);
  font-size: 0.85rem;
  transition: all 0.3s ease;
}

.social-links a:hover {
  transform: translateY(-3px);
  opacity: 0.9;
}

.bio p {
  font-size: 0.9rem;
  line-height: 1.5;
  margin-top: 0.6rem;
}

.social-links a[href*="linkedin.com"]:hover { color: #0077b5 !important; }
.social-links a[href*="github.com"]:hover { color: #181717 !important; }
.social-links a[href*="mailto:"]:hover { color: #ea4335 !important; }
.social-links a[href*="://"]:hover .fa-link { color: #34e68a !important; }

.alumni-section {
  margin-top: 6rem;
  padding-top: 4rem;
  border-top: 2px solid var(--global-border-color);
}

.alumni-member {
  display: flex;
  flex-wrap: wrap;
  gap: 0.2rem 1.5rem;
  padding: 1rem;
  margin: 0.5rem 0;
}

.alumni-name-role {
  display: flex;
  gap: 1rem;
  align-items: baseline;
}

.alumni-name {
  font-weight: 600;
  color: var(--global-text-color);
  font-size: 1rem;
}

.alumni-role {
  color: var(--global-text-color);
  font-size: 0.9rem;
}

.alumni-bio {
  width: 100%;
  margin-top: 0;
  padding-top: 0;
  color: var(--global-text-color);
  border-top: none;
  line-height: 1.3;
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .team-member {
    grid-template-columns: 1fr;
    text-align: center;
    gap: 2rem;
  }

  .team-member__photo-container {
    width: 200px;
    height: 200px;
    max-width: 100%;
    height: auto;
    aspect-ratio: 1;
  }

  .team-member__info h3 {
    font-size: 1.2rem;
    margin: 0; 
  }

  .role {
    font-size: 0.8rem;
    margin: 0.1rem 0;
  }

  .social-links {
    gap: 0.6rem;
    justify-content: center;
  }

  .alumni-member {
    flex-direction: column;
    gap: 0.1rem;
  }
}
</style>

<div class="team-container">

  <!-- Jiayao Yang -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/jiayao-24-p.jpg' | relative_url }}" 
           alt="Jiayao Yang - PhD student in EECS" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Jiayao-Yang">Jiayao Yang</h3>
      <p class="role"><em>PhD Student in Electrial and Computer Engineering</em></p>
      <div class="social-links">
        <a href="https://jyang000.github.io/" aria-label="Personal website">
          <i class="fas fa-link"></i>
        </a>
        <a href="mailto:jiayao@umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in ECE, majoring in Signal & Image Processing and Machine Learning. I’m fortunate to be co-advised by Jon-Fredrik Nielsen and Yun Jiang. My current research explores new algorithms for multidimensional pulses design in magnetic resonance imaging (MRI) using optimization methods and their applications to reduced field-of-view imaging. I’m interested in developing new algorithms for MRI combining signal processing knowledge and machine learning. Outside of research, I enjoy drawing and painting.</p>
      </div>
    </div>
  </div>

  <!-- Hongze Yu -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/hongze_profile_image.png' | relative_url }}" 
           alt="Hongze Yu - PhD student in EECS" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Hongze-Yu">Hongze Yu</h3>
      <p class="role"><em>PhD Student in Electrial and Computer Engineering</em></p>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/hongze-yu-a2486721b/" aria-label="LinkedIn">
          <i class="fab fa-linkedin"></i>
        </a>
        <a href="https://hongzeyu0319.github.io/" aria-label="Personal website">
          <i class="fas fa-link"></i>
        </a>
        <a href="https://github.com/hongzeyu0319" aria-label="GitHub">
          <i class="fab fa-github"></i>
        </a>
        <a href="mailto:hongze@umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>I’m a PhD candidate in Electrical and Computer Engineering, specializing in signal and image processing and machine learning. My current work focuses on accelerated MRI reconstruction using self‑supervised deep learning methods. I’m also interested in quantitative MRI, sampling‑trajectory optimization, and inverse problems more broadly. Outside of research, I enjoy cycling, tennis, and road trips.</p>
      </div>
    </div>
  </div>

  <!-- Christopher Keen -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/chris_profile.jpg' | relative_url }}" 
           alt="Christopher Keen - PhD student in Biomedical Engineering" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Christopher-Keen">Christopher Keen</h3>
      <p class="role"><em>PhD Student in Biomedical Engineering</em></p>
      <div class="social-links">
        <a href="mailto:cekeen@med.umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>I’m a PhD student in Biomedical engineering, specializing in magnetic resonance fingerprinting (MRF). My work is focussed on improving the accuracy and quality MRF T1 and T2 maps and applying this technology to the diagnosis and management of abdominal and pelvic cancers. This includes MRF pulse sequence optimization and application in the prostate at 0.55T to improve MRI-guided biopsy procedures. When I’m not in the lab, I enjoy escaping the city to go camping, hiking, and skiing in the mountains.</p>
      </div>
    </div>
  </div>

  <!-- Tejinder Kaur -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/Headshot_Tejinder.jpg' | relative_url }}" 
           alt="Tejinder Kaur - Postdoctoral Research Fellow" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Tejinder-Kaur">Tejinder Kaur</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
      <div class="social-links">
        <a href="https://www.researchgate.net/profile/Tejinder-Kaur-28" aria-label="ResearchGate">
          <i class="fas fa-link"></i>
        </a>
        <a href="mailto:kaurte@med.umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>I’m an MD in Radiodiagnosis and currently working as a postdoctoral clinical research fellow. My work focuses on MRI-guided interventions at mid-field and the use of MRI fingerprinting in prostate imaging. I’m particularly interested in advancing techniques in prostate imaging to improve diagnostic accuracy. Outside of work, I enjoy reading and playing table tennis.</p>
      </div>
    </div>
  </div>

  <!-- Michael Jaroszewicz -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/mike_profile.jpg' | relative_url }}" 
           alt="Michael Jaroszewicz - Postdoctoral Research Fellow" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Michael-Jaroszewicz">Michael Jaroszewicz</h3>
      <p class="role"><em>Postdoctoral Research Fellow</em></p>
      <div class="social-links">
        <a href="mailto:jaroszem@med.umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>I'm an NMR spectroscopist by training, with a background in developing pulse sequences to address sensitivity and resolution challenges in solid- and solution-state NMR. My current work focuses on applying similar principles to quantitative MRI, particularly in developing techniques for diffusion and T2 mapping to better study disease. This includes designing specialized RF pulse sequences and creating strategies for robust and efficient data acquisition. Outside of research, I am passionate about cooking and especially enjoy preparing dishes from various cuisines I've encountered while traveling and studying abroad.</p>
      </div>
    </div>
  </div>

  <!-- Catherine Liang -->
  <div class="team-member">
    <div class="team-member__photo-container">
      <img src="{{ '/images/profile_Catherine.jpg' | relative_url }}" 
           alt="Catherine Liang - Undergraduate Student" 
           class="team-member__photo">
    </div>
    <div class="team-member__info">
      <h3 id="Catherine-Liang">Catherine Liang</h3>
      <p class="role"><em>Undergraduate Student in Biomedical Engineering</em></p>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/catherine-liang-95406b208" aria-label="LinkedIn">
          <i class="fab fa-linkedin"></i>
        </a>
        <a href="mailto:catliang@umich.edu" aria-label="Email">
          <i class="fas fa-envelope"></i>
        </a>
      </div>
      <div class="bio">
        <p>Catherine is an undergraduate student majoring in Biomedical Engineering with a minor in Computer Science. Her current project involves investigating the effects that different dMRI preprocessing methods have on ADC map generation (specifically for prostate scans). In her free time, she enjoys playing video games, watching anime, and drawing.</p>
      </div>
    </div>
  </div>

  <!-- Alumni Section -->
  <div class="alumni-section">
    <h2>Lab Alumni</h2>
    
    <div class="alumni-member">
      <div class="alumni-name-role">
        <div class="alumni-name">Jesus Fajardo</div>
        <div class="alumni-role">Postdoctoral Research Fellow (2022-2024)</div>
      </div>
      <div class="alumni-bio">Now Research Scientist at Wayne State University</div>
    </div>

    <div class="alumni-member">
      <div class="alumni-name-role">
        <div class="alumni-name">Jack Andrews</div>
        <div class="alumni-role">Master's Student in BME (2022-2023)</div>
      </div>
      <div class="alumni-bio">Now Software Engineer at Delphinus Medical Technologies</div>
    </div>

    <div class="alumni-member">
      <div class="alumni-name-role">
        <div class="alumni-name">Matthew Zhu</div>
        <div class="alumni-role">Master's Student in EECS (2020-2022)</div>
      </div>
      <div class="alumni-bio">Now Research Scientist at Western Digital</div>
    </div>
  </div>
</div>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
