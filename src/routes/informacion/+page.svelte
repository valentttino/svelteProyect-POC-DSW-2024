<script>
  import Header from '../../components/Header.svelte'
  import CardGrid from '../../components/CardGrid.svelte'


  let sections = [{section: "Autogestión Alumnos", icon: "../assets/user-icon.svg"},
                  {section: "Autogestión Docentes", icon: "../assets/user-icon.svg"},
                  {section: "CVG", icon: "../assets/user-icon.svg"}
                ];
</script>

<Header />
<h1>Información</h1>

<section>
  <CardGrid itemsInfo={sections}/>
</section>
