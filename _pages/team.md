---
layout: archive
title: "Meet Our Team"
permalink: /team/
author_profile: false
classes: wide #uses theme's full-width class

---
<style>
.archive .team-container {
  display: grid !important;
  grid-template-columns: 1fr !important;
  gap: 4rem !important;
  max-width: 1200px !important;
  margin: 0 auto !important;
  padding: 2rem 0 !important;
}

/* Team member grid */
.team-member {
  display: grid;
  grid-template-columns: 250px 1fr;
  gap: 3rem;
  padding: 2rem;
  background: #fff;
  border-radius: 15px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
}

/* Left column */
.team-member__photo {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 10px;
}

.team-member__social {
  margin-top: 1.5rem;
  text-align: center;
}

/* Right column */
.team-member__info {
  padding-right: 2rem;
}

/* Mobile styles */
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

/* Social links */
.team-member__social a {
  color: #333;
  font-size: 1.5rem;
  margin: 0 0.8rem;
  transition: all 0.3s ease;
}

.team-member__social a:hover {
  color: #0077b5;
  transform: translateY(-2px);
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





</div>


<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---
