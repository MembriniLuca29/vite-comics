

<template>
<div class="collegamenti">
    <ul class="collegamenti-list">
      <li v-for="link in linkImgArray" :key="link.icon">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <a :href="link.url"
        >{{ link.text }}</a>
      </li>
    </ul>
</div>
<div class="info">
    <div class="info-list">
       <div class="column-info">
        <ul>
            <h2>DC COMICS</h2>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
        </ul>
        <ul>
            <h2>SHOP</h2>
            <li>Shop DC</li>
            <li>Shop DC cCollectibles</li>
        </ul>
       </div>
       <div class="column-info">
        <ul>
            <h2>DC</h2>
            <li>Terms Of Use</li>
            <li>Privacy Policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertsing</li>
            <li>Jobs</li>
            <li>Subscription</li>
            <li>Talent Workshps</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact us</li>
        </ul>
       </div>
       <div class="column-info">
        <ul>
            <h2>SITES</h2>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
        </ul>
       </div>
    </div>
    <div class="flogo">
        <img src="../assets/img/dc-logo-bg.png" alt="">
    </div>
</div>
<div class="sing-in">
    <div class="abutton"><a href=""> SING-UP NOW!</a></div>
    <div class="social">
        <h3>FOLLOW US</h3>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
    </div>
</div>
</template>


<script>
export default {
  data() {
    return {
        linkImgArray: [
        {
          icon: '../assets/img/buy-comics-digital-comics.png',
          text: 'DIGITAL COMICS',
          url: '',
        },
        {
          icon: '../assets/img/buy-comics-merchandise.png',
          text: 'DC MERCHANDISE',
          url: '',
        },
        {
          icon: '../assets/img/buy-comics-subscriptions.png',
          text: 'SUBSCRIPTION',
          url: '',
        },
        {
          icon: '../assets/img/buy-comics-shop-locator.png',
          text: 'COMIC SHOP LOCATOR',
          url: '',
        },
        {
          icon: '../assets/img/buy-dc-power-visa.svg',
          text: 'DC POWER VISA',
          url: '',
        },
        ]
    };
  }
};
</script>

<style>
    .collegamenti{
        width: 100%;
        height: 150px;
        background-color: #0282F9;
        padding: 20px 0;
    }
    .collegamenti-list{
        height: 80%;
        display: flex;
        list-style: none;
        justify-content: center;
        
    }
    .collegamenti-list>li{
        padding: 0 50px;
        font-size: 1rem;
        
    }
    li>img{
        color: white;
        height: 80px;
        position: relative;
        top: 30px;
        right: 10px;
    }
    a{
        text-decoration: none;
        color: white;
    }
    .info{
        width: 100%;
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        height: 450px;
        display: flex;
        
    }
    .info-list{
        width: 30%;
        margin-left: 300px;
        margin-right: 200px;
        color: white;
        display: flex;
    }
    .flogo{
        height: 100%;
        overflow: hidden;
    }
    .flogo>img{
        height: 700px;
        position: relative;
        top: -90px;
        overflow: hidden;
    }
    ul{
        list-style: none;
        padding-top: 10px;
    }
    .column-info>ul>li{
        color: grey;
        padding-top: 5px;
    }
    .sing-in{
        width: 100%;
        height: 120px;
        background-color: #303030;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .abutton{
        margin-left: 300px;
        padding: 10px;
        border: 2px solid #0282F9;
    }
    .social{
        width: 30%;
        display: flex;
        margin-right: 200px;
        justify-content: flex-end;
        align-items: center;
    }
    .social>img{
        height: 40px;
        padding: 0 10px;
    }
    .social>h3{
        color: #0282F9;
        font-size: 1.5rem;
        padding-right: 10px;
    }
</style>