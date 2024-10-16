<script>
  import user from '../assets/user-icon.svg'
  export let section
</script>

<style>
  .icon {
    width: 70px;
    height: 70px;
  }

  .container {
    text-align: center;
    font-weight: bold;
    color: black;
  }
</style>

<figure class="container">
  <img src={user} alt="User Icon" class="icon" />
    <h4><b>{section}</b></h4> 
</figure>
