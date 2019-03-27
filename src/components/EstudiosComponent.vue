<template>
    <div class="container mb-5" id="estudio">
        <h2 variant="primary"><strong> Estudios </strong></h2>
        <br>
        <b-row>
            <b-col cols="2">
                <b-img rounded="circle" 
                    thumbnail 
                    fluid 
                    right
                    width="150"
                    src="https://st2.depositphotos.com/1906711/11469/v/950/depositphotos_114694940-stock-illustration-vector-flat-parchment-icon.jpg" 
                    alt="Image 3" />
            </b-col>
            <b-col cols="10">
                <h3 class="titulo text-left"><strong>T&iacute;tulo:</strong> Ingeniero en Inform&aacute;tica</h3>
                <p class="text-left"><strong>Universidad: </strong> Rafael Belloso Chac&iacute;n</p>
            </b-col>
        </b-row>
        <hr>
        <b-row>
            <b-col cols="9">
                <h3 class="titulo text-right"><strong>Titulo:</strong> T&eacute;cnico Superior Universitario en Inform&aacute;tica</h3>
                <p class="text-right"><strong>Tecnol&oacute;gico: </strong>Pedro Emilio COll</p>
            </b-col>
            <b-col cols="3">
                <b-img rounded="circle" 
                    thumbnail 
                    fluid 
                    left
                    width="150"
                    src="https://st2.depositphotos.com/4384799/8654/v/950/depositphotos_86549956-stock-illustration-diploma-icon-on-white.jpg" 
                    alt="Image 3" />
            </b-col>
        </b-row>
        <hr>
        <h2 variant="primary">
            <strong> Certificados </strong>
        </h2>
        <b-row>
            <b-col cols="2">
                <b-img rounded="circle" 
                    thumbnail 
                    fluid 
                    right
                    width="150"
                    src="https://st2.depositphotos.com/2866255/5752/v/950/depositphotos_57529891-stock-illustration-diploma-flat-icon.jpg" 
                    alt="Image 3" />
            </b-col>
            <b-col cols="10">
                <h3 class="titulo text-left"><strong>Certificado:</strong> WEB Master</h3>
                <p class="text-left">
                    <strong>Universidad: </strong>Rafael Belloso Chac&iacute;n
                </p>
            </b-col>
        </b-row>
    </div>
</template>

<script>
    export default {
        name:'EstudiosComponent'
    }
</script>

<style scoped>
    h2{
        color:blue;
        /*font-family: 'Courgette', cursive;*/
        font-family: 'Josefin Sans', sans-serif;
    }

    .titulo{
        font-family: 'Josefin Sans', sans-serif;
        font-size: 2.3em;
    }

    p{
        font-family: 'Josefin Sans', sans-serif;
        font-size: 1.6em;        
    }
</style>
<!--
    font-family: 'Josefin Sans', sans-serif;
font-family: 'Courgette', cursive;
    -->