---


# Spectral Analysis: Leiden Ice Database for Astrochemistry (LIDA)

The **Leiden Ice Database for Astrochemistry (LIDA)** is an open-access platform developed by astrophysicists at the Leiden Observatory. It provides a comprehensive collection of infrared spectra of astrophysical ice analogs, facilitating the interpretation of astronomical observations and supporting the analysis of data from missions like the James Webb Space Telescope (JWST).

## Key Features

- **Extensive Spectral Library**: LIDA hosts over 1,100 infrared spectra of solid-phase molecules in pure form or mixed in astrophysically relevant ice matrices, recorded at temperatures between 10 and ~100 K.

- **Advanced Visualization Tools**: The database integrates a 3D molecule viewer using the JSmol package, allowing users to interactively explore molecular structures and vibrational modes.

- **User-Friendly Interface**: Built using Flask and Bokeh, LIDA offers an intuitive web interface for searching, downloading, and visualizing spectral data.

## Significance

LIDA plays a crucial role in astrochemistry by providing essential data for understanding the chemical composition of interstellar ices. This information is vital for interpreting infrared observations of star-forming regions and contributes to our knowledge of the molecular building blocks of life in the universe.

For more information and to access the database, visit [Leiden Ice Database](https://icedb.strw.leidenuniv.nl).

## Visualizations

The figures below show some examples of data available in LIDA, which include the infrared spectram of frozen molecules in the infrared, complex refractive index and the 3D molecule viewer.

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
    src: "https://www.aanda.org/articles/aa/full_html/2022/12/aa44032-22/aa44032-22-fig3.jpg",
    caption: "H2O ice spectrum in the infrared."
  },
  {
    src: "https://www.aanda.org/articles/aa/full_html/2022/12/aa44032-22/aa44032-22-fig4.jpg",
    caption: "H2O ice complex refractive index."
  },
  {
    src: "https://www.aanda.org/articles/aa/full_html/2022/12/aa44032-22/aa44032-22-fig5.jpg",
    caption: "3D molecule viewer."
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
