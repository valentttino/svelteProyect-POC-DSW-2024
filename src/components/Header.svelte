<script>
  const utnLogo = "https://caimasegall.com.ar/wp-content/uploads/2020/08/logo-UTN-1.png"
</script>


<style>
  header {
    background-color: #fff;
    padding: 10px;
    box-shadow: 0px 2px 2px -2px gray;
  }

  nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  ul {
    display: flex;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;
  }

  li {
    margin-left: 35px;
  }

  img {
    height: 30px;
  }

  a {
    text-decoration: none;
    color: black;
    font-weight: bold;
    font-size: 18px;
  }

  a:hover {
    color: #333;
  }
</style>

<header>
  <nav>
    <ul>
      <li>
        <img src={utnLogo} alt="UTN Logo">
      </li>
      <li><a href="/">Inicio</a></li>
      <li><a href="/carreras">Carreras</a></li>
      <li><a href="/institucional">Institucional</a></li>
      <li><a href="/informacion">Información</a></li>
    </ul>
  </nav>
</header>