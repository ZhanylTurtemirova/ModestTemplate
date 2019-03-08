<template>
  <div class="c-about-wrapper">
    <section class="c-about">
      <h1 class="c-about__title">
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
            <a 
              href="" 
              class="c-about__social-link">
              <img 
                src="" 
                alt="" 
                class="c-about__social-icon">
            </a>
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
.c-about {
  width: 80%;
  margin: 4rem auto;
  &__title {
    color: #292f36;
    font-size: 3.6rem;
    font-weight: 700;
    text-transform: uppercase;
    padding-left: 1rem;
    border-left: 1rem solid #e1e6ea;
    margin: 8rem 0;
  }

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
    margin-bottom: 1rem;
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
