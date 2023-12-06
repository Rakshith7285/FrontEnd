<template>
    

    <div  :class="mobile.availability ? 'green': 'red' ">

                        <h2>{{mobile.brand}}</h2>
                        <h4> {{mobile.model}}</h4>
                        <h4> {{mobile.price}}</h4>
                        <h4> {{mobile.storage}}</h4>
                        <h4> {{mobile.color}}</h4>
                        <h4> {{mobile.availability}}</h4>
    </div>
</template>

<script>

export default{
    name: 'SingleMobile',
    props:{
        mobile: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}

h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>