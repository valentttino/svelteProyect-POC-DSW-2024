<script>
    export let textodescr
    import logo from '../assets/facultad-icon.svg';


  </script>
  
  <style>
    body{
        background-color: #201E43;
    color: white;
    display: flex; 
    flex-direction: column;
    justify-content: center; 
    align-items: center; 
    height: 100vh; 
    margin: 0; 
    padding: 100px;
    }
    img {
    height: 100px; 
    margin-right: 10px; 
  }

  h6 {
    display: flex;
    align-items: center; 
    margin: 0; 
  }

  </style> 

  
  <body>
    <h6>
        <img src={logo} alt="Logo Facultad" />
    
      {textodescr}
    </h6>
  </body>