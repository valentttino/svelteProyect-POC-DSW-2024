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
<DescriptionSection />
<Footer />
