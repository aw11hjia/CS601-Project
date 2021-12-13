<template>
    <div id="main">
    <Navigation />
    
    <div>
        <h1>My Hometown - Nanjing</h1>
        <p class="intro">Nanjing, the capital of Jiangsu Province, is one of China's greatest ancient capitals, located in Eastern China, near the Yangtze River. It is about 2 hours by air from Beijing and an hour from Shanghai.</p>
        <p class="intro">I left Nanjing when I was 16 years old. After that, I hardly had chances go back to my home town. Till now, I still miss everything about it everyday.</p>
        

    </div>

     <VueSlickCarousel :arrows="true" :dots="true">
      <div><img src="../static/multimedia/Nanjing1.jpg" style="width:100%" class="carousel_img"></div>
      <div><img src="../static/multimedia/Nanjing2.jpg" style="width:100%" class="carousel_img"></div>
      <div><img src="../static/multimedia/Nanjing3.jpg" style="width:100%" class="carousel_img"></div>
      <div><img src="../static/multimedia/Nanjing4.jpg" style="width:100%" class="carousel_img"></div>

    </VueSlickCarousel>

  <h2 id="location-title">Location</h2>
  <img src="../static/multimedia/Nanjing-map.png" class="hometown-img">
  <p>Nanjing, the capital of Jiangsu Province, is one of China's greatest ancient capitals, located in Eastern China, near the Yangtze River. It is about 2 hours by air from Beijing and an hour from Shanghai.</p>

  <h2>Population</h2>
  <img src="../static/multimedia/Nanjing-population.svg" class="hometown-img" width=80%>
  <p>The city has a population of 8,270,500 people stretched across 2,500 square miles. This makes the population density 3,183 people residing here per square mile.</p>
  <p>The city has seen steady growth throughout the years, posting double-digit growth during the 1960s and 1970s. The city’s natural growth rate has slowed in recent years, but because of Nanjing’s rich culture and history, its thriving economy and educational opportunities, this growth is expected to continue.</p>

  <h2>History</h2>
  <img src="../static/multimedia/Nanjing-history.jpeg" class="hometown-img" width=80%>
  <p>Nanjing first became a state capital in AD 229, when the state of Eastern Wu founded by Sun Quan during the Three Kingdoms period relocated its capital to Jianye (建業), the city extended on the basis of Jinling Yi in AD 211. Although conquered by the Western Jin dynasty in 280, Nanjing and its neighboring areas had been well cultivated, developing into one of the commercial, cultural and political centers of China during the Eastern Wu. </p>
    <p>This city would soon play a vital role in the following centuries. At the end of the Eastern Han Dynasty, Sun Quan, who ruled Jiangdong, moved his ruling office to Moling in 211. The following year, he built a stone city fortress in the old place of Jinling Town. In 229, Sun Quan proclaimed himself emperor in Wuchang and established Dong Wu (Eastern Wu). Then he moved his capital to Jianye, known as the "Zhongshan Dragon Plate, Stone Tigers", and opened the history of Nanjing as the capital. </p>
    <p>In 280, the Western Jin Dynasty destroyed Wu and rebuilt the industry into Moling. In 282, with the Qinhuai River as the boundary, Moling was divided into two counties, Jianye and Moling. In 313, Ye was renamed Jiankang because of avoiding the name taboo of Emperor Sima Ye of the Jin Dynasty. </p>
    <p>In 317, Emperor Sima Rui of the Jin and Yuan dynasties was building a country, known as the Eastern Jin Dynasty, and the northern gentry moved south. After more than 270 years of the Great Separatism between North and South, Jiankang became the orthodox place of China. </p>
    <p>The city has a long and unique history dating back to the 3rd century, and in modern times, is a center for education, culture and tourism. It is also the site of one of the largest inland ports in the world. Nanjing is also known for its number of universities and research centers and is one of the top scientific research centers in the country.</p>

  <h2>Food</h2>
  <p>Once the capital of several Chinese dynasties, Nanjing has a food scene befitting its distinguished history. The city is especially known for its duck, so make sure to be on the prowl for fowl in its many culinary forms.</p>
  <ol>
    <li>
      <h4>Duck Blood and Vermicelli Soup</h4>
      <img src="../static/multimedia/food1.jpeg" class="hometown-img" width=70%>
      <p>One of the most famous Nanjing delicacies, duck blood and vermicelli soup is popular with both locals and people from other parts of China. It consists of vermicelli soaked in duck soup, cubes of duck blood, deep-fried tofu and vegetables.</p>
    </li>

    <li>
      <h4>Pan-fried Beef Dumplings</h4>
      <img src="../static/multimedia/food2.jpeg" class="hometown-img" width=80%>
      <p>These pan-fried beef dumplings are considered one of Nanjing’s Eight treasures, namely eight renowned traditional snacks in Nanjing. Stuffed with ground beef, diced ginger and onions, the dumplings are fried until golden and crispy.</p>
    </li>

    <li>
      <h4>Red Bean Soup with Sweet Rice Balls</h4>
      <img src="../static/multimedia/food3.jpeg" class="hometown-img" width=80%>
      <p>These little sweet rice balls in red bean soup are the twin brothers of Tangyuan (汤圆), which are sticky rice balls stuffed with various fillings. The soup with sugared red bean paste goes perfectly well with the tender, self-melt sticky rice balls.</p>
    </li>

    <li>
      <h4>Nanjing Salted Duck</h4>
      <img src="../static/multimedia/food4.jpeg" class="hometown-img" width=80%>
      <p>People in Nanjing love duck. Salted duck, with a history of hundreds of years, is one of the Nanjing classics and is less greasy than most other duck dishes.</p>
    </li>
  </ol>


    <h2>A City With Tragedy</h2>
    <img src="../static/multimedia/Nanjing-massacre.jpeg" class="hometown-img">
    <p>The Nanjing Massacre or the Rape of Nanjing was an episode of mass murder and mass rape committed by Imperial Japanese troops against the residents of Nanjing (Nanking), at that time the capital of China, during the Second Sino-Japanese War (1937–1945). The massacre occurred over a period of six weeks starting on December 13, 1937, the day that the Japanese captured Nanjing.</p>
    <p>Japanese Army murdered tens or hundreds of thousands of disarmed combatants and unarmed Chinese civilians, and perpetrated widespread rape and looting. An estimated of over 300,000 Chinese were killed.</p>
  </div>
