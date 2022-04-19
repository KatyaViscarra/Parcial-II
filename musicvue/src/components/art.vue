<template>
     <b-table striped hover :items="artes" :fields="fields"></b-table>

</template>

<script>
import axios from 'axios'

export default {
    name: 'art',
    data(){
        return{
            artes:[],

        }
    },
    created(){
        axios.get('https://api-crud-example.herokuapp.com/Employee/read')
        .then(response=>{
            this.artes = response.data
            console.log(response.data)
        })
        .catch(e=>{
            this.errors.push(e)
        })
    }   
}
</script>