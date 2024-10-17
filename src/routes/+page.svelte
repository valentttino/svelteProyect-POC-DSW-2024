<script>
  import Header from '../components/Header.svelte'
  import WelcomeSection from '../components/WelcomeSection.svelte'
  import CardGrid from '../components/CardGrid.svelte'
  import DescriptionSection from '../components/DescriptionSection.svelte'
  import Footer from '../components/Footer.svelte'
  
  let sections = [{urlCard:"/desarrollo", section: "Diplomaturas"},
                  {urlCard:"/tecnicaturas", section: "Tecnicaturas"},
                  {urlCard:"/desarrollo", section: "Licenciaturas"},
                  {urlCard:"/desarrollo", section: "Maestrías"},
                  {urlCard:"/desarrollo", section: "Ingenierías"},
                  {urlCard:"/desarrollo", section: "Especializaciones"}
                ]

  const text="Bienvenido a la UTN Rosario"


  const textodescr="En Rosario, la Facultad Regional de la Universidad Tecnológica Nacional tiene sus orígenes en 1953 sobre la base de la Escuela Fábrica N° 40 (hoy E.E.T. N° 468) y del Ciclo Técnico (que funcionaba en el actual Colegio Nacional N° 2), dependientes ambos de la Comisión Nacional de Aprendizaje y Orientación Profesional. El primer Secretario Técnico fue el Ing. Giordano Marchiori, quien conformó las primeras cátedras e inscribió los primeros alumnos en las carreras de: Ingeniería Mecánica, Ingeniería en Construcciones e Ingeniería Electromecánica. A más de 65 años de aquellos comienzos, seguimos avanzando ofreciendo a la comunidad formación académica de excelencia."
</script>

<style>
  :global(body){
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    margin: 0;
  }

  :global(.back){
    background-color: #EEEEEE;
  }

  main {
    flex: 1;
  }
</style>

<Header />
<main>
  <WelcomeSection text={text}/>
  <section class='back'>
    <CardGrid itemsInicio={sections}/>
    <DescriptionSection textodescr={textodescr}/>
  </section>
</main>
<Footer />
