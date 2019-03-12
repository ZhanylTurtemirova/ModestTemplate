<template>
  <div class="c-section-wrapper">
    <div class="c-work c-section">
      <h1 class="c-section__title">
        Lovely work
      </h1>
      <div class="c-work__portfolio">
        <div 
          v-for="item in portfolio" 
          :key="item" 
          class="c-work__portfolio-item">
          <img 
            
            src="~assets/images/portfolio_item 3.jpg"
            alt="portfolio item">
        </div>
      </div>
      <div class="c-work__btn-wrapper">
        <button 
          class ="c-work__btn" 
          @click="showMore"> Show me More </button>
      </div>
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
  &__portfolio-item {
    // flex-basis: 30%;
    width: 30%;
    margin-bottom: 2rem;
    background: #4e5a62;

    &:not():nth-of-type(3n) {
      margin-right: 3rem;
    }
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
  }
}
</style>
<script>
export default {
  data() {
    return {
      portfolio: {
        item1: {
          imgPath: '~assets/images/portfolio-item1.jpg'
        },
        item2: {
          imgPath: '~assets/images/portfolio-item2.jpg'
        },
        item3: {
          imgPath: '~assets/images/portfolio-item3.jpg'
        },
        item4: {
          imgPath: '~assets/images/portfolio-item4.jpg'
        },
        item5: {
          imgPath: '~assets/images/portfolio-item5.jpg'
        },
        item6: {
          imgPath: '~assets/images/portfolio-item6.jpg'
        }
      }
    }
  }
}
</script>
