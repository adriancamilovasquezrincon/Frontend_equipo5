<template>
    <div>
        <h1>
            Buenos dias
        </h1>
        <h2>{{lista}}</h2>
    </div>
</template>
<script>
export default {
    name:"prueba",
    props:{
        msg:String
    },
    data() {
        return {
            casa:"Casa helada"
        }
    },
}
</script>