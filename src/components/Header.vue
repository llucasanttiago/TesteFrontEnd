<template>
    <section>
        <nav class="container">
            <router-link to="/"><a href="/"><img alt="logo" id="logo" src="../images/icon.png"></a></router-link><br>
            <router-link to="/"> <img v-on:click="openMenu" alt="Abrir menu" id="menu-abrir" src="../images/menu.png"></router-link>
            
            <!--<router-link to="/">Home</router-link> |-->
            <!-- <router-link to="/logar">Logar</router-link> |-->
            <!--<router-link to="/cadastro">Cadastro</router-link>-->
   
        <div v-on:click="closeMenu" id="menu-overlay" v-if="menuActive"></div>

        <div id="menu-items" :class="{active:menuActive}">
            <router-link to="/"><a href="/"><img  alt="logo" id="menu-logo" src="../images/icon.png"></a></router-link>
            <ul>
                <li><router-link to="/">Home</router-link></li>
                <li><router-link to="/logar">Logar</router-link></li>
                <li><router-link to="/cadastro">Cadastro</router-link></li>
            </ul>
        </div>


        </nav>
    </section>

</template>

<script>
export default {
    name: 'Header',
    data(){
        return {
            menuActive: false
        }
    },
    methods:{
        openMenu: function(){
            this.menuActive = true;
        },
        closeMenu: function(){
            this.menuActive = false;
        }
    }

}
</script>

<style scoped>


    section{
        width: 100%;
        height: 80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    nav{
        display: flex;
        justify-content: space-between;
        height: 80px;
        align-items: center;
    }

    #logo{
        width: 150px;
    }

    #menu-abrir{
        width: 30px;
    }

    #menu-overlay{
        position: fixed;
        top:0;
        left:0;
        width: 40%;
        height: 100vh;
        background-color: #000000;
        opacity: 0.8
    }

    #menu-logo{
        margin-top: 30px;
        margin-bottom: 10px;
        width: 110px;
    }

    #menu-items{
        position: fixed;
        top:0;
        right:0;
        background-color: var(--color-background-nav);
        width: 60%;
        height: 100vh;
        display: none;
        flex-direction:column;
        justify-content: flex-start;
        align-items: center;
    }

    #menu-items.active{
        display: flex;
    }

    ul{
        list-style: none;
        text-align: center;
    }

    ul li a{
        color: white;
    }

    ul li{
        margin: 20px 0;
    }

    @media (min-width:700px){
        #menu-button,
        #menu-logo,
        #menu-overlay,
        #menu-abrir{
            display: none;
        }

        #menu-items{
            display: flex;
            position: static;
            height: 80px;
            width: auto;
        }

        ul{
            display: flex;
            flex-direction: row;
            color: black;
            height: 80px;
            align-items: center;
        }

        ul li{
            margin: 0;
            margin-left: 10px;
        }

        ul li a{
        color: black;
        }

        #menu-items{
            background-color: white;
        }
    }
</style>