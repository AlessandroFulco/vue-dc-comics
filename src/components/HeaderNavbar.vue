<template>
  <header>
      <div>
          <img src="../assets/img/dc-logo.png" alt="logo dc comics">
      </div>
      <nav>
          <ul>
              <li v-for="(section, index) in sectionsMenu" :key="index">
                  <a :href="section.url" 
                     :class="section.current ? 'here' : '' "
                  >
                    {{section.name}}
                  </a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderNavbar',
  data(){
    return {
        sectionsMenu: [
            {
                name: "characters",
                ulr: "#",
                current: false
            },
            {
                name: "comics",
                ulr: "#",
                current: true
            },
            {
                name: "movies",
                ulr: "#",
                current: false
            },
            {
                name: "tv",
                ulr: "#",
                current: false
            },
            {
                name: "games",
                ulr: "#",
                current: false
            },
            {
                name: "collectibles",
                ulr: "#",
                current: false
            },
            {
                name: "videos",
                ulr: "#",
                current: false
            },
            {
                name: "fans",
                ulr: "#",
                current: false
            },
            {
                name: "news",
                ulr: "#",
                current: false
            },
            {
                name: "shop",
                ulr: "#",
                current: false
            },
        ]
    }
    
}
}





</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;

    div {

        img {
            height: 80px;
            width: auto;
        }
    }

    nav {
        height: 100%;
        ul {
            margin: 0;
            list-style-type: none;
            height: 100%;
            li {
                display: inline-block;
                height: 100%;
                a {
                    display: inline-block;
                    height: 100%;
                    padding: 10px;
                    text-decoration: none;
                    color: #000;
                    text-transform: uppercase;
                    cursor: pointer;
                    font-size: 12px;
                    display: flex;
                    align-items: center;

                    &.here {
                        color: blue; 
                        border-bottom: 5px solid blue;
                    }
                }
            }
        }
    }
    
}
h1 {
  color: blueviolet;
}

</style>
