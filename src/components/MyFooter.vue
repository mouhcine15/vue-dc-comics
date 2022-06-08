<template>
    <footer>
        <div id="container">
            <div id="primaparte">
                <div>
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="(link1, i) in dccomics" :key="i">
                                <a :href="link1.url">{{link1.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="(link2, i) in shop" :key="i">
                                <a :href="link2.url">{{link2.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                         <li v-for="(link3, i) in DC" :key="i">
                            <a :href="link3.url">{{link3.text}}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3>SITIES</h3>
                    <ul>
                        <li v-for="(link4, i) in sities" :key="i">
                            <a :href="link4.url">{{link4.text}}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div id="secondaparte">
    
            </div>
        </div>

    </footer>
</template>

<script>
export default {
  name: 'MyFooter',
  data(){
      return {
          dccomics: [
             {
                 text: "Characters",
                 url: "#"
             }, 
             {
                 text: "Comics",
                 url: "#"
             }, 
             {
                 text: "Movies",
                 url: "#"
             },
             {
                 text: "TV",
                 url: "#"
             }, 
             {
                 text: "Games",
                 url: "#"
             },
             {
                 text: "Videos",
                 url: "#"
             },
             {
                 text: "News",
                 url: "#"
             }
          ],

          shop: [
             {
                 text: "Shop DC",
                 url: "#"
             }, 
             {
                 text: "Shop DC Collecibles",
                 url: "#"
             }
          ],
          DC: [
             {
                 text: "Terms of use",
                 url: "#"
             }, 
             {
                 text: "Privacy policy (New)",
                 url: "#"
             }, 
             {
                 text: "Ad Choises",
                 url: "#"
             },
             {
                 text: "Advertising",
                 url: "#"
             }, 
             {
                 text: "Jobs",
                 url: "#"
             },
             {
                 text: "Subscriptions",
                 url: "#"
             },
             {
                 text: "Talent Workshops",
                 url: "#"
             },
             {
                 text: "CPSC Certificates",
                 url: "#"
             },
             {
                 text: "Ratings",
                 url: "#"
             },
             {
                 text: "Shop Help",
                 url: "#"
             },
             {
                 text: "Contact Us",
                 url: "#"
             }

          ],
         sities: [
             {
                 text: "DC",
                 url: "#"
             }, 
             {
                 text: "MAD Magazine",
                 url: "#"
             }, 
             {
                 text: "DC Kids",
                 url: "#"
             },
             {
                 text: "DC Universe",
                 url: "#"
             }, 
             {
                 text: "DC Power Visa",
                 url: "#"
             }
        ]

      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    #container {
        background-image: url("../assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: 100%;
        width: 100%;
    }

    #primaparte {
        color: white;
        display: flex;
        justify-content: flex-start;
    }

    #secondaparte {
        background-color: grey;
        height: 100px;
    }

    li {
        list-style: none;
    }

    a {
        color: rgb(96, 96, 96);
        text-decoration: none;
    }
</style>