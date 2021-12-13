<template>
    <div id="main">
            <Navigation />
            <div class="page_title"><h1>My Working Experience</h1></div>
          
            <div id="work">
                <div id="work_content">
                    <ul>
                        <li class="workList">
                            <h2>Verizon Wireless, Waltham, MA</h2>
                            <h3>Senior Software Engineer, Oct 2019 - Aug 2021</h3>

                            <img id="verizon" class="work-img" src="../static/multimedia/verizon-lte-innovation-center.jpeg" alt="verizon">
                            <ul>
                                <li><p>Used Golang to maintain and develop company’s container based microservices in the Verizon Thingspace IOT project</p></li>
                                <li><p>Used Docker and K8s to build service images and deployed on AWS ec2 instance for releasing</p></li>
                                <li><p>Designed and implemented the data storage using Redis application cache, and connected to services using Redigo client</p></li>
                                <li><p>Implemented the RabbitMQ messaging queues as message broker in microservices</p></li>
                                <li><p>Implemented GPG Key Pair on JWT for RESTful services to secure the client service talk, using Runscope to monitor APIs</p></li>
                            </ul>
                            <a href="https://thingspace.verizon.com/index.html"><p>Click here to check my Verizon Project</p></a>
                        </li>  
                        
                        <li class="workList">
                            <h2>HBUS Holdco Inc(Huobi-US), San Francisco, CA</h2>
                            <h3>Software Developer, Aug 2018 – Sep 2019</h3>

                            <img id="hbus" class="work-img" src="../static/multimedia/hbus.jpeg" alt="hbus">
                            <ul>
                                <li><p>Designed and implemented the RESTful API services in Java with trigger of node.js on the customer’s on-boarding data collection</p></li>
                                <li><p>Designed and developed front-end using Vue.js, providing support for projects including customer on-boarding and fiat transaction. Deployed the program into Jenkins test environment and production</p></li>
                                <li><p>Designed and developed the token list page for company and deployed to production</p></li>
                                <li><p>Worked on the front-end of MIS internal management platform that allows the view and change on account binding status using Vue.js and IviewUI</p></li>
                                <li><p>Implemented backend data persistent on node.js for customer on-boarding data</p></li>
                                <li><p>Performed the QA automatic test on the cooperated bank's APIs including account creation, contribution and disbursement using JSON and Python on Newman on both sandbox and production</p></li>
                                <li><p>Used Agile/Scrum development methodologies, and used JIRA tracking system for planning and building products</p></li>
                            </ul>
                            <a href="https://www.huobi.us/"><p>Click here to check HBUS homepage</p></a>
                        </li>
                        <li class="workList">
                            <h2>Huangshan Multinational Workshop & Trade Coop, Huangshan, China</h2>
                            <h3>Software Developer, Aug 2018 – Sep 2019</h3>
                            <ul>
                                <li><p>Implemented a service using JavaScript to manage the payment transaction</p></li>
                                <li><p>Used JavaScript to design the company website for listing and ordering</p></li>
                                <li><p>Maintained, and enhanced the website for usability</p></li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
</template>

<script>
export default {
   head() {
        return {
            title: "working experience",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "my working experience"
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

#main {
    width: 980px;
    margin: auto;
    background-color: rgb(245, 219, 216);
}

.navigation_bar {
    background-color: rgb(245, 219, 216) !important;
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

#work-list {
    font-size: 30px;
}

h2{
    margin-top: 60px;
    color: #44c5ae;
    font-size:  30px;
}

h3{
    color: #ff5757;
    font-size: 25px;
}

p{
    color: rgb(0, 0, 0);
    font-size: 20px;
}

a p{
    color: blue;
}

#work{
    width: 90%;
    display: inline-block;
}

#work_content{
    display: inline-block;
}

.work-img{
    margin-top: 30px;
    margin-bottom: 30px;
}

#hbus {   
    width: 620px;
}

</style>