<template>
    <div>
    <Navigation />   
    <div class="page_title"><h1>My Travels In The US</h1></div>
   
        <div id="usmap">

                <div class="dot" id='la' @mouseover="la_hover = true" @mouseleave="la_hover = false"></div>
                <div class="dot" id='sf' @mouseover="sf_hover = true" @mouseleave="sf_hover = false"></div>
                <div class="dot" id='sd' @mouseover="sd_hover = true" @mouseleave="sd_hover = false"></div>
                <div class="dot" id='abq' @mouseover="abq_hover = true" @mouseleave="abq_hover = false"></div>
                <div class="dot" id='decorah' @mouseover="decorah_hover = true" @mouseleave="decorah_hover = false"></div>
                <div class="dot" id='chi' @mouseover="chi_hover = true" @mouseleave="chi_hover = false"></div>
                <div class="dot" id='mon' @mouseover="mon_hover = true" @mouseleave="mon_hover = false"></div>
                <div class="dot" id='atl' @mouseover="atl_hover = true" @mouseleave="atl_hover = false"></div>
                <div class="dot" id='orl' @mouseover="orl_hover = true" @mouseleave="orl_hover = false"></div>
                <div class="dot" id='mia' @mouseover="mia_hover = true" @mouseleave="mia_hover = false"></div>
                <div class="dot" id='phi' @mouseover="phi_hover = true" @mouseleave="phi_hover = false"></div>
                <div class="dot" id='nyc' @mouseover="nyc_hover = true" @mouseleave="nyc_hover = false"></div>
                <div class="dot" id='bos' @mouseover="bos_hover = true" @mouseleave="bos_hover = false"></div>





                <div class="text" id='la-text' v-if = la_hover>
                    <p>Though I never had a chance to have fun in LA, I have often used the airport travel back to and from China since 2011.</p>
                </div>
                <div class="text" id='sf-text' v-if = sf_hover>
                    <p>I worked in San Francisco from 2018 to 2020, right after I got my bachelor's degree.</p>
                </div>
                <div class="text" id='sd-text' v-if = sd_hover>
                    <p>I visited San Diego with my friends during 2012 summer. I really like the beach and zoo there.</p>
                </div>
                <div class="text" id='abq-text' v-if = abq_hover>
                    <p>I flyed to Albuquerque in 2011 for high school. And my school is in Montezuma, a town 30min drive from Albuquerque.</p>
                </div>
                <div class="text" id='decorah-text' v-if = decorah_hover>
                    <p>I had my first two years Luther College in Decorah, IA.</p>
                </div>
                <div class="text" id='chi-text' v-if = chi_hover>
                    <p>I used Chicago airport for travel when I studied in Iowa. Sometimes I went to Chicago for shopping during weekends.</p>
                </div>
                <div class="text" id='mon-text' v-if = mon_hover>
                    <p>I spent three years in Troy University in Troy, AL. And I earned my B.S of Computer Science there.</p>
                </div>
                <div class="text" id='atl-text' v-if = atl_hover>
                    <p>Most times I used Atlanta airport to travel to and from China when I studied in Troy University.</p>
                </div>
                <div class="text" id='orl-text' v-if = orl_hover>
                    <p>I played in Universal Studios and Disneyland in Orlando, FL in summer 2016.</p>
                </div>
                <div class="text" id='mia-text' v-if = mia_hover>
                    <p>I travelled to Miami and Key West with my parents in summer 2017.</p>
                </div>
                <div class="text" id='phi-text' v-if = phi_hover>
                    <p>I travelled to Philadelphia in 2018. I enjoyed the history of the city.</p>
                </div>
                <div class="text" id='nyc-text' v-if = nyc_hover>
                    <p>I have been to NYC twice. The places I liked most there are Brooklyn Bridge and The Metropolitan Museum of Art.</p>
                </div>
                <div class="text" id='bos-text' v-if = bos_hover>
                    <p>I worked in Boston for two years since 2019. After that I went to Boston University for my M.S of Computer Science.</p>
                </div>

        </div>

    </div>
</template>

<script>


export default {
  data() {
    return {
      la_hover: false,
      sf_hover: false,
      sd_hover: false,
      abq_hover: false,
      decorah_hover: false,
      chi_hover: false,
      mon_hover: false,
      atl_hover: false,
      orl_hover: false,
      mia_hover: false,
      phi_hover: false,
      nyc_hover: false,
      bos_hover: false,
    };
  },
  head() {
        return {
            title: "travel",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "My travels in the US"
                }
            ]
        };
    }
}
</script>

<style>
body {
    background: url("../static/multimedia/usa-map-hd-blur.png") no-repeat;
    background-size: cover;
    background-color: rgb(135, 188, 228);
    
}


.page_title {
    padding-top: 30px;
    margin: auto;
    text-align: center;
}

.page_title h1 {
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #245cd3;
    font-size: 34px;
}

#usmap {
    margin: auto;
    width: 1500px;
    height: 1006px;
    background: url("../static/multimedia/usa-map-hd.jpeg") no-repeat;
    position: relative;
}


.dot {
    height: 25px;
    width: 25px;
    background-color: rgb(223, 29, 29);
    border-radius: 50%;
    position: relative;

}

.dot:hover{
    background-color: blue;
}

#la {
    top: 584px;
    left: 228px;
}

#sf {
    top: 444px;
    left: 129px;
}

#sd {
    top: 565px;
    left: 252px;
}

#abq {
    top: 478px;
    left: 500px;
}

#decorah {
    top: 241px;
    left: 856px;
}

#chi {
    top: 223px;
    left: 951px;
}

#mon {
    top: 473px;
    left: 979px;
}

#atl {
    top: 413px;
    left: 1026px;
}

#orl {
    top: 528px;
    left: 1097px;
}

#mia {
    top: 577px;
    left: 1121px;
}

#phi {
    top: 157px;
    left: 1245px;
}

#nyc {
    top: 106px;
    left: 1271px;
}

#bos {
    top: 28px;
    left: 1340px;
}

.text {
    height: 120px;
    width: 200px;
    background-color: white;
    border-radius: 5%;
    position: absolute;
    border-color: #304547;
    border-style: solid;
}

.text p {
    font-size: 16px;
    margin-left: 5px;
    margin-right: 5px;
}

#sf-text {
    top: 510px;
    left: 30px;
}

#la-text {
    top: 627px;
    left: 128px;
}

#sd-text {
    top: 653px;
    left: 155px;
}

#abq-text {
    top: 592px;
    left: 403px;
}

#decorah-text {
    top: 388px;
    left: 757px;
}

#chi-text {
    top: 395px;
    left: 850px;
}

#mon-text {
    top: 669px;
    left: 895px;
}

#atl-text {
    top: 634px;
    left: 925px;
}

#orl-text {
    top: 773px;
    left: 993px;
}

#mia-text {
    top: 849px;
    left: 1041px;
}

#phi-text {
    top: 447px;
    left: 1150px;
}

#nyc-text {
    top: 423px;
    left: 1175px;
}

#bos-text {
    top: 371px;
    left: 1243px;
}

</style>