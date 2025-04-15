---
layout: archive
title: "Meet Our Team"
permalink: /team/
author_profile: true

---
# Meet Our Team

Our talented team driving innovation forward.

<div class="team-container">

<div class="team-member">
  <img src="https://i.pravatar.cc/300?img=1" alt="John Doe" class="member-photo">
  <div class="member-info">
    <h3>John Doe</h3>
    <p class="role">CEO & Founder</p>
    <p class="bio">Tech visionary with 15+ years experience building disruptive solutions</p>
    <div class="social-links">
      <a href="#"><i class="fab fa-linkedin"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
      <a href="#"><i class="fas fa-envelope"></i></a>
    </div>
  </div>
</div>

<div class="team-member">
  <img src="https://i.pravatar.cc/300?img=2" alt="Jane Smith" class="member-photo">
  <div class="member-info">
    <h3>Jane Smith</h3>
    <p class="role">CTO</p>
    <p class="bio">Full-stack architect passionate about scalable systems</p>
    <div class="social-links">
      <a href="#"><i class="fab fa-github"></i></a>
      <a href="#"><i class="fab fa-dev"></i></a>
    </div>
  </div>
</div>

<div class="team-member">
  <img src="https://i.pravatar.cc/300?img=3" alt="Mike Johnson" class="member-photo">
  <div class="member-info">
    <h3>Mike Johnson</h3>
    <p class="role">Marketing Director</p>
    <p class="bio">Growth hacker with expertise in viral campaigns</p>
    <div class="social-links">
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-tiktok"></i></a>
    </div>
  </div>
</div>

</div>

<style>
.team-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  padding: 2rem 0;
}

.team-member {
  background: #ffffff;
  border-radius: 15px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  overflow: hidden;
}

.team-member:hover {
  transform: translateY(-5px);
}

.member-photo {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-bottom: 3px solid #f0f0f0;
}

.member-info {
  padding: 1.5rem;
  text-align: center;
}

.role {
  color: #666;
  font-weight: 500;
  margin: 0.5rem 0;
}

.bio {
  color: #444;
  font-size: 0.95rem;
  line-height: 1.5;
  margin: 1rem 0;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 1rem;
  padding: 1rem 0;
}

.social-links a {
  color: #333;
  font-size: 1.2rem;
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: #0077b5; /* LinkedIn blue */
}
</style>

<!-- Add Font Awesome for icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
---

### Jiayao Yang 
![Jiayao](https://i.pravatar.cc/150?img=1)  
**Role:** PhD student of EECS
**Intro:** Visionary leader  
**Connect:** [LinkedIn](#) | [Twitter](#) | [Email](#)

---

### Hongze Yu  
![Hongze](https://i.pravatar.cc/150?img=2)  
**PhD student of EECS**
**Intro:** Full-stack developer 
**Connect:** [GitHub](#) | [Medium](#)

---

### Chris Keen  
![Mike Johnson - Marketing](https://i.pravatar.cc/150?img=3)  
**PhD student of BME** 
**Intro:** Digital 
**Connect:** [Instagram](#) | [Facebook](#)

---

### 🖼️ How to Add Your Photos:
1. Replace image URLs (`https://i.pravatar.cc/...`) with actual image paths:
   ```markdown
   ![Alt Text](/path/to/your-image.jpg)
   ```
2. For better formatting, use square images (1:1 aspect ratio).

### 🌐 Image Hosting Options:
- Upload to your website's `/images/team/` folder
- Use free image hosting: [Imgur](https://imgur.com), [Cloudinary](https://cloudinary.com)
- Use placeholders: `https://i.pravatar.cc/150?img=[1-70]`

### 💡 Pro Tip: 
While this is pure Markdown, to create columns/grids you'll need to either:
1. Use a Markdown table (limited customization)
2. Add CSS later using your website builder/static site generator
{% include base_path %}
