<template>
    <footer>
        <div class="container">
            <div v-for="(menu, index ) in footerLists" :key="index" class="footer-menu">
                <h3>{{menu.title}}</h3>
                <ul>
                    <li v-for="(link, index) in menu.links" 
                        :key="index">
                            {{link.label}}
                    </li>
                </ul>
            </div>
        </div>
        <BottomFooter/>

        
    </footer>
</template>

<script>
import BottomFooter from '@/components/BottomFooter'
export default {
    name: 'Footer',
    components: {
        BottomFooter,
    },
    data() {
        return {
            footerLists: [
                {
                    title: 'DC COMICS',
                    links: [
                        { label: 'Characters', url: '#', active: false, },
                        { label: 'Comics', url: '#', active: false, },
                        { label: 'Movies', url: '#', active: false, },
                        { label: 'Tv', url: '#', active: false, },
                        { label: 'Games', url: '#', active: false, },
                        { label: 'Videos', url: '#', active: false, },
                        { label: 'News', url: '#', active: false, },       
                    ]
                },
                {
                    title: 'DC SHOP',
                    links: [
                        { label: 'Shop DC', url: '#', active: false, },
                        { label: 'Shop DC Collectibles', url: '#', active: false, },     
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        { label: 'Terms Of Use', url: '#', active: false, },
                        { label: 'Privacy Policy (New)', url: '#', active: false, },
                        { label: 'Ad Choices', url: '#', active: false, },
                        { label: 'Advertising', url: '#', active: false, },
                        { label: 'Jobs', url: '#', active: false, },
                        { label: 'Subscriptions', url: '#', active: false, },
                        { label: 'CPSC Certificates', url: '#', active: false, },
                        { label: 'Ratings', url: '#', active: false, },       
                        { label: 'Shop Help', url: '#', active: false, },
                        { label: 'Contact Us', url: '#', active: false, },    
                    ]
                },
                {
                    title: 'SITES',
                    links: [
                        { label: 'DC', url: '#', active: false, },
                        { label: 'DC UNIVERSE INFINITE', url: '#', active: false, },
                        { label: 'DC Kids', url: '#', active: false, },
                        { label: 'DC Shop', url: '#', active: false, },
                        { label: 'MAD Magazine', url: '#', active: false, },      
                    ]
                },
            ],

        }
    },
}
</script>

<style lang="scss" scoped>
     @import '../style/mixins';
     @import '../style/vars';



    footer {
        height: 480px;
        background-image: url(../assets/img/footer-bg.jpg);
        & > .container {
            display: flex;
            height: 370px;
            padding-top: 2.5rem;
            flex-direction: column;
            align-content: flex-start;
            flex-wrap: wrap;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position-x: 100%;
            background-position-y: center;
            background-size: 41%;
            .footer-menu {
                width: 150px;
                color: rgb(97, 97, 97);

                h3 {
                    color: #fff;
                    font-weight: 600;
                }
                ul {
                    margin: 1.5rem 0 ;

                }
            }
        }
    }

</style>