<script>
    export let imageSrc = '';  
    export let title = '';    
    export let text = '';      
  </script>
  
  <style>
    a{
      text-decoration: none;
      color: black;
    }

    .article-container {
      display: flex;
      align-items: flex-start;
      padding: 16px;
      border-radius: 8px;
      margin-bottom: 16px;
    }
  
    .article-image {
      width: 150px;
      height: 150px;
      object-fit: cover;
      margin-right: 16px;
    }
  
    .article-content {
      flex: 1;
    }
  
    .article-title {
      font-size: 1.5em;
      margin: 0;
      margin-bottom: 8px;
    }
  
    .article-text {
      font-size: 1em;
      color: #666;
    }
  </style>
 
<a href="/desarrollo">
  <div class="article-container">
    <img src={imageSrc} alt={title} class="article-image" />
    <div class="article-content">
      <h2 class="article-title">{title}</h2>
      <p class="article-text">{text}</p>
    </div>
  </div>
</a>