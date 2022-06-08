<template>
    <main>
      <div id="primocontainer">
        <div id="primaparte">
          Content goes here
        </div>
      </div>
      <div id="secondocontainer">
        <div id="secondaparte">
           <ul>
             <li v-for="(link, i) in links" :key="i">
                <a :href="link.url">
                  <div>
                    <img :src="link.img" alt="">
                  </div>
                  <div>
                    {{link.text}}
                  </div>
                </a>
             </li>
           </ul>
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
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    #primocontainer {
      background-color: black;
    }
    #primaparte {
      color: white;
      font-size: 20px;
      width: 80%;
      margin: auto;
    }

    #secondocontainer {
      background-color: blue;

    }
    #secondaparte {
      display: flex;
      justify-content: center;
    }

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

    img {
        width: 50px;
        height: 60px;
    }
</style>