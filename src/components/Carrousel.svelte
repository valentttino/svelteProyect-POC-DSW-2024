<script>
  let currentIndex = 0;
  const slides = [
    {
      image: "/src/assets/image1.jpg",
      title: "Ciencia y Tecnología para la Sociedad",
      description: "Nuestros estudiantes desarrollan proyectos reales y adquieren habilidades para transformar el mundo."
    },
    {
      image: "/src/assets/image2.jpg",
      title: "Vive la Experiencia UTN",
      description: "Explora nuestras instalaciones de investigación y disfruta de nuestras actividades sociales."
    },
    {
      image: "/src/assets/image4.jpg",
      title: "Nos visita Maslatón",
      description: "Recibimos una visita de parte del reconocido influencer financiero, quien dio una charla para alumnos avanzados en distintas carreras."
    }
  ];

  function next() {
    currentIndex = (currentIndex + 1) % slides.length;
  }

  function prev() {
    currentIndex = (currentIndex - 1 + slides.length) % slides.length;
  }
</script>

<style>
  .novedades{
    background-color: #EEEEEE;
    text-align: center;
    padding: 20px 0;
  }

  h1{
    margin: 0;
    font-size: 2rem;
  }

.carousel {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  width: 100%;
  height: 470px; 
  background-color: #EEEEEE; 
  overflow: hidden;
}

.carousel img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain; 
  background-color: black;
  transition: transform 0.5s ease-in-out;
}

.text-overlay {
  position: absolute;
  bottom: 20px; 
  left: 50%; 
  transform: translateX(-50%);
  color: white;
  background-color: rgba(0, 0, 0, 0.5);
  padding: 10px;
  text-align: center; 
  border-radius: 5px;
  max-width: 40%;
}

.text-overlay h2 {
  margin: 0;
  font-size: 24px;
}

.text-overlay p {
  margin: 5px 0 0;
  font-size: 16px;
}

.buttons {
  position: absolute;
  top: 50%; 
  width: 100%;
  display: flex;
  justify-content: space-between;
  transform: translateY(-50%);
}

.prev, .next {
  background-color: rgba(0, 0, 0, 0.5);
  border: none;
  color: white;
  padding: 10px;
  cursor: pointer;
  border-radius: 8px;
}

.prev {
  position: absolute;
  left: 20px;
}

.next {
  position: absolute;
  right: 20px;
}
</style>

<div class="novedades">
  <h1>NOVEDADES</h1>
</div>
<div class="carousel">
  <img src={slides[currentIndex].image} alt={slides[currentIndex].description} />
  <div class="text-overlay">
    <h2>{slides[currentIndex].title}</h2>
    <p>{slides[currentIndex].description}</p>
  </div>
    <div class="buttons">
      <button class="prev" on:click={prev}>&lt;</button>
      <button class="next" on:click={next}>&gt;</button>
    </div>
</div>