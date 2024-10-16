<script>
    export let textodescr
    import logo from '../assets/facultad-icon.svg';


  </script>
  
  <style>
    body{
        background-color: #EEEEEE;
       color: black;
       display: flex; 
       flex-direction: column;
       justify-content: flex; 
        align-items: center; 
       height: 100vh; 
       margin: 0; 
       padding: 50px;
    }
    img {
    height: 100px; 
    margin-left: 10px; 
  }
  .content {
    display: flex;
    align-items: center; 
    max-width: 50%; 
  }


  h6 {
   display: flex;
    align-items: center; 
    margin: 0; 

  }

  </style> 

  
  <body>
    <div class="content">
    <h6>
        <img src={logo} alt="Logo Facultad" />
    
      {textodescr}
    </h6>
  </div>
  </body>