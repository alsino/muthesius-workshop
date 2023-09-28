<script>

  let projects = [
    {
      title: "Project 1",
      subtitle: "A cool project",
      authors: "Kim, Peter"
    },
    {
      title: "Project 2",
      subtitle: "A cool project",
      authors: "Kim, Peter"
    },
    {
      title: "Project 3",
      subtitle: "A cool project",
      authors: "Kim, Peter"
    },
    {
      title: "Project 4",
      subtitle: "A cool project",
      authors: "Kim, Peter"
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
  <!-- <div>
    A main objective of the course is to give an introduction to a couple of different mapping tools (open source where possible), which can be used to create interactive maps on different devices. These tools are easy to handle, even if you have little or no background in programming, but can also be used for more advanced projects by expanding the functionalities with code. The course will also show you where to find open geodata (i.e. OpenStreetMap) and how to use it in conjunction with these tools.
  </div> -->

  <section class="grid">
    {#each projects as proj}
    <a href="#" class="project">
      <img src="https://placehold.co/300x300" alt="">
      <div class="title">{proj.title}</div>
      <div>{proj.subtitle}</div>
      <div>{proj.authors}</div>
    </a>
    {/each}
    


  </section>
 
</div>


<style>
   @import url('https://fonts.googleapis.com/css2?family=DM+Mono&family=DM+Sans:wght@400;700&family=IBM+Plex+Sans&family=Martian+Mono&display=swap');

   h1, h2{
    font-family: 'DM Mono', monospace;
   }

  .wrapper {
    font-family: 'DM Sans', sans-serif;
    line-height: 1.5;
    padding: 1em 5em 5em 5em ;
  }

  .grid {
    margin-top: 1em;
    display: flex;
   justify-content: space-between;
  }

  .title {
    font-weight: bold;
  }

  a{
    text-decoration: none;
  }
</style>
