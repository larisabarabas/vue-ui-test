<template>
  <div class="home">    
    <div>
      <h2>Testing the <b>vertical</b> timeline</h2>
        <hooper :itemsToShow="2" :vertical="true" style="height: 700px" :infiniteScroll="false">
          <slide>
            <p class="month">JAN</p>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">FEB</p>
              <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
              </div>
          </slide>
          <slide>
            <p class="month">MAR</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">APR</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">MAY</p>
              <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">JUN</p>
              <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">JUL</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">AUG</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">SEP</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">OCT</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">NOV</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <p class="month">DEC</p>
            <div class="columns is-multiline">
                <div class="column card">card </div>
                <div class="column card">card </div>
                <div class="column card">card </div>
            </div>
          </slide>
        </hooper>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';

export default {
  name: 'home',
  components: {
      Hooper,
      Slide
  },
  methods:{
    slideTo(i){
      console.log(i)
      return this.$refs.group1.slideTo(i)
    }
  }
}
</script>

<style>
  .month{
    font-size: 1rem;
    text-align:left;
    padding: 0px 25px;
  }
  .margin-100{
    margin: 100px 0px;
  }
  .card{
      border-radius:5px;
      background-color: white;
      max-width: 285px !important;
      cursor: pointer;
      color: #707070 !important;
      border: 1px solid #ffffff;
      width: 236.61px;
      margin:20px 10px;
  }

  .card-list{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr
  }
</style>
