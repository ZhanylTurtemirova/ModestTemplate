<template>
  <div class="c-section-wrapper">
    <div class="c-team c-section">
      <h1 class="c-section__title">
        Meet the team.
      </h1>

      <div class="c-team__staff">
        <div 
          v-for="person in stuff" 
          :key="person" 
          class="c-team__staff-member" >
          <div 
            class = "c-team__staff-img" 
            @mouseover="mouseOver">
            <div 
              v-if="hover"
              class="c-team__staff-hover"> 
              <div 
                class="c-team__hover-bg" />
              <div class="c-team__staff-links">
                <div class="c-team__link-wrapper">
                  <a 
                    href="" 
                    class="c-team__link">
                    <i class="fab fa-twitter"/>
                  </a>
                </div>
                <div class="c-team__link-wrapper">
                  <a 
                    href="" 
                    class="c-team__link">
                    <i class="fab fa-facebook-f"/>
                  </a>
                </div>
                <div class="c-team__link-wrapper">
                  <a 
                    href="" 
                    class="c-team__link">
                    <i class="fab fa-linkedin-in"/>
                  </a>
                </div>
              </div>  
            </div>
            <img 
              src="~assets/images/pic1.jpg"
              alt="profile photo" 
              class ="c-team__img">
          </div>
          <div class="c-team__staff-info">
            <p class="c-team__staff-name">
              {{ person.name }}
            </p>
            <p class="c-team__staff-position">
              {{ person.position }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
  
</template>
<style lang="scss" scoped>
.c-section {
  &__title {
    color: #292f36;
    font-size: 3.6rem;
    font-weight: 700;
    text-transform: uppercase;
    padding-left: 1rem;
    border-left: 1rem solid #e1e6ea;
    margin: 8rem 0;
  }
}
.c-section-wrapper {
  width: 100%;
  padding-bottom: 8rem;
  border-bottom: 0.3rem solid #dde1e4;
}
.c-team {
  width: 80%;
  margin: 8rem auto;

  &__staff {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  &__staff-member {
    background: #e1e6ea;
    &:hover {
      background: #3a454d;
      & .c-team__staff-name {
        color: white;
      }
      & .c-team__staff-position {
        color: white;
      }
    }
  }

  &__img {
    width: 100%;
    height: 100%;
  }

  &__staff-name {
    font-size: 1.6rem;
    font-weight: 700;
    color: #292f36;
    text-transform: uppercase;
    padding: 2rem;
    padding-bottom: 0.9rem;
  }

  &__staff-position {
    font-family: 'Open Sans';
    font-size: 1.4rem;
    font-weight: 400;
    padding-left: 1.9rem;
    padding-bottom: 2rem;
    color: #8d8f92;
  }
  &__staff-img {
    position: relative;
  }

  &__staff-hover {
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
  }

  &__hover-bg {
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 0;
    background-color: #ffffff;
    opacity: 0.4;
  }

  &__staff-links {
    display: flex;
    justify-content: center;
    height: 100%;
    align-items: center;
  }

  &__link-wrapper {
    background: #3a454d;
    width: 5rem;
    height: 5rem;
    margin-right: 0.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;

    &:hover {
      background: #4e5a62;
      cursor: pointer;
    }
  }
  &__link {
    text-decoration: none;
    font-size: 2.8rem;
    color: white;
  }
  &__staff-hover {
    opacity: 0;
    &:hover {
      opacity: 1;
    }
  }
}
</style>

<script>
export default {
  data() {
    return {
      hover: false,
      stuff: {
        person1: {
          name: 'Gloria Bromley',
          position: 'CEO and Founder',
          imgPath: '/_nuxt/assets/images/pic1.jpg'
        },
        person2: {
          name: 'Paul Torres',
          position: ' Head of Development',
          imgPath: '~assets/images/pic2.jpg'
        },
        person3: {
          name: 'Judith Gillette',
          position: 'Graphic Desinger',
          imgPath: 'assets/images/pic3.jpg'
        },
        person4: {
          name: 'Delores Reed',
          position: 'Client Service Director',
          imgPath: 'assets/images/pic4.jpg'
        }
      }
    }
  },
  methods: {
    mouseOver: {
      function() {
        this.hover == true
      }
    }
  }
}
</script>