</template>

<script>
  
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'

  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

  export default {
    name: 'MyComponent',
    components: { VueSlickCarousel },
    head() {
        return {
            title: "hometown",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "description of my hometown"
                }
            ]
        };
    }
  }
</script>

<style>
body {
  background: url("../static/multimedia/hometown-background-blur.jpg") no-repeat center center fixed;
}

#main{
    width: 1050px;
    padding-left: 30px;
    padding-right: 30px;
    padding-bottom: 30px;
    margin: auto !important;
    background-color: #a0cacf;
}

.navigation_bar {
    background-color: #a0cacf !important;
}


ol{
  font-size: 25px;
}

h1 {
  padding-top: 30px;
  padding-bottom: 50px;
  text-align: center;
  font-size: 50px;
}

p {
  width: 980px;
  margin: auto;
  font-size: 20px;
  margin-bottom: 30px;
}

h2 {
  margin-top:60px;
  margin-bottom: 60px;
  font-size: 35px;
  text-align: center;
}

#location-title {
  margin-top: 71px;
  margin-bottom: 40px;
}

.hometown-img{
  margin: auto;
  margin-bottom: 40px;
  margin-left: 80px;
  
}

h4{
  margin-top: 60px;
  margin-bottom: 65px;
  font-size: 25px;
}

.carousel_img{
    width: 980px;  
    height: auto; 
    margin: auto;
}


</style>