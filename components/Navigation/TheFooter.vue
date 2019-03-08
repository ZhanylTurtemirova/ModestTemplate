<template>
  <footer class="c-footer">
    <div class="c-footer__content">
      <p class="c-footer__copyright">© Copyright 2014 by PSD Booster. All Rights Reserved.</p>
      <ul class="c-footer__social-icons">
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link">
          <div class="c-footer__social-icon c-footer__social-icon--tw"/> 
        </a>
        </li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><div class="c-footer__social-icon c-footer__social-icon--fb"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><div class="c-footer__social-icon c-footer__social-icon--skype"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><div class="c-footer__social-icon c-footer__social-icon--be"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><div class="c-footer__social-icon c-footer__social-icon--in"/></a></li>
      </ul>
    </div>
  </footer>
</template>

<style lang="scss">
//color variables
$black: #1d2126;
$white: #ffffff;
$dark-grey: #3a454d;
$green-blue: #23b7a4;
$grey: #d0d5d9;
$medium-grey: #4e5a62;

.c-footer {
  z-index: 10000;
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  justify-content: center;
  padding: 3rem 0;
  background-color: $black;

  &__content {
    width: 80%;
    // max-width: 96rem;
    display: flex;
    justify-content: space-between;
    color: white;
    font-size: 1.4rem;
  }

  &__social-icons {
    position: relative;
  }

  &__social-item {
    margin: 0;
    padding: 0;
    list-style: none;
    position: absolute;
    top: 0;

    // &--tw {
    //   background-image: url('~assets/images/icons.svg') 0 0;
    //   left: 0;
    //   width: 1.8rem;
    // }

    // &--fb {
    //   background-image: url('~assets/images/icons.svg') -1.9rem 0;
    //   left: 1.8rem;
    //   width: 1.8rem;
    // }

    // &--skype {
    //   background-image: url('~assets/images/icons.svg') -3.8rem 0;
    //   left: 3.6rem;
    //   width: 1.8rem;
    // }

    // &--be {
    //   background-image: url('~assets/images/icons.svg') -5.7rem 0;
    //   left: 5.4rem;
    //   width: 1.8rem;
    // }

    &--in {
      background-image: url('~assets/images/icons.svg');
      left: 7.2rem;
      width: 1.8rem;
    }
  }

  &__social-link {
    height: 1.8rem;
    display: block;
  }
}
</style>
