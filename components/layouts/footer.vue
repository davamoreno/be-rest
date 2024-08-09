<template>
<footer class="footer">
    <div class="footer__top">
        <div class="container">
            <div class="row gy-4 gy-lg-0">
                <div class="col-lg-3">
                    <a href="https://berest.id/" class="footer__logo-container">
                        <img src="https://berest.id/wp-content/uploads/2023/07/logo-full.svg" alt="logo">
                    </a>
                    <div class="footer__info">
                        <h2>
                            <strong>Kasih solusi, terima Berest!</strong>
                        </h2>
                        <p>Blok A No. 18 STA Niaga Sentul City Bogor 16810</p>
                    </div>
                </div>
                <div class="col-lg-3 col-xxl-2 offset-lg-2 offset-xxl-3">
                    <h2 class="footer__heading">Layanan Kami</h2>
                    <div>
                        <a href="https://berest.id/layanan-kami/?rumah" class="footer__subheading">Layanan Rumah</a>
                    </div>
                    <div>
                        <a href="https://berest.id/layanan-kami/?pengajar" class="footer__subheading">Layanan Pengajar</a>
                    </div>
                </div>
                <div class="col-lg-2">
                    <h2 class="footer__heading">Bantuan</h2>
                    <div>
                        <a href="mailto:info@berest.id" class="footer__subheading" target="_blank">CS Email</a>
                    </div>
                    <div>
                        <a href="https://wa.me/6285215053547" class="footer__subheading" target="_blank">CS Whatsapp</a>
                    </div>
                </div>
                <div class="col-lg-2">
                    <h2 class="footer__heading">Social Media</h2>
                    <div class="footer__social">
                        <a href="https://www.instagram.com/berest.id/" target="_blank" class="footer__social-container">
                        <img src="https://berest.id/wp-content/uploads/2023/07/instagram.svg" alt="icon">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="footer__bottom">
        <div class="container">
            <h2 class="footer__copyright">© Copyright 2024 Berest. All rights reserved.</h2>
            <h2 class="footer__terms-privacy">
                <a href="https://berest.id/terms-and-conditions/">Terms and Conditions</a> • 
                <a href="https://berest.id/privacy-policy/">Privacy Policy</a>
            </h2>
        </div>
    </div>
</footer>
</template>

<style lang="scss" scoped>
p {
    margin-top: 0;
    margin-bottom: 1rem;
}
    .footer__top{
        padding: 80px 0;
        background-color: #f6f6f6;
    }
    .footer__logo-container{
        position: relative;
        width: 100%;
        display: inline-block;
        max-width: 144px;
        margin-bottom: 8px;
    }
    .footer__info{
        h2{
            font-size: 18px;
            line-height: 1.5;
            color: #000;
            margin-bottom: 16px;
        }
        p{
            font-size: 18px;
            line-height: 1.3;
            color: #6c6c6c;
        }
    }
    .footer__heading {
    font-size: 20px;
    line-height: 1.3;
    font-weight: 600;
    color: #000;
    margin-bottom: 16px;
    }

    .footer__subheading {
    font-size: 18px;
    line-height: 1.3;
    display: inline-block;
    color: #6c6c6c;
    margin-bottom: 16px;
    text-decoration: none;
    transition: color .3s ease;
    }

    .footer__social {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    }

    .footer__bottom {
    background-color: #2c89ce;
    padding: 20px 0;
    text-align: center;
    }

    .footer__copyright {
    font-size: 16px;
    color: #fff;
    font-weight: 400;
    margin-bottom: 6px;
    }
    .footer__terms-privacy {
        font-size: 14px;
        margin: 0;
        font-weight: 400;
        color: #fff;
        a{
            text-decoration: none;
            color: rgba(255, 255, 255, .6);
            transition: color .3s ease;
        }
    }
</style>