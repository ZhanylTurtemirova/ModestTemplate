<template>
  <div class="c-banner">
    <div class="c-banner__slider">
      <transition name="fade">
        <img 
          v-if="curSlide=='first'"
          class="c-banner__img" 
          src="~/assets/images/banner_1.png" 
          alt="bg-1">
        <img 
          v-if="curSlide=='second'"
          class="c-banner__img" 
          src="~/assets/images/banner_2.jpg" 
          alt="bg-1">
        <img 
          v-if="curSlide=='third'"
          class="c-banner__img" 
          src="~/assets/images/banner_3.jpg" 
          alt="bg-1">
      </transition>  
    </div>
    
    <div class="c-banner__info">
      <h1 class="c-banner__title">Welcome to our marketplace</h1>
      <p class="c-banner__text h-text-ellipsis"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed nisi metus, tristique<br> ndolor non, ornare sagittis dolor. Nulla vestibulu lacus sed molestie gravida. Crferm entum  quismagna congue, vel sodales arcu vestibulum. Nunc lobortis dui magna, quis lacusullamcorper at. 
      Phasellus sollicitudin ante eros ornare, sit amet luctus lorem semper. Suspendisse posuere, quamdictum consectetur, augue metus pharetra tellus, eu feugiatloreg egetnisi. Cras ornare bibendum ante, ut bibendum odio convallis eget. vel sodales arcu vestibulum</p>
      <div class="c-baner__bottoms">
        <nuxt-link 
          to="/#about"
          class="c-banner__link" 
          @click="showMore">
          View More
        </nuxt-link>
        <nuxt-link 
          to="/#about"
          class="c-banner__link" 
          @click="showVideo">
          Video Tour
        </nuxt-link>
      </div>
    </div>
    <div class="c-banner__pagination">
      <span 
        :class="{'c-banner__pagination-dot--active' : curSlide==='first'}" 
        class="c-banner__pagination-dot"
        @click.prevent = "currentSlide('first')"/>
      <span 
        :class="{'c-banner__pagination-dot--active' : curSlide==='second'}" 
        class="c-banner__pagination-dot" 
        @click.prevent= "currentSlide('second')"/>
      <span 
        :class="{'c-banner__pagination-dot--active' : curSlide==='third'}" 
        class="c-banner__pagination-dot" 
        @click.prevent= "currentSlide('third')"/>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.c-banner {
  z-index: 100;
  width: 100%;
  margin: 0;
  background-color: #3a454d;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: auto;
  height: 100vh;

  &__slider {
    position: absolute;
    margin: auto;
    max-height: 66rem;
    width: 100%;
  }

  &__img {
    object-fit: contain;
    width: 100%;
    height: 100vh;
    animation-name: fade;
    animation-duration: 1.5s;
    // background-image: url('~/assets/images/banner_1.png');
  }

  &__info {
    z-index: 1000;
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
    line-height: 2.6rem;
    font-family: 'Open Sans';
  }

  &__link {
    margin-right: 1.5rem;
    text-decoration: none;
    color: white;
    text-transform: uppercase;
    font-size: 1.4rem;
    padding: 1.5rem 2rem;
    border: 2px solid white;
    border-radius: 0.3rem;

    &:hover {
      border-color: #23b7a4;
      background-color: #23b7a4;
    }
  }

  &__pagination {
    z-index: 1000;
    width: 5.2rem;
    display: flex;
    justify-content: space-between;
    align-self: flex-end;
    margin-bottom: 15rem;
  }

  &__pagination-dot {
    border: 2px solid white;
    height: 0.9rem;
    width: 0.9rem;
    border-radius: 50%;

    &:hover {
      background: #23b7a4;
      border-color: #23b7a4;
    }

    &--active {
      background: #23b7a4;
      border-color: #23b7a4;
    }
  }
}

.slide-fade-enter-active {
  transition: all 0.3s ease;
}
.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-enter,
.slide-fade-leave-to {
  opacity: 0;
}

.h-text-ellipsis {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

@keyframes fade {
  from {
    opacity: 0.4;
  }
  to {
    opacity: 1;
  }
}
</style>

<script>
export default {
  data() {
    return {
      curSlide: 'first'
    }
  },
  methods: {
    currentSlide(slide) {
      console.log('slide')
      this.curSlide = slide
    },
    showMore() {
      console.log('show more')
    },
    showVideo() {
      console.log('show video')
    }
  }
}
</script>
