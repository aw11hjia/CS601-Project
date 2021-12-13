<template>
    <div>
        <ul class="navigation_bar">
               <li><a href="/">Home</a></li>
               <li><a href="/education">My Education</a></li>
               <li><a href="/work">My Working Experience</a></li>
               <li><a href="/hometown">My Hometown</a></li>
               <li><a href="/news">Hometown News</a></li>
               <li><a href="/travel">My Travels</a></li>
               <li><a href="/contact">Contact Me</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Navigation',
}
</script>

<style>
.navigation_bar {
    width: 100%;
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: rgb(255, 255, 255);
}

.navigation_bar li {
    float: left;
}
  
.navigation_bar li a {
    display: block;
    color: black;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}
  
.navigation_bar li a:hover {
    background-color: rgb(112, 112, 112);
}
</style>