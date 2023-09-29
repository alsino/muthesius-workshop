<script>

  let projects = [
    {
      title: "Gaardener Neubaumonitor",
      subtitle: "Große Neubauprojekte verändern den Stadt-und Sozialraum Gaards nachhaltig und zeigen schon jetzt ihren Einfluss auf die Lebensrealitäten der Anwohner*innen.",
      authors: "Flora Wedel, Carolin Birkners",
      url: "https://www.google.de",
      img: "neubau.png"
    },
    {
      title: "Schnelle Badung",
      subtitle: "Kiel liegt direkt an der Ostsee, aber nur ein kleiner Bereich ist zum Baden zugänglich. Finde heraus welcher Badeort am schnellsten erreichbar ist",
      authors: "Mialena Kneschke, Adrian Herzig", 
      url: "https://adriangreyish.github.io/Wepmapping_Badestellen/",
      img: "badung.png"
    },
    {
      title: "Femizide in Deutschland 2023 – One Billion Rising",
      subtitle: "Invisible map der globalen Initiative “One Billion Rising” gegen Gewalt an Frauen und Mädchen in Deutschland 2023 ",
      authors: "Selina Meier, Levke Ohm, Ainoa Policke",
      url: "https://ainoaplck.github.io/intro-code/",
      img: "onebillion.png"
    },
    {
      title: "Public Trees of Hamburg",
      subtitle: "Mapping Hamburg’s trees by location, size and age.",
      authors: "Emily Steiner, Gunnar Kähler",
      url: "https://baum-map2.vercel.app/",
      img: "baum.png"
    }
  ]
</script>

<div class="wrapper">

  <h1>The Invisible Map</h1>
  <h3>Visualizing spatial contrasts with open data and web maps</h3>
  <div>
    These are the project results of the 1-week workshop <span style="font-style:italic;">»The Invisible Map - Visualizing spatial contrasts with open data and web maps«</span>, held at Muthesius Kunshochschule in Kiel, Germany from 25 - 29 September 2023. This course was an introduction to the world of web mapping and geospatial data visualization. The students explored different urban and social phenomena by mapping highly contrasting datasets using open data sources, which can tell interesting stories about our world and highlight social issues. Below the selection of the different projects produced during the workshop week.
  </div>
  <br>

  <section class="grid">
    {#each projects as proj}
    <a target="_blank" href={proj.url} class="project">
      <div class="project-container">
        <img src={proj.img} alt="" class="img">
        <div class="title">{proj.title}</div>
        <div>{proj.subtitle}</div>
        <div class="authors">{proj.authors}</div>
      </div>
      
    </a>
    {/each}
    


  </section>
 
</div>


<style>
   @import url('https://fonts.googleapis.com/css2?family=DM+Mono&family=DM+Sans:wght@400;700&family=IBM+Plex+Sans&family=Martian+Mono&display=swap');


    

   h1 {
    /* font-family: 'DM Mono', monospace; */
    font-family: 'DM Sans', sans-serif;
    margin: 0.5em 0;
   }


  .wrapper {
    font-family: 'DM Sans', sans-serif;
    line-height: 1.5;
    padding: 1.5em 5em 5em 5em ;
  }

  .grid {
    margin-top: 2em;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .project {
    color: black;
    margin-bottom: 3em;
    max-width: 600px;
    transition: all 0.5s;
  }

  .project:hover {
    transform: translateY(-5px);
  }

  
  .title {
    font-weight: bold;
  }

  a{
    text-decoration: none;
  }

  .authors {
    font-style: italic;
    margin-top: 0.5em;;
  }

  img {
    width: 550px;
    height: auto;
  }

 
</style>
