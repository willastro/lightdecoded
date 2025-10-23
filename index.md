  if (!sessionStorage.getItem("visited")) {
    sessionStorage.setItem("visited", "true");
    window.location.href = "splash.html";
  }
</script>
<link rel="stylesheet" href="/lightdecoded/assets/css/style.css">
<nav style="text-align:center; margin-bottom:2rem;">
  <a href="/lightdecoded/index.html" style="margin:0 1rem;">Home</a>
  <a href="about/" style="margin:0 1rem;">About</a>
  
  <!-- Dropdown container -->
  <div class="dropdown">
    <button class="dropbtn">Projects ▾</button>
    <div class="dropdown-content">
      <a href="projects/spec_analysis/">Spectral Analysis</a>
      <a href="projects/lida_db/">Leiden Ice Database for Astrochemistry</a>
      <a href="projects/mri/">Medical Imaging Data Science</a>
    </div>
  </div>
</nav>


# 👋 Hi, I'm Dr. Will Rocha. Welcome to Light Decoded!  
**Spectral & Imaging Data Scientist**

<div class="mri-gallery">
  <img src="https://willastro.github.io/lightdecoded/assets/images/Perfil_linkedin.jpg" alt="Profile">
</div>

<style>
.mri-gallery {
  display: flex;
  justify-content: center;
  gap: 0.8rem;
  flex-wrap: wrap;
  margin: 1rem auto 1rem;
}
.mri-gallery img {
  width: 20%;
  max-width: 160px;
  border-radius: 10px;
  box-shadow: 0 0 12px rgba(255,255,255,0.12);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.mri-gallery img:hover {
  transform: scale(1.05);
  box-shadow: 0 0 20px rgba(255,255,255,0.25);
}
</style>

I specialize in extracting insights from complex spectra and imaging data — from astronomy to medical imaging.  
My work focuses on **spectral fitting, image analysis, and AI-based data pipelines** that transform raw measurements into actionable results.

---

## 🧠 Expertise
- Spectral analysis and modeling (MCMC, Bayesian fitting, ENIIGMA)
- Image processing and computer vision (OpenCV, scikit-image, deep learning)
- Machine learning for feature extraction and classification
- Reproducible pipelines (Python, NumPy, SciPy, Astropy)
- Data visualization (Matplotlib, Bokeh)

---

## 🔬 Featured Projects
### [ENIIGMA: AI-Based Spectral Fitting Tool](https://willastro.github.io/lightdecoded/projects/spec_analysis/)
Intelligent pipeline for spectral fitting using AI.

### [Leiden Ice Database for Astrochemistry](https://willastro.github.io/lightdecoded/projects/lida_db/)
Relational database built with Python-Flask and SQL.

### [Medical Imaging Data Science](https://willastro.github.io/lightdecoded/projects/mri/)
Robust pipeline for cancer detection using computer vision.

---

## 📬 Contact
📧 [willrobsonastro@gmail.com](mailto:willrobsonastro@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/will-rocha-275b6374/)  
💻 [GitHub](https://github.com/willastro)


<!-- INSTITUTIONS SECTION -->
<section class="institutions-section">
  <h2>Institutions I Have Worked With</h2>
  <div class="institutions-logos">
    <img src="https://www.universiteitleiden.nl/binaries/content/assets/algemeen/dossiers/450-jaar/beeldscherm/beeldscherm-logoul-450diap.png" alt="Leiden University">
    <img src="https://www.citypng.com/public/uploads/preview/nasa-white-logo-free-png-701751694712949kl9wa1xf80.png" alt="NASA">
    <img src="https://esahubble.org/media/archives/logos/medium/esa_screen_white.jpg" alt="ESA">
    <img src="https://brand.airbus.com/sites/g/files/jlcbta121/files/styles/w900/public/2021-06/logo_white.webp?itok=qH71b_6l" alt="Airbus">
  </div>
</section>

<style>
.institutions-section {
  background: radial-gradient(circle at 50% 50%, #0a0a0a, #000);
  padding: 3rem 1rem;
  text-align: center;
  border-top: 1px solid rgba(255,255,255,0.1);
  border-bottom: 1px solid rgba(255,255,255,0.1);
  box-shadow: 0 0 40px rgba(255,255,255,0.05) inset;
}

.institutions-section h2 {
  color: #fff;
  font-weight: 500;
  font-size: 1.6rem;
  margin-bottom: 2rem;
  letter-spacing: 0.03em;
  text-shadow: 0 0 10px rgba(255,255,255,0.25);
}

.institutions-logos {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  align-items: center;
  gap: 2rem;
}

.institutions-logos img {
  height: 60px;
  max-width: 140px;
  object-fit: contain;
  opacity: 0.85;
  filter: drop-shadow(0 0 6px rgba(255,255,255,0.15));
  transition: transform 0.3s ease, opacity 0.3s ease, filter 0.3s ease;
}

.institutions-logos img:hover {
  transform: scale(1.1);
  opacity: 1;
  filter: drop-shadow(0 0 12px rgba(255,255,255,0.4));
}
</style>



