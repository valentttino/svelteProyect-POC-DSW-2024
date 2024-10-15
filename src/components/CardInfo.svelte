<script>
  import user from '../assets/user-icon.svg'
  export let section
</script>

<style>
  .icon {
    width: 70px;
    height: 70px;
    filter: brightness(0) invert(1);
  }

  .container {
    text-align: center;
    font-weight: bold;
  }
</style>

<figure class="container">
  <img src={user} alt="User Icon" class="icon" />
    <h4><b>{section}</b></h4> 
</figure>
