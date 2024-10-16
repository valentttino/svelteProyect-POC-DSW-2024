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

</style>


<div class="grid-container">
  {#each itemsInfo as {section, icon}}
    <CardInfo section={section} icon={icon}/>
  {/each}
</div>

<div class="grid-container">
  {#each itemsInicio as {section, icon}}
    <CardPrincipal section={section} icon={icon}/>
  {/each}
</div>
