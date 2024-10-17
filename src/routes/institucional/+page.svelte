<script>
  import Header from "../../components/Header.svelte"
  import IntroSection from "../../components/IntroSection.svelte"
  import Carrousel from "../../components/Carrousel.svelte"
  import Article from "../../components/Article.svelte"
  import Footer from "../../components/Footer.svelte"

</script>

<Header />
<IntroSection text={"Institucional"} />
<Carrousel />
<Article imageSrc={"https://i.info7.mx/img/i7/4020000/4022879_mono-fumando.jpg"} title={"Mono de pana"} text={"Se lo ve bien de pana al pedazo de macaco este."}/>
<Article imageSrc={"https://pbs.twimg.com/media/FTe9q3pXoAEBy3B.jpg"} title={"Mono disfrutando su cigarrito"} text={"Se lo ve bien gostoso a este buen mamífero disfrutando su enrolado de tabaco."}/>
<Footer />