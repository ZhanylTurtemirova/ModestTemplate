<template>
  <div class="c-section-wrapper">
    <section class="c-about c-section">
      <h1 class="c-section__title ">
        We are Modest
      </h1>
      <div class="c-about__content">
        <div class="c-about__content-left">
          <p class="c-about__content-paragraph">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed nisi metus, tristique ndolor non, ornare sagittis dolor. Nulla vestibulu lacus sed molestie gravida. Crferm entum  quismagna congue, vel sodales arcu vestibulum. Nunc lobortis dui magna, quis lacusullamcorper at. 
          </p> 
          <p class="c-about__content-paragraph">
            Lorem ipsum dolor sit amet,<strong>consectetur adipiscing elit</strong> . Sed nisi metus, tristique ndolor non, ornare sagittis dolor. Nulla vestibulu lacus sed molestie gravida. Crferm entum  quismagna congue, vel sodales arcu vestibulum. Nunc lobortis dui magna, quis lacusullamcorper at. 
          </p>
          <div class="c-about__social">
            <div class="c-about__social-link-wrapper">
              <a 
                href="" 
                class="c-about__social-link">
                <i class="fab fa-facebook-f"/>
              </a>
            </div>
            <div class="c-about__social-link-wrapper">
              <a 
                href="" 
                class="c-about__social-link">
                <i class="fab fa-twitter"/>
              </a>
            </div>
            <div class="c-about__social-link-wrapper">
              <a 
                href="" 
                class="c-about__social-link">
                <i class="fab fa-google-plus-g"/>
              </a>
            </div>
            <div class="c-about__social-link-wrapper">
              <a 
                href="" 
                class="c-about__social-link">
                <i class="fab fa-dribbble"/>
              </a>
            </div>
            <div class="c-about__social-link-wrapper">
              <a 
                href="" 
                class="c-about__social-link">
                <i class="fab fa-behance"/>
              </a>
            </div>
          </div>
        </div>
        <div class="c-about__content-right c-article">
          <div class="c-article__article">
            <div class="c-article__right">
              <p class="c-article__number">
                01
              </p>
            </div>
            <div class="c-article__left">
              <h2 class="c-article__title">
                Dedication to the customers
              </h2>
              <p class="c-article__text">
                Integer vel lacus non dui ullamcorper venenatis. Aliquam vitae tristique nisi, vitae ullamcorper risus. Nam porttitor blandit ultricies.
              </p>
            </div>
           
          </div>
          <div class="c-article__article">
            <div class="c-article__right">
              <p class="c-article__number">
                02
              </p>
            </div>
            <div class="c-article__left">
              <h2 class="c-article__title">
                Dedication to the customers
              </h2>
              <p class="c-article__text">
                Integer vel lacus non dui ullamcorper venenatis. Aliquam vitae tristique nisi, vitae ullamcorper risus. Nam porttitor blandit ultricies.
              </p>
            </div>
          </div>  
          <div class="c-article__article">
            <div class="c-article__right">
              <p class="c-article__number">
                03
              </p>
            </div>
            <div class="c-article__left">
              <h2 class="c-article__title">
                Dedication to the customers
              </h2>
              <p class="c-article__text">
                Integer vel lacus non dui ullamcorper venenatis. Aliquam vitae tristique nisi, vitae ullamcorper risus. Nam porttitor blandit ultricies.
              </p>
            </div>
          </div>        
        </div>
    </div></section>
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
.c-about {
  width: 80%;

  margin: 4rem auto;

  &__content {
    margin-bottom: 4rem;
    display: flex;
    justify-content: space-between;
  }

  &__content-left,
  &__content-right {
    flex-basis: 45%;
  }

  &__content-paragraph {
    color: #8d8f92;
    font-family: 'Open Sans';
    font-size: 1.6rem;
    font-weight: 400;
    line-height: 2.6rem;
    margin-bottom: 5rem;
  }
  &__social {
    display: flex;
  }
  &__social-link-wrapper {
    background: #c8cdd0;
    width: 4rem;
    height: 4rem;
    margin-right: 0.5rem;
    display: flex;
    justify-content: center;
    align-items: center;

    &:hover {
      background-color: #d0d5d9;
      cursor: pointer;
    }
  }
  &__social-link {
    text-decoration: none;
    font-size: 2rem;
    color: #fff;
    // padding: 2rem;
  }
}
.c-article {
  display: flex;
  flex-direction: column;
  justify-content: space-between;

  &__article {
    display: flex;
    align-items: flex-start;
  }

  &__number {
    font-size: 2rem;
    font-weight: 700;
    padding: 0.5rem;
    color: white;
    background: #23b7a4;
    margin-right: 1rem;
  }

  &__title {
    font-size: 1.6rem;
    font-weight: 700;
    text-transform: uppercase;
    margin-bottom: 1rem;
  }

  &__text {
    color: #8d8f92;
    font-family: 'Open Sans';
    font-size: 1.6rem;
    font-weight: 400;
    line-height: 2.6rem;
    margin-bottom: 1rem;
  }
}
</style>
