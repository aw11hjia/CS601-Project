<template>
    <div>
    <main>
        <Navigation />
        <h1>My Hometown News</h1>
        <Article v-for="article in articles" :key="article.title" :image="article.image" :id="article.title" :title="article.title" :source="article.source" :date="article.published_at" :description="article.description" :url="article.url"/>
    </main>
    </div>
</template>

<script>
import axios from "axios";
import Article from '../components/Article'

export default {

    components: {
        Article
    },

    data() {
        return {
            articles: []
        }
    },
    async created() {
        const config = {
            headers: {
                'Accept': 'application/json'
            }
        }
        try {
            const res = await axios.get(
            'https://api.mediastack.com/v1/news?keywords=China&access_key=46a0737a62896b755d5b8b8668ea37fc&limit=30&sort=published_desc&languages=en', config);
            //console.log(res.data);

            this.articles = res.data.data;

            console.log(this.articles);
        } catch (error) {
            console.log(error);
        }

    },
    head() {
        return {
            title: "Nanjing News",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "News of my hometown - Nanjing"
                }
            ]
        };
    }
};
</script>
<style>
body {
  background-color: rgb(245, 232, 216);
}
main{
    width: 980px;
    margin: auto;
    background-color: rgb(243, 223, 167);
}

h1 {
    font-size: 50px;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    text-align: center;
}

.navigation_bar {
    list-style-type: none;
    margin: auto;
    overflow: hidden;
    background-color: rgb(243, 223, 167);
}

.navigation_bar {
    background-color: rgb(243, 223, 167) !important;
}

</style>