<template>
  <div class="hello">
    <div class="row">
        <div class="col-md-6 my-4">
            <div class="animation1"></div>
        </div>

        <div class="col-md-6 my-5 text-dark animation2">
            <h1 class="fw-bolder">Introduction</h1>
            <p class="h6 fw-bold">Hey! My name is Laurentius. I am 18 years old. I graduated from Xaverius Vocational Highschool and a student at Multi Data Palembang University and I'm also working at a company that produce and sells hospital and rehabilitation product. About my hobbies, I don't have much hobbies, but I'm sure you can tell that I watch anime...from the picture on the left, I also watch YouTube videos or playing video game like Valorant</p>
            <hr>
            <h1 class="fw-bolder">Internship</h1>
            <p class="h6 fw-bold">
                <ul>
                    <li>
                        November 2019 - February 2019 at Artha Komputer
                    </li>

                    <li>
                        July 2020 - October 2020 at Chandra Komputer
                    </li>
                </ul>
            </p>
            <hr>
            <h1 class="fw-bolder">Achievement</h1>
            <p class="h6 fw-bold">
                <ul>
                    <li>800 out of 990 TOEIC score</li>
                </ul>
            </p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
