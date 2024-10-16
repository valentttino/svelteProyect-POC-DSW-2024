<script>
  import Header from '../components/Header.svelte'
  import WelcomeSection from '../components/WelcomeSection.svelte'
  import CardGrid from '../components/CardGrid.svelte'
  import DescriptionSection from '../components/DescriptionSection.svelte'
  import Footer from '../components/Footer.svelte'


  import data from '../data/data.json'
  
  let sections = [{section: "Diplomaturas", icon: "../assets/diploma-icon.svg"},
                  {section: "Tecnicaturas", icon: "../assets/diploma-icon.svg"},
                  {section: "Licenciaturas", icon: "../assets/diploma-icon.svg"},
                  {section: "Maestrías", icon: "../assets/diploma-icon.svg"},
                  {section: "Ingenierías", icon: "../assets/diploma-icon.svg"},
                  {section: "Especializaciones", icon: "../assets/diploma-icon.svg"}
                ]
  console.log(data)

  const text="Bienvenido a la UTN Rosario"
</script>

<style>
  :global(body){
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  .back{
    background-color: #EEEEEE;
  }
</style>

<Header />
<WelcomeSection text={text}/>
<section class='back'>
  <CardGrid itemsInicio={sections}/>
  <DescriptionSection />
</section>
<Footer />
