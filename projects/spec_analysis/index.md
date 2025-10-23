---

# Spectral Analysis: Unveiling the Secrets of Space Ice

Spectral analysis is a cornerstone of astrophysical research, enabling the identification and characterization of molecular compositions in the interstellar medium. Through the study of infrared spectra, we can infer the chemical makeup, physical conditions, and evolutionary stages of cosmic environments.

## Research Highlights

### 1. Fitting Infrared Ice Spectra with Genetic Modelling Algorithms

In this 2021 study, I developed and introduced the **ENIIGMA** (Evolutionary Non-linear Infrared Ice Modelling Algorithm), a genetic algorithm-based tool designed to fit complex infrared spectra of interstellar ices. By applying ENIIGMA to the Elias 29 molecular cloud, we successfully modeled the ice composition of this source, thus highlighting the potential of the software.

[Read the full paper](https://www.aanda.org/articles/aa/full_html/2021/10/aa39360-20/aa39360-20.html)

### 2. First Detecting Icy Complex Organic Molecules and Ions in the Milky Way

Building upon our previous work, this 2024 study focused on the detection of complex organic molecules (COMs) and ions in the ices of low- and high-mass protostars. Utilizing data from the **James Webb Space Telescope (JWST)**, we identified a diverse array of COMs in the ices of NGC 1333 IRAS 2A and IRAS 23385+6053, offering new insights into the chemical complexity of star-forming regions.

[Read the full paper](https://www.aanda.org/articles/aa/full_html/2024/03/aa48427-23/aa48427-23.html)


### 3. First Detecting Icy Complex Organic Molecules and Ions in another galaxy (Large Magellanic Cloud)

On an extension of the 2024 work, we detected COMs and ions outside the Milky Way, in the Large Magellanic Cloud. Here, we utilised hyperspectral data cubes from the **James Webb Space Telescope (JWST)**. 

[Read the full paper](https://iopscience.iop.org/article/10.3847/2041-8213/ae0ccd)

## Methodology

- **ENIIGMA Tool**: A genetic algorithm-based fitting tool developed to model complex infrared spectra of interstellar ices.
- **JWST Observations**: Utilized high-resolution infrared spectra from JWST to detect and analyze COMs and ions in protostellar ices.
- **Spectral Analysis Techniques**: Employed advanced spectral fitting and analysis methods to extract chemical compositions and physical conditions from the observed spectra.

## Visualizations

The below visualization showcases the power of spectral analysis in identifying molecular features within infrared spectra using **ENIIGMA**. Tools like **ENIIGMA** facilitate the interpretation of complex spectral data sets.

<!-- LIGHT DECODED IMAGE CAROUSEL -->
<div class="carousel-container">
  <div class="carousel-image-wrapper">
    <img id="carousel" src="https://www.aanda.org/articles/aa/full_html/2021/10/aa39360-20/aa39360-20-fig17.jpg" alt="Spectral Analysis Visualization">
  </div>

  <div class="carousel-caption">Spectral Analysis - Elias 29</div>

  <div class="carousel-controls">
    <button onclick="prev()" aria-label="Previous image">◀</button>
    <button onclick="next()" aria-label="Next image">▶</button>
  </div>
</div>

<style>
.carousel-container {
  position: relative;
  width: 82%;
  max-width: 780px;
  margin: 3rem auto; /* more top space */
  padding: 2rem 0 2.5rem; /* more breathing room top/bottom */
  border-radius: 1rem;
  overflow: hidden;
  box-shadow: 0 0 30px rgba(255,255,255,0.15);
  background: radial-gradient(circle at 40% 60%, #0c0c0c, #000);
}

.carousel-image-wrapper {
  width: 100%;
  height: 500px; /* larger figures */
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  padding-top: 0.8rem; /* subtle top breathing space inside wrapper */
}

.carousel-image-wrapper img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
  transition: opacity 1s ease-in-out;
  border-radius: 0.6rem;
}

.carousel-caption {
  text-align: center;
  font-size: 1.05rem;
  margin-top: 1rem;
  color: #ddd;
  text-shadow: 0 0 10px rgba(255,255,255,0.3);
  min-height: 1.3rem;
}

.carousel-controls {
  text-align: center;
  margin-top: 1.3rem;
}

.carousel-controls button {
  background: rgba(255,255,255,0.12);
  border: 1px solid rgba(255,255,255,0.3);
  color: #fff;
  border-radius: 50%;
  padding: 0.7rem 1rem;
  margin: 0 0.7rem;
  font-size: 1.25rem;
  cursor: pointer;
  backdrop-filter: blur(6px);
  transition: all 0.3s ease;
}

.carousel-controls button:hover {
  background: rgba(255,255,255,0.25);
}
</style>

<script>
const images = [
  {
    src: "https://www.aanda.org/articles/aa/full_html/2021/10/aa39360-20/aa39360-20-fig17.jpg",
    caption: "Spectral Analysis - Elias 29"
  },
  {
    src: "https://www.aanda.org/articles/aa/full_html/2024/03/aa48427-23/aa48427-23-fig6.jpg",
    caption: "Spectral Analysis - IRAS2A and IRAS23385"
  },
  {
    src: "https://www.aanda.org/articles/aa/full_html/2025/01/aa51505-24/aa51505-24-fig10.jpg",
    caption: "Spectral Analysis - Ced 110 IRS4A"
  },
  {
    src: "https://content.cld.iop.org/journals/2041-8205/992/2/L30/revision2/apjlae0ccdf3_lr.jpg",
    caption: "Spectral Analysis - ST6"
  },
  {
    src: "https://media.springernature.com/m312/springer-static/image/art%3A10.1038%2Fs41586-025-09163-z/MediaObjects/41586_2025_9163_Fig3_HTML.png?",
    caption: "Spectral Analysis - HOPS-315"
  }
];

let i = 0;
function showImage() {
  const img = document.getElementById("carousel");
  const caption = document.querySelector(".carousel-caption");
  img.style.opacity = 0;
  setTimeout(() => {
    img.src = images[i].src;
    caption.textContent = images[i].caption;
    img.style.opacity = 1;
  }, 400);
}
function next() { i = (i + 1) % images.length; showImage(); }
function prev() { i = (i - 1 + images.length) % images.length; showImage(); }
setInterval(next, 5000); // auto-slide every 5 seconds
</script>


## Key Takeaways

- **Chemical Complexity**: The detection of COMs in protostellar ices suggests a rich chemical environment conducive to the formation of prebiotic molecules.
- **Technological Advancements**: The application of genetic algorithms and JWST data represents a significant leap in our ability to analyze and interpret complex astronomical data.
- **Future Directions**: Ongoing research aims to expand the catalog of detected COMs and ions, enhancing our understanding of the chemical evolution of the universe.

