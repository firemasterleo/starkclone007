<template>
<div class="grandparent">


<div class="parentcontainer">
    <div class="headercontainer" :class="{ 'fixedheader': is_expanded }">
        <div class="header">

            <div class="headerleft">
                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <div class="navlist">
                    <ul class="nav">
                        <li>
                            <a href="">PRODUCT</a>
                            <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='24' height='24'><path d="M11.178 19.569a.998.998 0 0 0 1.644 0l9-13A.999.999 0 0 0 21 5H3a1.002 1.002 0 0 0-.822 1.569l9 13z"></path></svg>
                        </li>
                        <li>
                            <a href="">PRICING</a>
                        </li>
                        <li>
                            <a href="">SUPPORT</a>
                        </li>
                        <li>
                            <a href="">RESOURCES</a>
                            <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='24' height='24'><path d="M11.178 19.569a.998.998 0 0 0 1.644 0l9-13A.999.999 0 0 0 21 5H3a1.002 1.002 0 0 0-.822 1.569l9 13z"></path></svg>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="headerright">
                <button class="login">LOG IN</button>
                <button class="startfree">START FREE TRIAL</button>
            </div>


        </div>
        <div class="mobileheader" :class="{ 'fixedheader': is_expanded }">
            
            <div class="headerleft">
                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
            </div>
            <div class="headerright">
                <button class="startfree">START FREE TRIAL</button>
                <div class="hamburger" @click="ToggleMenu">
                <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='28' height='28'><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"></path></svg>

                </div>
            </div>
        </div>
    </div>
    <div class="menuslidelist" :class="{ 'is-expanded': is_expanded }">
        <button class="login"></button>
        <div class="products">
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
            <a href="">PRODUCTS</a>
           
            <div class="productlist"></div>
        </div>
        <div class="pricing">
            <a href="PRICING"></a>
        </div>
    </div>
    <div class="body" v-if="!is_expanded">
        <h1>hellvgggvo</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>hello</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>
        <h1>helloplase</h1>

    </div>
    <div class="footer"></div>

</div>
</div>

<!-- <h1>
okay so to get this 
 slidein menuu right where we have 
 slide menu come in and take the whole screen and is scrollable
 and transitions in and out and the body not visible , we had to use a 
 couple of commands 
 we used v-if="!is_expanded" in the html body tag to hide body and prevent body scroll
 sledein menu was set to fixed bottom 0 to prevent entire slidemenu scrolling
 up once it comes into view
 we used overflow auto, we used visibility hidden to hide 
     slide menu in plain sight to allow access to body when !isexpanded
     also there was a very huge difference between using display none 
     and block vs using visibility visible and hidden to hide objects
      when using media query or @click comands, the latter 

</h1> -->

  
</template>





<script setup>

import { ref } from 'vue'

const is_expanded = ref(false)

const ToggleMenu = () => {
    is_expanded.value = !is_expanded.value;
}

</script>



<style scoped lang="scss">
@import '../sass/main.scss';
</style>

