<script>
  import diploma from '../assets/diploma-icon.svg'
  export let section
</script>

<style>
  .icon {
    width: 50px;
    height: 50px;
    filter: brightness(0) invert(1);
  }

  .container{
    text-align: center;
    font-weight: bold;
  }
</style>
<div>
  <img src={diploma} alt="Diploma Icon" class="icon" />
  <div class="container">
    <h4><b>{section}</b></h4>
  </div>
</div>


