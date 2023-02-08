<template>
  <div class="window-body">
    
    <section class="grid-1">
      <div class='title'>
        <h2 > <u> Avi Bhadore </u></h2>
        <p id="intro">Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, asperiores! Inventore ut earum, aperiam commodi natus veniam fuga animi eaque molestiae eum voluptatum quae in blanditiis dicta minus totam debitis temporibus cupiditate quis. Autem ab eius cumque eos quod deleniti odit quia eveniet incidunt sit officia esse ad tempora, at est reprehenderit alias qui temporibus animi, neque sunt! Fugit itaque distinctio, odio tempore obcaecati voluptate repellat nisi consequuntur provident nulla amet fugiat expedita sapiente consequatur dignissimos autem, porro nihil odit minus perspiciatis delectus, aliquam harum! Et ullam nisi expedita, vel eum est ipsum placeat maxime laudantium minus possimus saepe illum eaque iusto fugiat, quasi debitis commodi itaque officia quas id! Adipisci id a minus sint in excepturi laudantium sed? Architecto ut incidunt atque perferendis, eligendi iure voluptatem delectus dignissimos. Dolor asperiores quam harum quidem rem eius rerum quae ex et error vel, repellat autem aliquid illum. Consectetur quo accusantium harum!</p>
      </div>
      <div class='img'>
        <!-- <img  class='img' src="../assets/ansi.jpg"> -->  
        <img class='img' src="../assets/unedited-me.svg">
        <div v-html="html"> </div>
        <p> <i>  poggy woggy time is all the time </i> </p>
      </div>
      

      <!-- row 2-->
      <div class="links">
        <h4> <u> Links </u> </h4>
        <ul class="linklist">
            <li> amogus </li>
            <li> pogus </li>
            <li> what the dog doin </li>
            <li> he got that dog in him</li>
        </ul>
      </div>
      <div class="routes">
          <button>
        <router-link to="/">Home</router-link>
      </button>
      <button>
      <router-link to="/about">About</router-link>
      </button>
      </div>
    </section>

  </div>
</template>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.grid-1 {

display: grid;
grid-template-columns: [marginleft] 0.5vw [first] 10vw [second] 10vw [third] 10vw [fourth] 10vw [fifth] 10vw [marginright] 4.5vw  ;
grid-template-rows: auto auto auto;
grid-gap: 10px;
}
.title{
  grid-column-start: first;
  grid-column-end: fifth;
  grid-row-start: 1;
}
#intro{
  font-size: large;
}
.img{
  background-color: red;
  grid-row-start: 1;
  grid-column-start: fifth;
  max-width: 15vw;
  max-height: 14vw ;
}
.links{
  grid-row-start: 2;
  grid-column-start: first;
  grid-column-end: third;
}
.linklist{
  font-size: large;
}
.routes{
  grid-row-start: 2;
  grid-column-start: second;
  height: 100px;
  width: 200px;
}
</style>

<!--
  Resources:
  [quickstart] https://webdesign.tutsplus.com/tutorials/css-grid-layout-quick-start-guide--cms-27238
  [extensive] https://css-tricks.com/snippets/css/complete-guide-grid/
-->

<script>
export default {
  name: 'HomePage',
  props: {
    msg: String
  },
  data(){
    return {
      html: ''
    }
  }
}
</script>