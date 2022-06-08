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
          <section id="bg-logo"></section>
        </div>
        <!-- sezione inferiore -->
        <div class="down">

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
    }

  }

</style>
