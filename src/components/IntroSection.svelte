<script>
  export let text
  export let subtitle

  if (subtitle===undefined){
    subtitle = ""
  }
</script>

<style>
  .intro-section {
    background-color: #201E43;
    color: white;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 30vh;
    width: 100%; 
  }

  h1 {
    margin: 0;
    font-size: 2.5rem; 
  }

  h2{
    font-size: large;
    margin-top: 10px;
  }
</style>

<div class="intro-section">
  <h1>{text}</h1>
  <h2>{subtitle}</h2>
</div>