<template>
  <div>
      <main>
    
        <Navigation />
    
        <div class="page_title"><h1>Introduction of Hantao</h1></div>
        
        <div id = "index_intro_content">
            <div id = "index_p">
                <div class = "index_p_content"><p>My name is Hantao Jiang. I am 27 years old. I am a first year student of M.S of Computer Science student in Boston University Metropolitan College. </p></div>
                <div class = "index_p_content"><p>Before I entered the college, I had been working in software industry for three years. And my commitment to critical thinking and attention to detail have gotten me to where I am today: a software engineer</p></div>
                <div class = "index_p_content"><p>During my free time, I love playing tennis and billiards with my friends. I also spend lots of time reading articles about the up-to-date technology.</p></div>
            </div>
            <div id = "index_picture_set">
                <div class = "index_picture"><img src="../static/multimedia/Billiard-balls-table.jpeg" alt="billiard"></div>
                <div class = "index_picture"><img src="../static/multimedia/tennis.jpeg" alt="tennis"></div>
            </div>
        </div>
        <br>
        <br>
        <br>
        <div id = "index_subcontent">
            <h4>Technical Background</h4>
            <div id = "index_tech">
              <ul>
                  <li>full stack developer in Software Engineering with extensive education and experience</li>
                  <li>In depth experience in designing and developing RESTful APIs, messaging queues and data storage. </li>
                  <li>Extensive hands-on experience in object-oriented analysis, design, component-based development.</li>
                  <li>fast learner with strong time management and multitasking skills</li>
              </ul>
            </div>
            <br>
            <a href="www.linkedin.com/in/hantao-jiang">Click here to visit my linkedin page</a>
            <br>
            <br>
            <h4>My Favourite Music</h4>
            <iframe width="420" height="315" src="https://www.youtube.com/embed/SX_ViT4Ra7k"></iframe>
        </div>
        </main>
  </div>
</template>

<script>
export default {
  head() {
        return {
            title: "Home Page",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "Home page of project"
                }
            ]
        };
    }
}
</script>

<style>
body {
    background: url("../static/multimedia/book-laptop.jpeg") no-repeat center center fixed;
    background-size: cover;
    background-color: #b89090;
}

.navigation_bar {
    background-color: rgb(245, 224, 224) !important;
}

main {
  width: 1200px;
  margin: auto;
  background-color: rgb(245, 224, 224)
}


.page_title {
    padding-top: 30px;
    margin: auto;
    text-align: center;
}

.page_title h1 {
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color:rgb(211 94 169);
    font-size: 34px;
}

#index_intro_content {
    display: flex;
    flex-direction: column;
    margin: auto;
    text-align: center;
    margin-top: 90px;
    width: 80%;
}

#index_p {
    width: 900px;
    display: inline-block;
    vertical-align: top;
    text-align: left;
}


.index_p_content {
    height: 130px;
    width: 900px;
    display: inline-block;
    vertical-align: top;
}

.index_p_content p {
    margin-top: 0px;
    margin-bottom: 0px;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: rgb(0, 0, 0);
    font-size: 20px;
}

#index_picture_set {
    display: inline-block;
}

.index_picture {
    display: inline-block;
    margin: 15px;
}

@media screen and (max-width: 1100px) {
    #index_p {
        width: 500px;
    }

    .index_p_content {
        width: 500px;
    }

    #work_content{
        width: 800px;
    }

}

@media screen and (max-width: 790px) {
    #index_p {
        width: 400px;
    }

    .index_p_content {
        width: 400px;
        height: 200px;
    }

    #index_picture_set {
        width: 400px;
    }

    .index_picture {
        margin-top: 20px;
    }

    #work_content{
        width: 600px;
    }


}

#index_subcontent {
    margin: auto;
    text-align: center;
    width: 80%;
}

#index_subcontent h4 {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 25px;
    color:rgb(211 94 169);
    margin-top: 100px;
}

#index_subcontent ul {
    text-align: left;
}

#index_subcontent ul li{
    margin-top: 5px;
}

#index_tech {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 20px;
    color:rgb(0, 0, 0);
    margin: auto;
    width: 1000px;
}



</style>