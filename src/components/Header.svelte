<script>
  import { page } from '$app/stores'
  const utnLogo = "https://caimasegall.com.ar/wp-content/uploads/2020/08/logo-UTN-1.png"
</script>


<style>
  header {
    background-color: #EEEEEE;
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

  .active {
    font-weight: bold; 
    border-bottom: 2px solid #201E43;
  }
</style>

<header>
  <nav>
    <ul>
      <li>
        <a href="/">
          <img src={utnLogo} alt="UTN Logo">
        </a>
      </li>
      <li>
        <a href="/" class={$page.url.pathname === '/' ? 'active' : ''}>Inicio</a>
      </li>
      <li>
        <a href="/carreras" class={$page.url.pathname === '/carreras' ? 'active' : ''}>Carreras</a>
      </li>
      <li>
        <a href="/institucional" class={$page.url.pathname === '/institucional' ? 'active' : ''}>Institucional</a>
      </li>
      <li>
        <a href="/informacion" class={$page.url.pathname === '/informacion' ? 'active' : ''}>Información</a>
      </li>
    </ul>
  </nav>
</header>