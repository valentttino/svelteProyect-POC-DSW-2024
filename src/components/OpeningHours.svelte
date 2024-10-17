<script>
  import horarios from "../data/horarios.json";
</script>

<style>
  .info-box {
    background-color: #EEEEEE;
    padding: 20px;
    margin: 20px auto;
    max-width: 90%;
    text-align: left;
    display: flex; 
    flex-direction: row; 
    justify-content: space-between; 
    align-items: flex-start; 
  }

  .text-container {
    flex: 1; 
  }

  .info-box p {
    padding: 5px;
    margin: 0;
    font-size: 1.1em;
    color: #333;
  }

  .map-container {
    width: 250px; 
    height: 250px; 
    position:relative; 
  }

  .map-container iframe {
    width: 100%; 
    height: 100%; 
    border: 1px solid black; 
    position: absolute; 
  }
</style>

<div class="info-box">
  <div class="text-container">
    <p><strong>Alumnos y público general</strong></p>
    <p>{horarios.horariosAlumnos}</p>
    <br>
    <p><strong>Egresados</strong></p>
    <p>{horarios.horariosEgresados}</p>
    <br>
    <p> {horarios.direccion}</p>
    <p> {horarios.telefono}</p>
  </div>

  <div class="map-container">
    <iframe
      title="Mapa de la Facultad" 
      src="https://www.openstreetmap.org/export/embed.html?bbox=-60.646368%2C-32.957713%2C-60.641370%2C-32.951514&layer=mapnik&marker=-32.954613%2C-60.643869&zoom=19"
      allowfullscreen=""
      loading="lazy"></iframe>
  </div>
</div>
