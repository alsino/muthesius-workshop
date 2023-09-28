<script>

  let projects = [
    {
      title: "Bäume in Hamburg",
      subtitle: "A cool project",
      authors: "Kim, Peter",
      url: "http://www.google.de"
    },
    {
      title: "Neubau in Kiel",
      subtitle: "A cool project",
      authors: "Kim, Peter",
      url: "http://www.google.de"
    },
    {
      title: "Femizide in Deutschland",
      subtitle: "A cool project",
      authors: "Kim, Peter",
      url: "http://www.google.de"
    },
    {
      title: "Badestellen in Kiel",
      subtitle: "A cool project",
      authors: "Kim, Peter", 
      url: "http://www.google.de"
    }
  ]
</script>



<div class="wrapper">

  <h1>The Invisible Map</h1>
  <h2>Visualizing spatial contrasts with open data and web maps</h2>
  <div>
    This course is an introduction to the world of web mapping and geospatial data visualization. We will explore different urban and social phenomena by mapping highly contrasting datasets, which can tell interesting stories about our world. For example, how could we compare different speeds of a city (slow vs. fast), varying levels of openness of space (public vs. private), the different histories of its parts (east vs. west), the age of the architecture (old vs. new) or any other type of contrast imaginable. Topics can be simple or complex, at the local or global scale.
  </div>
  <br>

  <section class="grid">
    {#each projects as proj}
    <a target="_blank" href={proj.url} class="project">
      <div class="project-container">
        <img src="https://placehold.co/300x300" alt="" >
        <div class="title">{proj.title}</div>
        <div>{proj.subtitle}</div>
        <div>{proj.authors}</div>
      </div>
      
    </a>
    {/each}
    


  </section>
 
</div>


<style>
   @import url('https://fonts.googleapis.com/css2?family=DM+Mono&family=DM+Sans:wght@400;700&family=IBM+Plex+Sans&family=Martian+Mono&display=swap');


    

   h1, h2{
    font-family: 'DM Mono', monospace;
    /* color: #8330FE; */
    margin: 0.5em 0;
   }



   h2 {
    margin-bottom: 2em;
   }


  .wrapper {
    font-family: 'DM Sans', sans-serif;
    line-height: 1.5;
    padding: 1.5em 5em 5em 5em ;
  }

  .grid {
    margin-top: 1em;
    display: flex;
   justify-content: space-between;
  }

  .project {
    color: #8330FE;
  }

  .project:hover{
    color: #0D00C2;
  }

  
  .project-container{
    /* padding: 2em; */
    /* border-radius: 5px; */
    /* box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1); */
  }

  .title {
    font-weight: bold;
  }

  a{
    text-decoration: none;
  }

 
</style>
