<script>
  import CardInfo from "./CardInfo.svelte"
  import CardPrincipal from "./CardPrincipal.svelte"

  export let itemsInicio = [];
  export let itemsInfo = [];
</script>

<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    gap: 20px; 
    max-width: 80%; 
    padding: 2% 0%;
    margin: 0 auto; 
  }

  .sin-subrayar{
    text-decoration: none;
  }

</style>


<div class="grid-container">
  {#each itemsInfo as {section, icon, link}}
    <a href={link} class="sin-subrayar"><CardInfo section={section} icon={icon}/></a>
  {/each}
</div>

<div class="grid-container">
  {#each itemsInicio as {section, icon}}
    <CardPrincipal section={section} icon={icon}/>
  {/each}
</div>
