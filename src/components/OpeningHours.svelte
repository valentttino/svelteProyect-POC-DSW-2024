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
  }

  .info-box h2 {
    font-size: 1.5em;
    margin: 0;
    padding-bottom: 30px;
    text-align: center;
    color: #333;
  }

  .info-box p {
    padding:5px;
    margin:0;
    font-size: 1.1em;
    color: #333;
  }
</style>

<div class="info-box">
  <h2>HORARIOS DE ATENCIÓN</h2>

  <p><strong>Alumnos y público general</strong></p>
  <p>{horarios.horariosAlumnos}</p>
  <br>
  <p><strong>Egresados</strong></p>
  <p>{horarios.horariosEgresados}</p>
  <br>
  <p>{horarios.direccion}</p>
  <p>{horarios.telefono}</p>
</div>
