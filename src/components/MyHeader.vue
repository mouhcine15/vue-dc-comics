<template>
    <header>
        <div id="container">
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
        background-color: white;
    }

    #container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 80%;
        margin: auto;
    }
    li {
        display: inline;
        padding: 10px;
    }
    a:hover {
        color: blue;
        border-bottom: solid blue 5px;
    }

    a {
        color: black;
        text-decoration: none;
        padding: 40px 0;
    }

</style>