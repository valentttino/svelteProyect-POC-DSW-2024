<script>
  export let title
</script>

<style>
  .container{
    height: 150px;
    width: 180px;
    border: 2px;
    border-color: #201E43;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .neutroColor{
    width: 100%;
    height: 70%;
    background-color: #201E43;
  }

  .text{
    width: 100%;
    height: 30%;
    text-align: center;
    align-items: center;
  }
</style>

<div class="container">
  <div class="neutroColor">
  </div>
  <div class="text">
    {title}
  </div>
</div>
