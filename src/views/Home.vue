<template>
  <div class="home">    
    <div>
      <h2>Testing the <b>vertical</b> timeline</h2>
        <hooper :itemsToShow="2" :vertical="true" style="height: 700px" :infiniteScroll="false">
          <slide v-for="(item, index) in groupByMonth" :key="index">
            <p class="month">{{index}}</p>
            <div class="columns is-multiline">
              <div class="column card" v-for="element in item" :key="element.id">card </div>

            </div>
          </slide>
        </hooper>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';
import _ from 'lodash'
import moment from 'moment'

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
  },
  data:()=>{
    return{
      projects:[
        {id:0, name:'Wix Marketing translations part 2', created_date:"2020-01-06", month:'january'},
        {id:1, name:'Wix Marketing translations part 1', created_date:"2020-01-04",  month:'january'},
        {id:2, name:'Wix Logistics translations', created_date:"2020-02-06",  month:'february'},
        {id:3, name:'Wix RMs translations', created_date:"2019-12-06",  month:'december'},
        {id:4, name:'Wix sss translations', created_date:"2019-12-20",  month:'december'},
        {id:5, name:'Wix RMddds translations', created_date:"2019-12-12",  month:'december'},
        {id:6, name:'Wix RdddMs translations', created_date:"2019-12-06",  month:'december'},
      ]
    }
  },
  computed:{
    groupByMonth: function (){
      return _.groupBy(this.projects, (item)=>{
        return moment(item.created_date).format('MMMM')
      })
    }
  },
  mounted(){
    console.log(moment("2020-01-06T08:54:27.000000Z").format('MMMM'))
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
