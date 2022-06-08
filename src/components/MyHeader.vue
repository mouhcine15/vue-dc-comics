<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div id="menu">
            <ul>
                <li v-for="(link, i) in links" :key="i">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data(){
      return {
          links: [
             {
                 text: "CHARACTERS",
                 url: "#"
             }, 
             {
                 text: "COMICS",
                 url: "#"
             }, 
             {
                 text: "MOVIES",
                 url: "#"
             },
             {
                 text: "TV",
                 url: "#"
             }, 
             {
                 text: "GAMES",
                 url: "#"
             },
             {
                 text: "COLLECTIBLES",
                 url: "#"
             }, 
             {
                 text: "VIDEO",
                 url: "#"
             },
             {
                 text: "FANS",
                 url: "#"
             }, 
             {
                 text: "NEWS",
                 url: "#"
             },
             {
                 text: "SHOP",
                 url: "#"
             }
          ]
      }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: white;
    }
    li {
        display: inline;
        padding: 10px;
    }
    a:hover {
        color: blue;
        border-bottom: solid blue 2px;
    }

    a {
        color: black;
        text-decoration: none;
    }

</style>