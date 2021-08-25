<template>
  <main>
    <section>
      <div id="content">
        <h1>Get <b>insights</b> that help your business grow.</h1>
        <p>Discover the benefits of data analytics and make better decisions regarding revenue, customer 
        experience, and overall efficiency.</p>
        <div class="stats">
          <div class="companies">
            <h1>10k+</h1>
            <p>COMPANIES</p>
          </div>
          <div class="templates">
            <h1>314</h1>
            <p>TEMPLATES</p>
          </div>
          <div class="queries">
            <h1>12M+</h1>
            <p>QUERIES</p>
          </div>
        </div>
      </div>
      <div id="image">
      </div>
    </section>
    <div class="attribution">
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
      Coded by <a href="https://github.com/Antoni0o">Antoni0o</a>.
  </div>
  </main>
</template>

<script>
export default {
  name: 'StatsPreviewComponent'
}
</script>

<style scoped>
  main {
    height: 100vh;
    
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .attribution {
    text-align: center;
    text-decoration: none;
  }

  .attribution a {
    color: var(--purple);
  }

  section {
    width: 75vw;
    height: 60vh;

    display: grid;
    grid-template-columns: 1fr 1fr;
    margin: 2rem;

    background-color: var(--dark-blue);
    border-radius: 0.5rem;
  }
  
  /* Content */ 
  #content {
    margin: 7rem 7rem 2rem 7rem;
  }

  /* Texts */ 
  #content h1 {
    font-size: 4rem;
  }
  #content h1 b {
    color: var(--purple);
  }

  #content p {
    font-size: 2rem;
    line-height: 3rem;
    font-family: 'Inter', sans-serif;
    color: var(--transparent-white);
  }
  
  /* Stats */
  #content .stats {
    display: flex;
    margin-top: 7rem;

    gap: 10rem;
  }

  #content .stats h1 {
    font-size: 3rem;
    
    margin-bottom: 0.7rem;
  }

  #content .stats p {
    font-family: 'Lexend Deca', sans-serif;
    font-size: 1.8rem;
    
    margin-top: 0.2rem;
  }

  /* Image */
  section #image {
    position: relative;
    
    background-image: url(/images/image-header.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    border-radius: 0 0.5rem 0.5rem 0; 
  }


  section #image::after {
    content: "";
    
    position: absolute;
    width: 100%;
    height: 100%;

    background-color: #5d0788;
    opacity: 0.5;
    
    overflow: hidden;
  }  

  /* Responsive */

  @media (max-width: 1024px) {
    body {
      overflow-y: visible;
      overflow-x: hidden
    }

    .attribution {
      text-align: center;
    }

    section {
      display: grid;
      grid-template-columns: 100%;
      grid-template-rows: 25% 75%;

      height: 90%;
      width: 90%;
      
      margin: auto;
    }

    #content {
      grid-area: 2;
      
      text-align: center;
      
      margin: 3rem;
    }
    
    #content h1 {
      font-size: 2.6rem
    }

    #content p {
      font-size: 1.6rem
    }

    #content .stats {
      display: block;
      
      margin-top: 3rem;
    }

    #content .stats h1 {
      margin-bottom: 0rem;
      
      font-size: 2.2rem;
    }

    #content .stats p {
      margin-top: 0.2rem;
      
      font-family: 'Inter', sans-serif;
      font-size: 1.2rem;
    }

    section #image {
      grid-area: 1;
      
      background-image: url(/images/image-header-mobile.jpg);
      background-repeat: no-repeat;
      background-size: cover;
      
      border-radius: 0.5rem 0.5rem 0 0
    }

    section #image::after {
      content: "";
      overflow: hidden;
      
      width: 100%;
      max-height: 100%;
      
      background-color: #5d0788;
      opacity: 0.5;
    } 
  }

  @media (min-width: 2560px) {
  .attribution {
    text-decoration: none;
    text-align: center;
    font-size: 2.6rem;
  }

  .attribution a {
    color: var(--purple);
  }

  #content {
    margin: 7rem 7rem 2rem 7rem;
  }

  /* Texts */ 
  #content h1 {
    font-size: 6rem;
  }
  #content h1 b {
    color: var(--purple);
  }

  #content p {
    font-size: 3rem;
    line-height: 4rem;
    font-family: 'Inter', sans-serif;
    color: var(--transparent-white);
  }
  
  /* Stats */
  #content .stats {
    margin-top: 25rem;
    display: flex;
  }

  #content .stats h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
  }

  #content .stats p {
    font-family: 'Lexend Deca', sans-serif;
    font-size: 2rem;
    margin-top: 0.4rem;
  }
  }

  @media (max-height: 730px) {
    #content .stats {
      display: none;
    }
  }
</style>