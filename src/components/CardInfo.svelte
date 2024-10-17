<script>
  import user from '../assets/user-icon.svg'
  export let link
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
  <a href={link}>
    <img src={user} alt="User icon" class="icon" />
    <h4><b>{section}</b></h4>
  </a>
</figure>
