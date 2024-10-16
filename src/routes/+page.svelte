<script>
  import Header from '../components/Header.svelte'
  import WelcomeSection from '../components/WelcomeSection.svelte'
  import CardGrid from '../components/CardGrid.svelte'
  import DescriptionSection from '../components/DescriptionSection.svelte'
  import Footer from '../components/Footer.svelte'

  import Card from '../components/Card.svelte'

  import data from '../data/data.json'
  console.log(data)

  const text="Bienvenido a la UTN Rosario"
 


  const textodescr="En Rosario, la Facultad Regional de la Universidad Tecnológica Nacional tiene sus orígenes en 1953 sobre la base de la Escuela Fábrica N° 40 (hoy E.E.T. N° 468) y del Ciclo Técnico (que funcionaba en el actual Colegio Nacional N° 2), dependientes ambos de la Comisión Nacional de Aprendizaje y Orientación Profesional. El primer Secretario Técnico fue el Ing. Giordano Marchiori, quien conformó las primeras cátedras e inscribió los primeros alumnos en las carreras de: Ingeniería Mecánica, Ingeniería en Construcciones e Ingeniería Electromecánica. A más de 65 años de aquellos comienzos, seguimos avanzando ofreciendo a la comunidad formación académica de excelencia."
</script>

<style>
  :global(body){
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

    .CardContainer {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    max-width: 50%; 
    padding-top: 5%;
    margin: 0 auto; 
  }


</style>

<Header />
<WelcomeSection text={text}/>
<div class="CardContainer">
  <Card section={"Diplomaturas"}/>
  <Card section={"Tecnicaturas"}/>
  <Card section={"Licenciaturas"}/>
  <Card section={"Maestrías"}/>
  <Card section={"Ingenierías"}/>
  <Card section={"Especializaciones"}/>
</div>
<CardGrid {data} />
<DescriptionSection textodescr={textodescr}/>
<Footer />
