<template>
  <header>
      <div class="container">
          <a href="#">
              <img class="brand" src="../assets/img/dc-logo.png" alt="logo DC">
          </a>
            <nav>
                <ul>
                    <li v-for="(link, index) in menuLinks"
                        :key="index"
                    >
                        <a :href="link.url">{{link.label}}</a>
                    </li>
                </ul>
            </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            menuLinks: [
                {
                    label: 'characters', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'comics', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'movies', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'tv', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'games', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'collectibles', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'videos', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'fans', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'news', 
                    url: '#',
                    active: false,
                },
                {
                    label: 'shop', 
                    url: '#',
                    active: false,
                },
                

            ]
        }
    },
}

</script>

<style lang="scss" scoped>
    @import '../style/layout';
    @import '../style/mixins';

    
    header {
        font-weight: 600;
        text-transform: uppercase;
    }
    .container {
        height: 120px;
        @include flex-row-center('vertical');
        justify-content: space-between;

        .brand {
            height: 80px;
        }
        li {
            display:inline-flex;
            &:not(:last-of-type) {
                margin-right: 1.8rem;
            }
        }
    }
</style>