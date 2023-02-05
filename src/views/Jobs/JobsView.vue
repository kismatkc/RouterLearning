<template>
  <h1>jobs</h1>
  <div v-for = "job in jobs" :key='job.id' class="job">
  <router-link :to=" {name: 'JobDetails' , params: {id: job.id}} ">
    <h2>{{ job.title }} </h2>
</router-link>
  </div>
</template>

<script>
export default {
    components: {

    },
data(){
    return{
jobs:[
    {title: 'Designer',id: 5,details: 'lorem'},
    {title: 'Teacher',id: 4,details: 'lorem'},
    {title: 'Pilot',id: 3,details: 'lorem'},
    {title: 'Comedian',id: 2,details: 'lorem'},

]        
    }
}
}
</script>

<style>
.job h2 {
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
}
.job h2:hover {
    background: #ddd;
}
.job a {
    text-decoration: none;
}
</style>