<script>
  import CardInfo from "./CardInfo.svelte"
  import Card from "./Card.svelte"

  export let itemsInicio = [];
  export let itemsInfo = [];
</script>

<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    gap: 20px; 
    max-width: 80%; 
    padding-top: 5%;
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
    <Card section={section} icon={icon}/>
  {/each}
</div>
