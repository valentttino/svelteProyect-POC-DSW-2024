<script>
  let name = ''
  let phone = ''
  let mail = ''
  let message = ''

  function handleSubmit(event) {
    event.preventDefault();
    alert("Formulario enviado con éxito")

    name = ''
    phone = ''
    mail = ''
    message = ''
  }
</script>

<style>
  h2{
    color:black;
    font-weight: 400;
    text-align: left;
  }
  
  form{
    text-align: center;
  }

  label{
    display: none;
  }
  
  input[type=text], [type=phone], [type=mail], textarea {
  width: 100%;
  padding: 12px; 
  border: 1px solid #ccc; 
  border-radius: 4px; 
  box-sizing: border-box; 
  margin-top: 6px; 
  margin-bottom: 16px; 
  resize: vertical 
}

input[type=submit] {
  background-color: black;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  align-items: center;
}

input[type=submit]:hover {
  background-color: #134B70;
}

.container {
  padding: 20px;
}

::placeholder {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; /* Ensure it uses the same font */
  }
</style>

<div class="container">
  <h2>FORMULARIO DE CONTACTO</h2>

  <form on:submit={handleSubmit}>

    <label for="name">Nombre</label>
    <input type="text" id="name" bind:value={name} placeholder="Nombre*">

    <label for="phone">Teléfono</label>
    <input type="phone" id="phone" bind:value={phone} placeholder="Teléfono*">

    <label for="mail">Mail</label>
    <input type="mail" id="mail" bind:value={mail} placeholder="Mail*">

    <label for="message">Mensaje</label>
    <textarea id="message" bind:value={message} placeholder="Mensaje*" style="height:200px"></textarea>

    <input type="submit" value="ENVIAR CONSULTA">

  </form>
</div>