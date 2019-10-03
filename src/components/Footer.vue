<template>
    <footer>
        <div class="container">
            <div class="logo">
                <img src="/assets/img/footer-logo.svg" alt="">
                <span>Eu augue ut lectus
                    <br>arcu bibendum at.</span>
            </div>
            <FooterMenu title="MENU">
              <FooterNav :list="menuList"></FooterNav>
            </FooterMenu>
            <FooterMenu title="SERVICES">
                <FooterNav :list="servicesList"></FooterNav>
            </FooterMenu>
            <FooterMenu title="CONTACT US">
                <FooterNav :list="contactsList"></FooterNav>
            </FooterMenu>
            <FooterMenu title="FOLLOW US">
                <FooterNav direction="horizontal" :list="socialsList"></FooterNav>
            </FooterMenu>
        </div>
    </footer>
</template>

<script>
    import FooterMenu from "@/components/FooterMenu";
    import FooterNav from "@/components/FooterNav";

    export default {
        name: "Footer",
        components: {FooterNav, FooterMenu},
        data() {
            return {
                menuList: [
                    { name: 'Home' },
                    { name: 'About' },
                    { name: 'Services' },
                    { name: 'News' },
                    { name: 'Gallery' },
                    { name: 'Contacts' },
                ],
                servicesList: [
                    { name: 'Lorem' },
                    { name: 'Ipsum' },
                    { name: 'Dolor' },
                    { name: 'Sit Amet' },
                ],
                contactsList: [
                    { name: 'example@gmail.com', image: '/assets/img/letter.svg' },
                    { name: '+7 (999) 999-99-99', image: '/assets/img/number.svg' },
                ],
                socialsList: [
                    { image: '/assets/img/twitter.svg' },
                    { image: '/assets/img/facebook.svg' },
                    { image: '/assets/img/inst.svg' },
                    { image: '/assets/img/youtube.svg'},
                    { image: '/assets/img/m.svg'}
                ],
            };
        }
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    footer {
        background-color: var(--footer-bg-color);
        padding-top: 124px;

        .container {
            display: grid;
            grid-template-columns: 3fr 1fr 1.5fr 2fr 3fr;

            @include tablet-portrait {
                grid-template-columns: 2fr 1fr 1fr;
            }

            .logo {
                display: flex;
                flex-direction: column;
                align-items: flex-start;

                span {
                    font-size: 16px;
                    line-height: 26px;
                    color: var(--service-color);
                    margin-top: 24px;
                }
            }
        }
    }
</style>
