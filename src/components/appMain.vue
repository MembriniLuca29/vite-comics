<script >
import product from './product.vue';

export default {
    name:"maincomponent",
  data() {
    return{
            products:[
  {
      "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book",
  },
  {
      "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book",
  },
  {
      "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel",
  },
  {
      "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book",
  },
  {
      "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel",
  },
]
        };
  },
  components:{
    product
  }
}

</script>

<template>

        <div class="jumbotron"></div>
        <div class="resolution">
        <div class="product-container">
            <h4>CURRENT SERIES </h4>
            <product
            v-for="(product, productIndex) in products" :key="productIndex"
            :productImage="product.thumb"
            :productTitle="product.series"/>
            </div>
            <div class="loadbutton"><a href="">LOAD MORE</a></div>
            </div>
</template>

<style scoped lang="scss">
    h4{
        color: white;
        margin-left: 200px;
        font-size: 2rem;
        background-color: #0282F9;
        padding: 10px;
        display: inline;
        position: absolute;
        top: -80px;
        left: 30px;
    }
    .resolution{
        width: 100%;
        background-color: #1C1C1C;
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-bottom: 70px;
    }
    .jumbotron{
        background-image: url(../assets/img/jumbotron.jpg);
        width: 100%;
        height: 400px;
        background-size: cover;
    }
   
    .product-container{
    background-color: #1C1C1C;
    width: 70%;
    height: 600px;
    display: flex;
    flex-wrap: wrap;
    position: relative;
    padding-top: 60px;
    padding-bottom: 90px;
}
a{
    color: white;
    
    text-decoration: none;
}
.loadbutton{
    background-color: #0282F9;
    padding: 10px 30px;
}
</style>