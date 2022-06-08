<template>
    <footer>

    </footer>
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
    
</style>