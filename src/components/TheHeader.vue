

<template>
    <header class="container">
        
        <nav>
            <img src="../assets/dc-logo.png" alt="">
            <ul class="navbar-links">
                <li v-for="(link, i) in navLinks" :key="i">
                    <a class="nav-link" :href="link.href">{{ link.text }}</a>
                </li>
                
            </ul>
        </nav>
    </header>

  
</template>


<script>

export default{
    data(){
        return{
            navLinks:[
                {
                    href:"#characters",
                    text: "CHARACTERS"
                },
                {
                    href:"#comics",
                    text: "COMICS"
                },
                {
                    href:"#movies",
                    text: "MOVIES"
                },
                {
                    href:"#tv",
                    text: "TV"
                },
                {
                    href:"#games",
                    text: "GAMES"
                },
                {
                    href:"#collectibles",
                    text: "COLLECTIBLES"
                },
                {
                    href:"#home",
                    text: "VIDEOS"
                },
                {
                    href:"#home",
                    text: "FANS"
                },
                {
                    href:"#home",
                    text: "NEWS"
                },
                {
                    href:"#home",
                    text: "SHOP"
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>

nav{
    display: flex;
   justify-content: space-between;
    align-items: center;
   
}
nav img{
    display: inline-block;
    padding: 0.5rem 1rem;
}
.navbar-links { 
    display: flex;
    justify-content: end;
    align-items: center;
    list-style: none;
}
.nav-link {
    padding: 0.5rem 1rem;
    color: black;
    text-decoration: none;

    &:hover{
    color: blue;
    text-decoration: underline;
}
    
}



</style>