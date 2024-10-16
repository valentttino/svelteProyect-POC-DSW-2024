<script>
    let currentIndex = 0;
    const slides = [
      {
        image: "/src/assets/image1.jpg",
        title: "Título 1",
        description: "Descripción breve de la primera imagen."
      },
      {
        image: "/src/assets/image2.jpg",
        title: "Título 2",
        description: "Descripción breve de la segunda imagen."
      },
      {
        image: "/src/assets/image3.jpg",
        title: "Título 3",
        description: "Descripción breve de la tercera imagen."
      },
      {
        image: "/src/assets/image4.jpg",
        title: "Nos visita Maslatón",
        description: "Recibimos una visita de parte del reconocido influencer financiero, quien dió una charla para alumnos avanzados en distintas carreras."
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
    .carousel {
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      width: 100%;
      height: 450px;
      overflow: hidden;
    }
  
    .carousel img {
      width: 600px;
      height: 450px;
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
  
    .prev {
      left: 380px; 
      position: absolute;
      transform: translateY(-50%);
    }
  
    .next {
      right: 380px; 
      position: absolute;
      transform: translateY(-50%);
    }
  
    .button {
      background-color: rgba(0, 0, 0, 0.5);
      border: none;
      color: white;
      padding: 10px;
      cursor: pointer;
      border-radius: 8px;
    }
  </style>
  
  <div class="carousel">
    <img src={slides[currentIndex].image} alt="Image Carousel" />
    <div class="text-overlay">
      <h2>{slides[currentIndex].title}</h2>
      <p>{slides[currentIndex].description}</p>
    </div>
    <div class="buttons">
      <button class="button prev" on:click={prev}>&lt;</button>
      <button class="button next" on:click={next}>&gt;</button>
    </div>
  </div>