<template>
    <div>
        <input type="text" name="email" id="email" placeholder="E-mail"><br>
        <input type="text" name="name" id="name" placeholder="Name"><br>
        <button>Cadastrar</button>
        <h2>{{parametro}}</h2>
    </div>
</template>
<script>

export default{
    created(){
        this.parametro = this.$route.params.id;
    },
    data(){
        return{
            parametro: ""
        }
        
    }
}

</script>