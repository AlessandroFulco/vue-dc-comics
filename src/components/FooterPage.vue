<template>
    <footer>
        <!-- sezione superiore -->
        <div class="row">
          <!-- sx side -->
          <section class="sx">
            <div>
              <h3>DC COMICS</h3>
              <ul>
                <li v-for="(section, index) in sectionsMenu" :key="index">
                  <a :href="section.link">{{section.sectionName}}</a>
                </li>
              </ul>

              <h3>SHOP</h3>
              <ul>
                <li v-for="(section, index) in sectionsShop" :key="index">
                  <a :href="section.link">{{section.sectionName}}</a>
                </li>
              </ul>
            </div>

            <div>
              <h3>DC</h3>
              <ul>
                <li v-for="(section, index) in dc" :key="index">
                  <a :href="section.link">{{section.sectionName}}</a>
                </li>
              </ul>
            </div>

            <div>
              <h3>SITES</h3>
              <ul>
                <li v-for="(section, index) in sites" :key="index">
                  <a :href="section.link">{{section.sectionName}}</a>
                </li>
              </ul>
            </div>
          </section>

          <!-- dx side -->
          <section id="bg-logo">
          </section>
        </div>
        <!-- sezione inferiore -->
        <div class="down">
          <div id="contentFooter">
            <div class="btn">
              SGN-UP NOW!
            </div>
            <div id="media">
              <h3>FOLLOW US</h3>
              <a href="#"><img src="../assets/img/footer-facebook.png" alt="logo Facebook"></a>
              <a href="#"><img src="../assets/img/footer-twitter.png" alt="logo twitter"></a>
              <a href="#"><img src="../assets/img/footer-youtube.png" alt="logo youtube"></a>
              <a href="#"><img src="../assets/img/footer-pinterest.png" alt="logo pinterest"></a>
              <a href="#"><img src="../assets/img/footer-periscope.png" alt="map"></a>
            </div>
          </div>
        </div>


    </footer>
</template>

<script>
export default {
  name: 'FooterPage',
  data() {
    return {
      sectionsMenu: [
        {
          sectionName: "Characters",
          link: "#"
        },
        {
          sectionName: "Comics",
          link: "#"
        },
        {
          sectionName: "Movies",
          link: "#"
        },
        {
          sectionName: "TV",
          link: "#"
        },
        {
          sectionName: "Games",
          link: "#"
        },
        {
          sectionName: "Videos",
          link: "#"
        },
        {
          sectionName: "News",
          link: "#"
        },
      ],
      sectionsShop: [
        {
          sectionName: "Shop DC",
          link: "#"
        },
        {
          sectionName: "Shop DC Collectibles",
          link: "#"
        }
      ],
      dc: [
        {
          sectionName: "Terms of Use",
          link: "#"
        },
        {
          sectionName: "Privacy policy(New)",
          link: "#"
        },
        {
          sectionName: "Ad Choice",
          link: "#"
        },
        {
          sectionName: "Advertising",
          link: "#"
        },
        {
          sectionName: "Jobs",
          link: "#"
        },
        {
          sectionName: "Subscriptions",
          link: "#"
        },
        {
          sectionName: "Talent Workshop",
          link: "#"
        },
        {
          sectionName: "CPSC Certificates",
          link: "#"
        },
        {
          sectionName: "Ratings",
          link: "#"
        },
        {
          sectionName: "Shop Help",
          link: "#"
        },
        {
          sectionName: "Contac Us",
          link: "#"
        },
      ],
      sites: [
        {
          sectionName: "DC",
          link: "#"
        },
        {
          sectionName: "MAD Magazine",
          link: "#"
        },
        {
          sectionName: "DC Kids",
          link: "#"
        },
        {
          sectionName: "DC Universe",
          link: "#"
        },
        {
          sectionName: "DC Power Visa",
          link: "#"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  footer {
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: none;
    background-size: contain;

    div.row {
      display: flex;
      width: 80%;
      min-height: 200px;
      margin: 0 auto;
      section.sx {
        width: 45%;
        display: flex;
        justify-content: flex-start;
        flex-wrap: wrap;

        div {
          padding: 10px;
          h3 {
            margin-top: 10px;
            color: #fff;
          }

          ul {
            list-style-type: none;
            
            li {
              a {
                display: inline-block;
                color: #888;
                padding: 5px 5px;
                font-size: 12px;
                text-decoration: none;
                font-weight: bold;
                &:hover {
                  background-color: rgba(255, 255, 255, 0.6);
                  color: #fff;
                }
              }
            }
          }
        }
      }
      section#bg-logo {
        width: 55%;
        background-image: url("../assets/img/dc-logo-bg.png");
        background-position: center center;
        background-repeat: none;
        background-size: cover;

      }
    }
    div.down {
      height: 100px;
      background-color: #303030;
      #contentFooter{
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 0 auto;
        width: 80%;

        .btn {
          background-color: transparent;
          border: 1px solid #0282f9;
        }
        #media{
          h3 {
            color:#0282f9;
          }
          display: flex;
          align-items: center;
          gap: 15px;
        }
      }
    }
  }

</style>
