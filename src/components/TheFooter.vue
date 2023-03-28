


<template>
     <footer id="site_footer">
        <div class="footer_top">
            <div class="container py-4 d-flex justify-content-between">
                <div class="row gx-5">
                    <div class="col" v-for="link in menuLinks">
                        <h4>{{ link.title }}</h4>
                        <ul class="list-unstyled">
                            <li v-for="item in link.list"><a href="#">{{ item }}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer_bot py-4">
            <div class="container d-flex justify-content-between">
                <div class="signup">
                    <a href="#" class="btn text-white border border-2 border-primary">SIGN-UP NOW!</a>
                </div>
                <div class="socials d-flex justify-content-around">
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="../assets/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-periscope.png" alt=""></a>

                </div>
            </div>
        </div>
    </footer>

</template>


<script>
export default {

    data() {
        return {
            menuLinks: [
                {
                    title: "Dc Comics",
                    list: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
                },
                {
                    title: "Shop",
                    list: ["Shop DC", "Shop DC Collectibles"],
                },
                {
                    title: "DC",
                    list: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                },
                {
                    title: "Sites",
                    list: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
                },
            ]
        }
    }
}


</script>

<style lang="scss" scoped>
@use "bootstrap";
footer{
    min-height: 60vh;
    background-image: url("../../public/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}


.footer_bot {
    background-color:#303030;
    z-index: 1;

   
}
.socials {
        flex-basis: 35%;
    }
    h3{
        color: #0282F9;
    }

.container {
        background-image: url("../assets/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position: right;
        .row{
            flex-direction: column;
            height: 330px;
        }

        h4 {
            text-transform: uppercase;
            color: white;
        }
    
        a {
           color: antiquewhite;
            text-decoration: none;
        }
    }

</style>