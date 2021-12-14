<template>
    <div>
    <main>
    <Navigation />
    <div id="form">
       <h1>Fill The Form To Contact Me</h1>
      
       <form
        accept-charset="UTF-8"
        v-on:submit.prevent="onSubmit()"
        method="POST"
       >
        <div>
          <label>First Name: </label><br>

          <input
            type="fName"
            v-model="fName"
            class="text-input"
            placeholder="first name"
            required="required"
          >
        </div>
        <div>
          <label>Last Name: </label><br>
          <input
            type="text"
            v-model="lName"
            class="text-input"
            placeholder="last name"
            required="required"
          >
        </div>

        <section>
            <p>Please select your role:</p>
            <input type="radio" v-model="role" value="professor"><span class="role-input">Professor</span>
            <input type="radio" v-model="role" value="tutor" ><span class="role-input">Tutor</span>
            <input type="radio" v-model="role" value="student"><span class="role-input">Student</span>
            <input type="radio" v-model="role" value="other"><span class="role-input">Other</span>
            <br />
        </section>

        <p>How do you like the website (score from 1-5):</p>
        <select v-model="score" required="required">
        <option disabled value="">Please select one</option>
            <option>5</option>
            <option>4</option>
            <option>3</option>
            <option>2</option>
            <option>1</option>
        </select>

        <div id="comment-container">
          <label>Comments:</label><br>
          <textarea
            type="text"
            v-model="comment"
            class="form-control"
            required="required"
          ></textarea>
        </div>
        <hr>
        <button type="submit">Submit</button>
        <div class="success" v-if="isSuccess">We received your feedback, thank you!</div>

      </form>


    </div>
    </main>
    </div>
</template>

<script>
import axios from "axios";

export default {
  publicPath: './',
  name: "Contact",
//   props: {
//     msg: String
//   },
  head() {
        return {
            title: "contact",
            meta: [
                {
                    hid: "description",
                    name: "decription",
                    content: "contact form"
                }
            ]
        };
  },
  data() {
    return {
      loading: true,
      fName: "",
      lName: "",
      role: "",
      score: "",
      comment: "",
      isSuccess: false,
      isValidated: true,
    };
  },
  methods: {
    onSubmit() {
      let data = {
        fName: this.fName,
        lName: this.lName,
        role: this.role,
        score: this.score,
        comment: this.comment,
      };

      var isValidated = true;
      if (data.fName.length < 2 || data.lName.length < 2) {
        alert('Name should have at least 2 characters');
          isValidated = false;
      };

      if( (!data.fName.match(/^[a-zA-Z]+$/)) || (!data.lName.match(/^[a-zA-Z]+$/))) {
          alert('Names should only have alpha characters');
          isValidated = false;
      };

      if (isValidated){
      axios
        .post("https://comment-receiver.glitch.me/comments", data, {
          headers: {
            Accept: "application/json"
          }
        })
        .then(
          response => {
            this.isSuccess = response.data.success ? true : false;
          },
          response => {
            // Error
          }
        );
      }
    }
  }
};

</script>

<style>
body {
    background: url("../static/multimedia/book-laptop.jpeg") no-repeat center center fixed;
    background-size: cover;
    background-color: #b89090;
    font-family: Verdana, sans-serif;
    font-size: 15px;
}

main {
    width: 1000px;
    padding-left: 30px;
    padding-right: 30px;
    padding-bottom: 30px;
    margin: auto;
    background-color: rgb(245, 219, 216);
}


h1{
    padding-top: 80px;
    padding-bottom: 50px;
}

label{
    font-size: 20px;
}

p{
    font-size: 20px;
}

.text-input{
    margin-top: 40px;
    margin-bottom: 40px;
    font-size: 20px;
}

section{
    margin-top: 20px;
    margin-bottom: 70px;
}

.role-input {
    font-size: 20px;
}

#comment-container{
    margin-top: 70px;
}

#comment-container textarea{
    width: 900px;
    height: 300px;
    font-size: 20px;
}

#submitted{
    text-align: center;
}

.navigation_bar {
    background-color: rgb(245, 219, 216) !important;
}
</style>