<template>
  <div class="c-banner">
    <div class="c-banner__bg">   
      
    </div>
    <div class="c-banner__info">
      <h1 class="c-banner__title">Welcome to our marketplace</h1>
      <p class="c-banner__text h-text-ellipsis"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed nisi metus, tristique ndolor non, ornare sagittis dolor. Nulla vestibulu lacus sed molestie gravida. Crferm entum  quismagna congue, vel sodales arcu vestibulum. Nunc lobortis dui magna, quis lacusullamcorper at. 
Phasellus sollicitudin ante eros ornare, sit amet luctus lorem semper. Suspendisse posuere, quamdictum consectetur, augue metus pharetra tellus, eu feugiatloreg egetnisi. Cras ornare bibendum ante, ut bibendum odio convallis eget. vel sodales arcu vestibulum</p>
      <div class="c-baner__bottoms">
        <nuxt-link 
          to="/#about" 
          class="c-banner__link">
          View More
        </nuxt-link>
        <nuxt-link 
          to="/#about" 
          class="c-banner__link">
          Video Tour
        </nuxt-link>
      </div>
    </div>
    <div class="c-banner__pagination">
      <span class="c-banner__pagination-dot"> </span>
      <span class="c-banner__pagination-dot"></span>
      <span class="c-banner__pagination-dot"></span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .c-banner {
    width: 100%;
    height: 100vh;
    margin: 0;
    padding-top: 10rem;
    background-color: #3a454d;
    color:white;
    display: flex;
    align-items: center;
    justify-content: center;

    &__bg {
      padding: absolute;
      top: 0;
      left: 0;
      background-image: url('/assets/image/banner-1.png');
    }

    &__info { 
     width: 75%;  
     display: flex;
     flex-direction: column;
     justify-content: space-between;

    }

    &__title {      
      text-transform: uppercase;
      font-size: 3.6rem;
      font-weight: 700;
      margin-bottom: 3.1rem;
    }

    &__text {
      width: 60%;
      font-size: 1.6rem;
      margin-bottom: 4.3rem;
    }

    &__link {
      margin-right:1.5rem ;
      text-decoration: none;
      color: white;
      text-transform: uppercase;
      font-size: 1.4rem;
      padding: 1.5rem 2rem;
      border: 2px solid white;
      border-radius: 0.3rem;
      
      &:hover {
        color:#23b7a4;
        border-color: #23b7a4;
      }
    }

    &__pagination {
      width:5.2rem;
      display: flex;
      justify-content: space-between;
      align-self: flex-end;
      margin-bottom: 15rem;
    }

    &__pagination-dot {
      border:2px solid white;    
      height:0.9rem;
      width: 0.9rem;
      border-radius:50%;

      &:hover {
        background:#23b7a4;
        border-color: #23b7a4;
      }
    }
  }
</style>

