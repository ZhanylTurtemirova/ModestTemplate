<template>
  <header class="c-header">
    <div class="c-header__items c-menu">
      <div class="c-menu__logo">
        <nuxt-link 
          :to="{name: 'index'}" 
          class="c-logo">
          <img 
            class="c-logo-img" 
            src="~/assets/images/modest.svg" 
            alt="logo">
        </nuxt-link>
      </div>
      <nav class="c-menu__nav">   
        <li class="c-menu__item"> 
          <nuxt-link 
            to="/#" 
            class="c-menu__link c-menu__link--active">
            Home
          </nuxt-link>      
        </li><li class="c-menu__item">
          <nuxt-link 
            to="/#about" 
            class="c-menu__link">
            About
          </nuxt-link>
        </li>
        <li class="c-menu__item"> 
          <nuxt-link 
            to="/#team" 
            class="c-menu__link">
            Team
          </nuxt-link>
        </li>
        <li class="c-menu__item"> 
          <nuxt-link 
            to="#work" 
            class="c-menu__link">
            Work
          </nuxt-link>
        </li>
        <li class="c-menu__item"> 
          <nuxt-link 
            to="#services" 
            class="c-menu__link">
            Services
          </nuxt-link>
        </li>
        <li class="c-menu__item"> 
          <nuxt-link 
            to="#futures" 
            class="c-menu__link">
            Futures
          </nuxt-link>
        </li>
        <li class="c-menu__item"> 
          <nuxt-link 
            to="#contact" 
            class="c-menu__link">
            Contact
          </nuxt-link>
        </li>
      </nav>
    </div>
  </header>  
</template>

<style lang="scss">
//color variables
$black: #1d2126;
$white: #ffffff;
$dark-grey: #3a454d;
$green-blue: #23b7a4;
$grey: #d0d5d9;
$medium-grey: #4e5a62;

.c-header {
  z-index: 10000;
  position: fixed;
  width: 100%;
  margin: 0;
  padding: 3rem 0;
  background-color: $black;
}

.c-menu {
  width: 80%;
  // max-width: 96rem;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  color: $white;
  font-size: 1.4rem;

  &__nav {
    display: flex;
    justify-content: flex-end;
  }

  &__item {
    list-style: none;
  }

  &__link {
    color: $white;
    text-decoration: none;
    text-transform: uppercase;
    padding: 0.7rem 1rem;

    &--active {
      color: $green-blue;
      border: 2px solid $green-blue;
    }

    &:hover {
      color: $grey;
      border: 2px solid $grey;
      padding: 0.7rem 1rem;
    }
  }
}
</style>
