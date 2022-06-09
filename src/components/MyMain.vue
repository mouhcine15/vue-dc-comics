<template>
    <main>
      <div id="jumbo">

      </div>
      <div id="container">
        <div id="primocontainer">
          <div id="primaparte">
            <div id="current">
              CURRENT SERIES
            </div>
            <ul>
               <li v-for="(link, i) in prodotti" :key="i">
                  <a :href="link.url">
                    <img :src="link.thumb" alt="">
                    <div>
                      {{link.series}}
                    </div>
                  </a>
               </li>
             </ul>
             <div id="more">
                LOAD MORE
             </div>
          </div>
        </div>
        <div id="secondocontainer">
          <div id="secondaparte">
             <ul>
               <li v-for="(link, i) in links" :key="i">
                  <a :href="link.url">
                    <img :src="link.img" alt="">
                    <div id="text">
                      {{link.text}}
                    </div>
                  </a>
               </li>
             </ul>
          </div>
        </div>
      </div>
    </main>
</template>

<script>
export default {
  name: 'MyMain',
  data(){
      return {
          links: [
             {
                 text: "DIGITALS",
                 url: "#",
                 img: require("../assets/img/buy-comics-digital-comics.png")
             }, 
             {
                 text: "DC MERCHANDISE",
                 url: "#",
                 img: require("../assets/img/buy-comics-merchandise.png")
             }, 
             {
                 text: "SUBSCRIPTION",
                 url: "#",
                 img: require("../assets/img/buy-comics-subscriptions.png")
             },
             {
                 text: "COMIC SHOP LOCATOR",
                 url: "#",
                 img: require("../assets/img/buy-comics-shop-locator.png")
             }, 
             {
                 text: "DC POWER VISA",
                 url: "#",
                 img: require("../assets/img/buy-dc-power-visa.svg")
             }
          ]
      }
  },
  props: {
    prodotti: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    #jumbo {
      background-image: url("../assets/img/jumbotron.jpg");
      height: 450px;
    }
    #container {
      background-color: black;
    }
    #primaparte {
      color: white;
      font-size: 20px;
      width: 80%;
      margin: auto;
      display: flex;
      flex-direction: column;
      align-items: center;

      #current {
        background-color: blue;
        width: fit-content;
        padding: 10px;
      }

      ul {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        
        li {
          display: inline-block;
          padding: 15px;

          a {
          color: white;
          display: flex;
          flex-direction: column;
          align-items: flex-start;

          img {
            width: 100%;
            height: 100%;
          }
          div {
            width: 110px;
            display: flex;
            flex-wrap: wrap;
          }
          }
        }
      }
      #more {
        background-color: blue;
        width: fit-content;
        padding: 10px;
        margin: 20px;
      }
    }

    #secondocontainer {
      background-color: blue;

    }
    #secondaparte {
      display: flex;
      justify-content: center;
      padding: 40px 0;
     
      li {
          display: inline-block;
          padding: 10px;
      }
      a {
          color: white;
          text-decoration: none;
          display: flex;
          align-items: center;
      }
    }

    #secondaparte ul li a div {
      padding: 0 10px;
    }

    img {
        width: 50px;
        height: 60px;
    }
</style>