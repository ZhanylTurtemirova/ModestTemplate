<template>
  <footer class="c-footer">
    <div class="c-footer__content">
      <p class="c-footer__copyright">© Copyright 2014 by PSD Booster. All Rights Reserved.</p>
      <ul class="c-footer__social-icons">
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link">
          <i class="fab fa-twitter"/>
        </a>
        </li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"> <i class="fab fa-facebook-f"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><i class="fab fa-skype"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><i class="fab fa-behance"/></a></li>
        <li class="c-footer__social-item "><a 
          href="" 
          class="c-footer__social-link"><i class="fab fa-linkedin-in"/></a></li>
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

  &__social-item {
    list-style: none;
  }

  &__social-icons {
    flex-basis: 20%;
    display: flex;
    justify-content: space-between;
  }

  &__social-link {
    font-size: 1.8rem;
    display: block;
    color: white;
    text-decoration: none;
  }
}
</style>
