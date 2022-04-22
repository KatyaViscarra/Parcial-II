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
        axios.get('http://localhost:8000/api/galleries')
        .then(response=>{
            this.artes = response.data.data
            console.log(response.data)
        })
        .catch(e=>{
            this.errors.push(e)
        })
    }   
}
</script>