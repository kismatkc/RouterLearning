<template>
  <h1>Job details</h1>
  <p>The job id is {{ id }}</p>

</template>

<script>
export default {
    
    components:{

    },
    props: ['id'],
    data(){
        return{
// id: this.$route.params.id
        }
    }

}
</script>

<style>

</style>