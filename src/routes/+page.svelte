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
</style>

<Header />
<WelcomeSection text={text}/>
<Card section={"Licenciaturas"}/>
<CardGrid {data} />
<DescriptionSection />
<Footer />
