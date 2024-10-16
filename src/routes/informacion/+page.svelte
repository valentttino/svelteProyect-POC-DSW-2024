<script>
  import Header from '../../components/Header.svelte'
  import CardGrid from '../../components/CardGrid.svelte'
  import Footer from '../../components/Footer.svelte'
	import OpeningHours from '../../components/OpeningHours.svelte';

  let sections = [{section: "Autogestión Alumnos", icon: "../assets/user-icon.svg"},
                  {section: "Autogestión Docentes", icon: "../assets/user-icon.svg"},
                  {section: "CVG", icon: "../assets/user-icon.svg"}
                ];
  
</script>

<style>
  :global(body){
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    margin: 0;
  }

  :global(.back){
    background-color: #EEEEEE;
    padding: 20px;
  }

    main {
    flex: 1;
  }
</style>

<Header />
<main>
  <h1>Información</h1>
  <section class='back'>
    <CardGrid itemsInfo={sections}/>
  </section>
  <OpeningHours/>
</main>

<Footer />
