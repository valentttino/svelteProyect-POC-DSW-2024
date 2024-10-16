<script>
  export let text
</script>

<style>
  .welcome-section{
    background-color: #201E43;
    color: white;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 100%;
  }

  h1{
    margin:0;
    font-size: 2.5rem;
  }
</style>

<div class="welcome-section">
  <h1>
    {text}
  </h1>
</div>