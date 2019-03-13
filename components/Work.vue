<template>
  <div class="c-section-wrapper">
    <div class="c-work c-section">
      <h1 class="c-section__title">
        Lovely work.
      </h1>
      <div class="c-work__portfolio">
        <div 
          v-for="(value,index) in 6"  
          v-show="!show"     
          :key="index" 
          class="c-work__portfolio-item">
          <div class="c-work__hover">
            <div class="c-work__hover-bg">
              <i class="fas fa-plus c-work__hover-icon"/>
            </div>
            <p class="c-work__hover-title">
              partnership guidlines
            </p>
          </div>
          <img 
            :src="portfolio[index].imgPath"
            alt="portfolio item"
            class="c-work__portfolio-img">
        </div>
      </div>
      <div 
        v-for="(value,index) in portfolio"
        v-show="show"          
        :key="index" 
        class="c-work__portfolio-item">
        <div class="c-work__hover">
          <div class="c-work__hover-bg">
            <i class="fas fa-plus c-work__hover-icon"/>
          </div>
          <p class="c-work__hover-title">
            partnership guidlines
          </p>
        </div>
        <img 
          :src="portfolio[index].imgPath"
          alt="portfolio item"
          class="c-work__portfolio-img">
      </div>
    </div>
    <div class="c-work__btn-wrapper">
      <button 
        class ="c-work__btn" 
        @click="showMore"> Show me More </button>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.c-section-wrapper {
  width: 100%;
  height: auto;
  padding: 8rem 0;
  background-color: #3a454d;
}
.c-section {
  width: 80%;
  margin: 0 auto;
  &__title {
    color: white;
    font-size: 3.6rem;
    font-weight: 700;
    text-transform: uppercase;
    padding-left: 1rem;
    border-left: 1rem solid #e1e6ea;
    margin: 8rem 0;
  }
}
.c-work {
  &__portfolio {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }

  &__hover {
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    display: flex;
    height: 100%;
  }
  &__hover-bg {
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background-color: #292f36;
    opacity: 0.5;
    color: white;
    font-size: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  &__hover-icon {
    z-index: 1000;
  }

  &__hover-title {
    width: 100%;
    align-self: flex-end;
    font-size: 1.8rem;
    font-weight: 700;
    text-transform: uppercase;
    padding: 1rem;
    background: #000;
    color: white;
  }

  &__portfolio-item {
    position: relative;
    // flex-basis: 30%;
    width: 32%;
    margin-bottom: 2rem;
    background: #4e5a62;

    &:not():nth-of-type(3n) {
      margin-right: 3rem;
    }
  }
  &__portfolio-img {
    width: 100%;
    height: auto;
    object-fit: contain;
  }

  &__btn-wrapper {
    width: 100%;
    text-align: center;
    margin: 6rem 0;
  }

  &__btn {
    margin: 0 auto;
    color: white;
    padding: 1.5rem 2.5rem;
    border: 2px solid #ffffff;
    border-radius: 3px;
    font-size: 1.4rem;
    font-weight: 700;
    text-transform: uppercase;
    background: transparent;
    &:hover {
      cursor: pointer;
    }
  }
}
</style>
<script>
export default {
  data() {
    return {
      // limit: 6,
      show: false,
      portfolio: [
        {
          imgPath: 'images/portfolio-item1.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item2.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item3.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item4.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item5.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item6.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item4.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item5.jpg'
        },
        {
          imgPath: '~assets/images/portfolio-item6.jpg'
        }
      ]
    }
  },
  methods() {
    showMore: {
      this.show = true
      // this.limit = this.portfolio.length
    }
  }
}
</script>
