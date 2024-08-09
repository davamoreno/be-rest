<script lang="ts" setup>
 import { onMounted } from 'vue';

  onMounted(() => {
    const navbar = document.querySelector('.custom-navbar') as HTMLElement;

    if (navbar) {
      window.addEventListener('scroll', () => {
        if (window.scrollY > 210) {
          navbar.classList.add('scrolled');
        } else {
          navbar.classList.remove('scrolled');
        }
      });
    } else {
      console.error("Navbar element not found")
    }
  });
</script> 

<template>
  <nav class="navbar navbar-expand-lg fixed-top custom-navbar">
    <div class="container-xl">
      <div class="custom-navbar__logo-wrapper">
        <a href="https://berest.id/" class="custom-navbar__logo-container" rel="home" aria-current="page">
          <img width="153" height="43" src="https://berest.id/wp-content/uploads/2023/07/logo-full.svg" class="custom-logo" alt="BeRest" decoding="async">
        </a>
      </div>
      <button class="navbar-toggler custom-navbar__toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="custom-navbar__toggler-icon top"></span>
        <span class="custom-navbar__toggler-icon middle"></span>
        <span class="custom-navbar__toggler-icon bottom"></span>
      </button>
      <div class="collapse navbar-collapse custom-navbar__navbar-collapse" id="navbarNav">
        <ul class="navbar-nav custom-navbar__navbar-nav">
          <li id="menu-item-31" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-home current-menu-item page_item page-item-11 current_page_item menu-item-31">
            <a href="https://berest.id/" aria-current="page" class="menu-link">Beranda</a>
          </li>
          <li id="menu-item-34" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-34">
            <a href="https://berest.id/tentang-kami/" class="menu-link">Tentang Kami</a>
          </li>
          <li id="menu-item-33" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-33">
            <a href="https://berest.id/layanan-kami/" class="menu-link">Layanan Kami</a>
          </li>
          <li id="menu-item-32" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-32">
            <a href="https://berest.id/bantuan/" class="menu-link">Bantuan</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
  @media (min-width: 992px) {
    .navbar-expand-lg .navbar-toggler {
        display: none;  
      }
    }
    
  .custom-navbar {
    background-color: #f6f6f6;
    padding: 32px 0;
    transition: background 0.3s ease, padding 0.3s ease;

    @media (max-width: 991px) {
      &{
        padding: 11px 0;
      }
      &__navbar-nav {
          padding: 10px 0;
      }
    }

    &.scrolled {
      background-color: #fff;
      padding: 11px 0;
    }
    &.scrolled &__logo-container {
      position: relative;
      width: 100%;
      display: inline-block;
      max-width: 120px;
      &::before{
        content: "";
        display: block;
        padding-top: 27.5%;
        @media (max-width: 991px) {
          content: "";
          display: block;
          padding-top: 27.5%;
        }
      }
      & > *{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        -o-object-fit: contain;
        object-fit: contain;
      }
    }

    &__logo-wrapper{
      flex: 0 1 175px;
    }
    &__logo-container{
      transition: 0.3s;
      position: relative;
      width: 100%;
      display: inline-block;
      max-width: 153px;
      @media(max-width: 991px) {
        &{
          position: relative;
          width: 100%;
          display: inline-block;
          max-width: 120px;
        &:before {
          content: "";
          display: block;
          padding-top: 27.5%;
          }
          & > *{
          position: absolute;
          top: 0;
          left: 0;
          width: 100%;
          height: 100%;
          -o-object-fit: contain;
          object-fit: contain;
          }
        }
      }
    }
    &__toggler{
      position: relative;
      width: 24px;
      height: 24px;
      display: flex;
      justify-content: center;
      align-items: center;
      border: 0;
      @media (max-width:991px) {
        margin: 5px;
      }
      &:hover &-icon{
        background-color: #2c89ce;
        text-decoration: none;
      }
      &:focus &-icon{
        outline: 0;
        box-shadow: none;
      }
      &-icon{
        display: block;
        position: absolute;
        left: 0;
        height: 2px;
        width: 100%;
        background-color: #000;
        border-radius: 1px;
        opacity: 1;
        transform: rotate(0deg);
        transition: 0.3s ease-in-out;
        &.top{
            margin-top: -15px;
            transform: rotate(0);
          }
        &.middle{
            margin-top: 0;
            opacity: 1;
          }
        &.bottom{
          margin-top: 15px;
          transform: rotate(0);
        }
      }
    }
    &__navbar-collapse{
      justify-content: center;
    }
    & .menu-item{
      margin: 0 16px;
      @media (max-width:991px){
        margin: 10px 0;
      }
      @media screen and (max-width: 1399px) {
        &.menu-item a {
          font-size: 18px;
        }
      }
      &.current-menu-item a {
        color: #2c89ce;
        opacity: 1;
        }
      a{
        color: #1b1b1b;
        font-size: 20px;
        line-height: 1.3;
        font-weight: 500;
        text-decoration: none;
        transition: color .3s ease;
        padding: 4px;
      }
      a:hover{
        color: #2c89ce;
      }
    }
  }
</style>