<template>
<div id="login">
    <section class="container">
        <h1>LOGIN</h1>
        
        <input type="text" placeholder="Usuário">
        <br><br>
        <input type="password" placeholder="Senha">
        <br><br>
        <input class="button" type="button" value="Entrar">
        <br><br>

    </section>
</div>
    
</template>

<script>
export default{
    name:'Login'
}
</script>

<style scoped>
       #login{
        display: flex;
        align-items: center;
        justify-content: center;

    }

    .container{
        display: flex; 
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }


</style>