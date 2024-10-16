<script>
  import Header from '../../components/Header.svelte'
  import IntroSection from '../../components/IntroSection.svelte'
  import CardGrid from '../../components/CardGrid.svelte'
  import ContactForm from '../../components/ContactForm.svelte'
  import Footer from '../../components/Footer.svelte'

  let sections = [{section: "Autogestión Alumnos", icon: "../assets/user-icon.svg"},
                  {section: "Autogestión Docentes", icon: "../assets/user-icon.svg"},
                  {section: "CVG", icon: "../assets/user-icon.svg"}
                ]
</script>

<style>

</style>

<Header />
<IntroSection text={"Información"}/>

<section class="back">
  <CardGrid itemsInfo={sections}/>
  <ContactForm />
</section>

<Footer />
