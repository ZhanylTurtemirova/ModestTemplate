<template>
  <div class="c-section-wrapper">
    <div class="c-services c-section">
      <h1 class="c-section__title">
        What we do.
      </h1>
      <div class="c-services__items">
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/cogs.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            Easy theme Setup
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/pencil.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            pixel perfect design
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/mobile.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            responsive display
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/clock.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            24/7 support
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
      </div>  
      <div class="c-services__items">
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/cogs.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            Easy theme Setup
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/pencil.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            pixel perfect design
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/mobile.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            responsive display
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
        <div class="c-services__item">
          <div class="c-services__icon">
            <img 
              src="~assets/images/clock.svg" 
              alt="service icon">
          </div>
          <h2 class="c-services__title">
            24/7 support
          </h2>
          <p class="c-services__description">
            Nunc mattis lorem in leo lobortis, ut venenatis justo commodo. Maecenas a justo nec velit egestas fermentum.
          </p>
        </div>
      </div>        
    </div>
    
  </div>
</template>

<style lang="scss" scoped>
.c-section-wrapper {
  width: 100%;
  height: auto;
  padding: 8rem 0;
}
.c-section {
  width: 80%;
  margin: 0 auto;
  &__title {
    font-size: 3.6rem;
    font-weight: 700;
    text-transform: uppercase;
    padding-left: 1rem;
    border-left: 1rem solid #e1e6ea;
    margin: 8rem 0;
  }
}
.c-services {
  &__items {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 7rem;
  }
  &__item {
    width: 22%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
  }

  &__title {
    color: #292f36;
    font-size: 1.7rem;
    font-weight: 700;
    text-transform: uppercase;
    margin: 3rem 0;
  }
  &__description {
    color: #8d8f92;
    font-family: 'Open Sans';
    font-size: 1.6rem;
    font-weight: 400;
    line-height: 2.6rem;
    text-align: center;
  }
}
</style>
