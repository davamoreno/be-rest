<script setup lang="ts">
import AOS from 'aos';
import 'aos/dist/aos.css';

onMounted(() => {
  AOS.init({
    once: true,
    easing: 'ease-in-out',
  });
});
</script>

<template>
  <section class="hero">
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-xl-8 col-xxxl-7">
                <div class="hero__text" data-aos="fade-up"  data-aos-duration="1000">
                    <h1 style="text-align: center;"><strong>Optimalkan Layanan Jasa Anda Dengan Kami Disini</strong></h1>
                    <p style="text-align: center;">Kami disini sebagai tim profesional yang siap membantu Anda memperbaiki dan meningkatkan pelayanan jasa.</p>
                </div>
                <div class="hero__buttons" data-aos="fade-up"  data-aos-duration="1000">
                    <a href="https://play.google.com/store/apps/details?id=id.berest.app&amp;hl=en&amp;gl=US" class="hero__button-container" target="_blank">
                        <img src="https://berest.id/wp-content/themes/tmdrxberest/img/google-play.png" alt="google play">
                    </a>
                    <a href="https://apps.apple.com/id/app/berest-jasa-freelancer/id6476479122" class="hero__button-container" target="_blank">
                        <img src="https://berest.id/wp-content/themes/tmdrxberest/img/apple-store.png" alt="apple store">
                    </a>
                </div>
            </div>
            <div class="col-xl-10 col-xxl-11">
                <div class="hero__image-container">
                    <img src="https://berest.id/wp-content/uploads/2023/07/hero.png" alt="hero" class="hero__image">
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<style lang="scss" scoped>
    .hero {
        padding: 139px 0 0 0;
        background-color: #F6F6F6;
        &__text h1 {
            position: relative;
            z-index: 2;
            font-size: 58px;
            font-weight: 300;
            margin-bottom: 12px;
        }
        &__text p {
            position: relative;
            z-index: 2;
            font-size: 20px;
            line-height: 1.3;
            color: #6C6C6C;
        }
        &__text::before {
            content: "";
            position: absolute;
            z-index: 0;
            left: 5%;
            top: 100%;
            background-image: url(https://berest.id/wp-content/themes/tmdrxberest/img/ornament/star.svg);
            width: 40px;
            height: 40px;
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
        }
        &__text::after {
            content: "";
            position: absolute;
            z-index: 0;
            left: 110%;
            top: 50%;
            background-image: url(https://berest.id/wp-content/themes/tmdrxberest/img/ornament/teacher.png);
            width: 78px;
            height: 78px;
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
        }
        &__buttons {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
        }
        &__button{
            &-container {
                position: relative;
                width: 100%;
                display: inline-block;
                max-width: 220px;
                &:before {
                    content: "";
                    display: block;
                    padding-top: 29.5454545455%;
                }
                & > * {
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
        &__image{
            max-width: 100%;
            width: 100%;
        }
        &__image-container {
            margin-top: 44px;
        }
    }
</style>