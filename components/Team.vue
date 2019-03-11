<template>
  <div class="c-section-wrapper">
    <div class="c-team c-section">
      <h1 class="c-section__title">
        Meet the team.
      </h1>
      <div class="c-team__staff">
        <div class="c-team__staff-member">
          <div class = "c-team__staff-img">
            <div class="c-team__staff-hover"> 
              <div class="c-team__hover-bg"/>
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
              src="~/assets/images/pic1.jpg"  
              alt="profile photo" 
              class ="c-team__img">
          </div>
          <div class="c-team__staff-info">
            <p class="c-team__staff-name">
              Gloria Bromley
            </p>
            <p class="c-team__staff-position">
              CEO and Founder
            </p>
          </div>
        </div>
        <div class="c-team__staff-member">
          <div class = "c-team__staff-img">
            <img 
              src="~/assets/images/pic2.jpg"  
              alt="profile photo" 
              class ="c-team__img">
          </div>
          <div class="c-team__staff-info">
            <p class="c-team__staff-name">
              Paul Torres
            </p>
            <p class="c-team__staff-position">
              Head of Development
            </p>
          </div>
        </div>
        <div class="c-team__staff-member">
          <div class = "c-team__staff-img">
            <img 
              src="~/assets/images/pic3.jpg"  
              alt="profile photo" 
              class ="c-team__img">
          </div>
          <div class="c-team__staff-info">
            <p class="c-team__staff-name">
              Judith Gillette
            </p>
            <p class="c-team__staff-position">
              Graphic Desinger
            </p>
          </div>
        </div>
        <div class="c-team__staff-member">
          <div class = "c-team__staff-img">
            <img 
              src="~/assets/images/pic4.jpg"  
              alt="profile photo" 
              class ="c-team__img">
          </div>
          <div class="c-team__staff-info">
            <p class="c-team__staff-name">
              Delores Reed
            </p>
            <p class="c-team__staff-position">
              Client Service Director
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
      & .c-team__hover-bg {
        height: 30rem;
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
    max-height: 0;
    background-color: #ffffff;
    opacity: 0.4;
    transition: height 2s;
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
}
</style>
