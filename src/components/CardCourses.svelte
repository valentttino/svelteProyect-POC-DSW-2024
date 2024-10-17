<script>
  export let title
</script>

<style>
  a{
    text-decoration: none;
    color: black;
  }
  
  .container{
    height: 200px;
    width: 250px;
    border: 2px;
    border-style: solid;
    border-color: #201E43;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .neutroColor{
    width: 100%;
    height: 65%;
    background-color: #201E43;
  }

  .text{
    width: 100%;
    height: 35%;
    text-align: center;
    font-weight: bold;
    display: flex;
    flex-wrap: wrap;
    align-content: center;
  }
</style>

<a href="/desarrollo">
  <div class="container">
    <div class="neutroColor">
    </div>
    <div class="text">
      {title}
    </div>
  </div>
</a>