<template>
  <div class="home">
    <div class="margin-100">
      <h2>Testing the <b>horizontal</b> timeline</h2>
        <hooper :itemsToShow="5" :infiniteScroll="true" group="group1">
          <slide>
            <p class="month">JAN</p>
          </slide>
          <slide>
            <p class="month">FEB</p>
          </slide>
          <slide>
            <p class="month">MAR</p>
          </slide>
          <slide>
            <p class="month">APR</p>
          </slide>
          <slide>
            <p class="month">MAY</p>
          </slide>
          <slide>
            <p class="month">JUN</p>
          </slide>
          <slide>
            <p class="month">JUL</p>
          </slide>
          <slide>
            <p class="month">AUG</p>
          </slide>
          <slide>
            <p class="month">SEP</p>
          </slide>
          <slide>
            <p class="month">OCT</p>
          </slide>
          <slide>
            <p class="month">NOV</p>
          </slide>
          <slide>
            <p class="month">DEC</p>
          </slide>
        </hooper>
        <hooper :itemsToShow="1" :infiniteScroll="true" group="group1">
          <slide>
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
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
           <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
           <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
           <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
           <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
           <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
          <slide>
            <div class="columns is-multiline">
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
              <div class="column card">card </div>
            </div>
          </slide>
        </hooper>
    </div>
    
    <div class="margin-100">
      <h2>Testing the <b>verical</b> timeline</h2>
        <hooper :itemsToShow="1.5" :vertical="true" style="height: 700px">
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
      return hooper.slideTo(i)
    }
  }
}
</script>

<style>
  .month{
    font-weight: 700;
    font-size: 1rem;
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
