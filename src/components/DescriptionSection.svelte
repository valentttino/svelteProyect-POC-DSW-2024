<script>
  export let textodescr
  import logo from '../assets/facultad-icon.svg'
</script>


<style>
  .wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh; 
    background-color: #EEEEEE; 
  }

  .content {
    background-color: #EEEEEE;
    color: black;
    display: flex; 
    flex-direction: row; 
    justify-content: flex-start; 
    align-items: center; 
    padding: 50px;
    max-width: 65%;
  }

  .logo-container {
    background-color: #2A2A5E;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 150px;
    height: 200px;
    margin-right: 20px;
  }

  img {
    height: 100px; 
    filter: invert(1);
  }

  p {
    margin: 0;
    text-align: justify;
  }
</style>

<div class="wrapper">
  <div class="content">
    <div class="logo-container">
      <img src={logo} alt="Logo Facultad" />
    </div>
    <p>{textodescr}</p>
  </div>
</div>
