<script>
  import Header from "../../components/Header.svelte"
  import IntroSection from "../../components/IntroSection.svelte"
  import Carrousel from "../../components/Carrousel.svelte"
  import Article from "../../components/Article.svelte"
  import Footer from "../../components/Footer.svelte"
  import news from "../../data/news.json"

</script>

<Header />
<IntroSection text={"Institucional"} />
<Carrousel />
<div class="news-container">
  {#each news as article (article.id)}
    <Article 
      imageSrc={article.urlImage} 
      title={article.title} 
      text={article.description}
    />
  {/each}
</div>
<Footer />