<template>



<div class="parentcontainer">
    <div class="headercontainer" :class="{ 'fixedheader': is_expanded }">
        <div class="header">

            <div class="headerleft">
                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <div class="navlist">
                    <ul class="nav">

                        <div class="product" @mouseover="showproductpopup" @mouseleave="hideproductpopup">

                        <li>
                            <a href="">PRODUCT</a>
                            <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='24' height='24'><path d="M11.178 19.569a.998.998 0 0 0 1.644 0l9-13A.999.999 0 0 0 21 5H3a1.002 1.002 0 0 0-.822 1.569l9 13z"></path></svg>
                        </li>

                        <div class="productpopup" v-if="is_producthovered">
                            <h1>helloworld</h1>
                        </div>
                        </div>



                        <div class="pricing" >

                        <li>
                            <a href="">PRICING</a>
                        </li>
                        </div>



                        <div class="support" >

                        <li>
                            <a href="">SUPPORT</a>
                        </li>
                        </div>



                        <div class="resources" @mouseover="showresourcespopup" @mouseleave="hideresourcespopup" >

                        <li>
                            <a href="">RESOURCES</a>
                            <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='24' height='24'><path d="M11.178 19.569a.998.998 0 0 0 1.644 0l9-13A.999.999 0 0 0 21 5H3a1.002 1.002 0 0 0-.822 1.569l9 13z"></path></svg>
                        </li>
                        <div class="resourcespopup" v-if="is_resourceshovered">
                            <h1>helloworld</h1>
                        </div>
                        </div>

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
                <div class="hamburger hamburger--spin-r" :class="{ 'is-active': is_expanded }" @click="ToggleMenu">
                    <span class="bar"></span>
                    <span class="bar"></span>
                    <span class="bar"></span>
                </div>
            </div>
        </div>
    </div>
    <div class="menuslidelist" :class="{ 'is-expanded': is_expanded }">
        <button class="login">LOG IN</button>
        <div class="products">
            <a href="">PRODUCT</a>        
            <div class="productlist">
                <a href="">Stark Web App</a>
                <a href="">Stark for Figma</a>
                <a href="">Stark for FigJam</a>
                <a href="">Stark for Sketch</a>
                <a href="">Stark for Adobe XD</a>
                <a href="">Stark for Chrome</a>
                <a href="">Stark for Firefox</a>
                <a href="">Stark for Edge</a>
                <a href="">Stark for Safari</a>
                <a href="">Stark for Arc</a>
                <a href="">Stark for Brave</a>
            </div>
        </div>
        <div class="menuitem">
            <a href="">PRICING</a>
        </div>
        <div class="menuitem">
            <a href="">SUPPORT</a>
        </div>
        <div class="menuitem">
            <a href="">BLOG</a>
        </div>
        <div class="menuitem">
            <a href="">LIBRARY</a>
        </div>
        <div class="menuitem">
            <a href="">COMMUNITY</a>
        </div>

    </div>
    <div class="body" v-if="!is_expanded">
        <div class="leftpanel">
            <h3>Search Library</h3>

            <div class="searchbar">
                <div class="searchicon">
                <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='20' height='20'><path d="M10 18a7.952 7.952 0 0 0 4.897-1.688l4.396 4.396 1.414-1.414-4.396-4.396A7.952 7.952 0 0 0 18 10c0-4.411-3.589-8-8-8s-8 3.589-8 8 3.589 8 8 8zm0-14c3.309 0 6 2.691 6 6s-2.691 6-6 6-6-2.691-6-6 2.691-6 6-6z"></path></svg>

                </div>
            <input type="text" placeholder="input">
            </div>
            <div class="menulist">
                <ul>
                    <li>
                        <a href="">Home</a>
                    </li>
                    <li>
                        <a href="">Collections</a>
                    </li>
                    <li class="categories">
                        <a href="">Categories</a>


                    </li>
                </ul>
            </div>
            <div class="contribute">
                <h3>Contribute to Stark</h3>
                <p>Got any accessibility resources or news ?</p>
                <button>Submit a Resource</button>
            </div>
        </div>

        <div class="rightpanel">
        <div class="section1">
            <div class="new">

                <div>
                    <h1>New in the Library</h1>
                    <a href="">VIEW ALL</a>
                </div>

                <p>Newly added accessibility resources,guides,and more.</p>
            </div>
        </div>
        <div class="section2">
            <div class="box">
                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
                
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
                
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
        </div>

        </div>
    </div>
    <div class="mobilebody" v-if="!is_expanded">
        <div class="menulistparent">
            <div class="menulist">
                <ul class="navlist">
                    <li>
                        <a href="">Home</a>
                    </li>
                    <li>
                        <a href="">Collections</a>
                    </li>
                    <li class="categories">
                        <a href="">Categories</a>


                    </li>
                </ul>
            <div class="searchbar">
                <div class="searchicon">
                <svg xmlns='http://www.w3.org/2000/svg'  viewBox='0 0 24 24' fill='#000000' width='20' height='20'><path d="M10 18a7.952 7.952 0 0 0 4.897-1.688l4.396 4.396 1.414-1.414-4.396-4.396A7.952 7.952 0 0 0 18 10c0-4.411-3.589-8-8-8s-8 3.589-8 8 3.589 8 8 8zm0-14c3.309 0 6 2.691 6 6s-2.691 6-6 6-6-2.691-6-6 2.691-6 6-6z"></path></svg>

                </div>
            <input type="text" placeholder="input">
            </div>
            </div>

        </div>
<!-- 
        <div class="sections">
        <div class="section1">
            <div class="new">

                <div>
                    <h1>New in the Library</h1>
                    <a href="">VIEW ALL</a>
                </div>

                <p>Newly added accessibility resources,guides,and more.</p>
            </div>
        </div>
        <div class="section2">
            <div class="box">
                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
                
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
                
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
            <div class="box">
                                <div class="logo">
                    <img src="../assets/starklogo2.png" alt="">
                </div>
                <h1>RESOURCES</h1>
                <h2>Making Accessible Books</h2>
            </div>
        </div>

        </div> -->
    </div>
    <div class="footer"></div>

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



const is_producthovered = ref(false)

const  showproductpopup= () => {
    is_producthovered.value = true;
}
const  hideproductpopup= () => {
    is_producthovered.value = false;
}


const is_resourceshovered = ref(false)

const  showresourcespopup= () => {
    is_resourceshovered.value = true;
}
const  hideresourcespopup= () => {
    is_resourceshovered.value = false;
}


</script>



<style scoped lang="scss">
@import '../sass/main.scss';
</style>

