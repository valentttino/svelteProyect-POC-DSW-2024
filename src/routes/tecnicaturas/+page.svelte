<script>
  import Header from "../../components/Header.svelte"
  import IntroSection from "../../components/IntroSection.svelte"
  import CardGrid from "../../components/CardGrid.svelte"
  import Footer from "../../components/Footer.svelte"

  const description = "Las Tecnicaturas Universitarias son carreras cortas que perimiten una rápida salida laboral que de respuesta a necesidades del medio, proporcionando a éste recursos humanos altamente capacitados."
  const courses = [
    {title: "Tecnicatura Universitaria en Programación"},
    {title: "Tecnicatura Universitaria en Mantenimiento Industrial"},
    {title: "Tecnicatura Universitaria en Administración"}
  ]
</script>

<Header />
<IntroSection text={"Tecnicaturas"} subtitle={description}/>
<CardGrid itemsCourses={courses}/> 
<Footer />