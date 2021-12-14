<template>
    <div>
    <main>
    <Navigation />
    <div class="page_title"><h1>Hantao's Education</h1></div>
    <table id="edu_table">
        <thead>
            <tr>
                <th>School Name</th>
                <th>Location</th>
                <th>Degree Earned</th>
                <th>Graduate Year</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Boston University</td>
                <td>Boston, MA</td>
                <td>M.S of Computer Science</td>
                <td>2022</td>
            </tr>
            <tr>
                <td>Troy University</td>
                <td>Troy, AL</td>
                <td>B.S of Computer Science</td>
                <td>2018</td>
            </tr>
            <tr>
                <td>Luther College</td>
                <td>Decorah, IA</td>
                <td>Transfer From</td>
                <td>2016</td>
            </tr>
            <tr>
                <td>United World College-USA</td>
                <td>Montezuma, NM</td>
                <td>IB diploma</td>
                <td>2012</td>
            </tr>
        </tbody>
    </table>
    <div id="edu_img">
        <a href="https://www.bu.edu/" id="bu"><img src="../static/multimedia/boston_university.png" alt="boston_university"></a>
        <a href="https://www.troy.edu/index.html" id="troy"><img src="../static/multimedia/troy_university.jpg" alt="troy_university"></a>
        <a href="https://www.uwc-usa.org" id="uwc"><img src="../static/multimedia/UWC-USA_logo.gif" alt="uwc_usa"></a>
    </div>
    </main>
    </div>
</template>

<script>
export default {
  head() {
        return {
            title: "eduction",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "my education received"
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

main {
    width: 1200px;
    margin: auto;
    
}

.navigation_bar {
    background-color: rgb(245, 224, 224) !important;
}



.page_title {
    padding-top: 30px;
    margin: auto;
    text-align: center;
}

.page_title h1 {
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: rgb(176, 126, 241);
    font-size: 34px;
}

#edu_table {
    margin: auto;
    margin-top: 60px;
}

#edu_table table{
    border-collapse: collapse;
    width: 500px;
}

#edu_table th, td {
    text-align: left;
    padding: 8px;
}

#edu_table tr:nth-child(even){background-color: #f2f2f2}

#edu_table tr:nth-child(odd){background-color: #ffffff}

#edu_table th {
    background-color: #04AA6D;
    color: white;
}

#edu_img {
    width: 1000px;
    margin: auto;
    margin-top: 100px;
    display: flex;
}

#edu_img > a {
    padding: 20px;
}

#troy {
    margin: auto;
}

#troy img, #bu img{
    height: 192px;
}

</style>