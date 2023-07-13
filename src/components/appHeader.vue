

<template>
<div class="container">
    <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="link">
        <ul class="link-list">
      <li v-for="link in linkArray" :key="link.url">
        <a :href="link.url">{{ link.text }}</a>
      </li>
    </ul>
    </div>
    
</div>
</template>
    
    
<script>
export default {
  data() {
    return {
        linkArray: [
          { text: 'CHARACTERS', url: '' },
          { text: 'COMICS', url: '' },
          { text: 'MOVIES', url: '' },
          { text: 'TV', url: '' },
          { text: 'GAMES', url: '' },
          { text: 'COLLECTIBLES', url: '' },
          { text: 'VIDEOS', url: '' },
          { text: 'FANS', url: '' },
          { text: 'NEWS', url: '' },
          { text: 'SHOP', url: '' },
        ]
    };
  }
};
</script>
    
    <style scoped>
        .container{
            background-color: white;
            width:100%;
            height: 100px;
            display: flex;
        }
        .logo{
            width: 30%;
            display: flex;
            align-items: center;
            margin: 20px 0 20px 300px;
        }
        img{
            height: 80px;
        }

        .link{
            width: 70%;
            display: flex;
            align-items: center;
        }
        .link-list{
            list-style: none;
            display: flex;
            padding-right: 200px;
            margin: 0;
            font-size: 0.9rem;
        }

        li{
            padding: 0 1rem;
        }

        a{
            text-decoration: none;
            color:black;
        }

        a:hover{
            color: #0282F9;
            border-bottom: 5px solid #0282F9;
            padding-bottom: 40px;

        }

    </style>