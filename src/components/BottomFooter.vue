
<template>
    <div class="bottom-footer">
            <div class="container">
                <div> 
                    <a class="cta" href="#">sign-up now!</a>
                </div>
                <div class="social">
                    <span> follow us </span>
                    <ul>
                        <li>
                            <a href="#">
                                <img src="@/assets/img/footer-facebook.png" alt="facebook">
                            </a>
                        </li>
                         <li>
                            <a href="#">
                                <img src="@/assets/img/footer-twitter.png" alt="twitter">
                            </a>
                        </li>
                         <li>
                            <a href="#">
                                <img src="@/assets/img/footer-youtube.png" alt="youtube">
                            </a>
                        </li>
                         <li>
                            <a href="#">
                                <img src="@/assets/img/footer-pinterest.png" alt="pinterest">
                            </a>
                        </li>
                         <li>
                            <a href="#">
                                <img src="@/assets/img/footer-periscope.png" alt="periscope">
                            </a>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
</template>

<script>
export default {
    name: 'BottomFooter',
}
</script>

<style lang="scss" scoped>

    @import '../style/mixins';
    @import '../style/vars';


    .bottom-footer {
        height: 110px;
        background: #303030;
        .cta {
            background-color: transparent;
        }
        & > .container {
            height: 100%;
            @include flex-row-center('vertical');
            justify-content: space-between;
            .social {
                @include flex-row-center('vertical');
                span {
                    font-weight: 600;
                    text-transform: uppercase;
                    color: $brand-colors;
                }
                li {
                    display: inline-flex;
                    margin-left: 20px;
                }
            }
        }
    }

</style>