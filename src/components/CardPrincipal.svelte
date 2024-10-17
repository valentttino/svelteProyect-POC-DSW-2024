<script>
  import diploma from '../assets/diploma-icon.svg'
  export let section

</script>

<style>
  .container {
    background-color: #201E43;
    height: 200px;
    width: 200px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 10px;
    transition: transform 0.3s ease, background-color 0.3s ease;
  }

  .container:hover {
    transform: scale(1.05); 
  }

  .icon {
    width: 60px;
    height: 60px;
    filter: brightness(0) invert(1); 
  }

  .text {
    color: #EEEEEE;
    text-align: center;
    font-weight: bold;
    margin-top: 10px; 
    font-size: 16px;
  }

  a {
    text-decoration: none;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>

<a href="/">
  <div class="container">
      <img src={diploma} alt="Diploma Icon" class="icon" />
      <div class="text">
        {section}
      </div>
  </div>
</a>

