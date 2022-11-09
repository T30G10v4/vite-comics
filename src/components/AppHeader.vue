<script>
  export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    title: "Characters",
                    href: "/characters",
                    active: false,
                },
                {
                    title: "Comics",
                    href: "/comics",
                    active: true,
                },
                {
                    title: "Movies",
                    href: "/movies",
                    active: false,
                },
                {
                    title: "TV",
                    href: "/tv",
                    active: false,
                },
                {
                    title: "Games",
                    href: "/games",
                    active: false,
                },
                {
                    title: "Collectibles",
                    href: "/collectibles",
                    active: false,
                },
                {
                    title: "Videos",
                    href: "/videos",
                    active: false,
                },
                {
                    title: "Fans",
                    href: "/fans",
                    active: false,
                },
                {
                    title: "News",
                    href: "/news",
                    active: false,
                },
                {
                    title: "shop",
                    href: "/shop",
                    active: false,
                },
            ]
        }
    }
}
</script>

    <template>

        <header>
            <div class="container">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <nav>
                    <ul>
                        <li 
                        v-for="(link, index) in links" 
                        :key="index"
                        >
                            <a 
                                :href="`${link.href}`"
                                class="active"
                                >
                                {{ link.title }}
                            
                            </a>
                            
                        </li>
                    </ul>
                </nav>
            </div>
        </header>
    </template>

<style lang="scss" scoped>
  @use "../styles/partials/variables" as *;

header {

    .container {

        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem 0;

        ul {

            list-style-type: none;
            display: flex;

            li {

                margin-left: 1rem;
                

                a {

                    display: inline-block;
                    text-decoration: none;
                    line-height: 103px;
                    position: relative;
                    &.active {
                        
                        position: absolute;
                        width: 100%;
                        height: 3px;
                        bottom: 0;
                        left: 0;
                    }

                }
  

            }

        }

    }



}

</style>