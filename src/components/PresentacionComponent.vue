<template>
    <div>
        <div class="portada" style="padding-bottom:10em">
            <b-card-text>
                <br><br>
                <h1 class="titulo">Ingeniero en Informatica</h1>
                <h3 class="titulo">Eduard Eddy Acevedo Bracho</h3>
                <b-img rounded="circle"
                    center 
                    src="https://media.licdn.com/dms/image/C4E03AQHn6EvBTHhv5g/profile-displayphoto-shrink_200_200/0?e=1557360000&v=beta&t=XtX443OckeHrjeUqXHblnObdaEIVVCV1-wkp2P7cvaY" 
                    alt="Center image" 
                />
                <p class="presentacion"><strong>Email:</strong> eduardeddyacevedo@gmail.com</p>
                <p class="presentacion"><Strong>Whats App:</Strong> (+58412) 6520309</p>
                <p class="presentacion"><strong>Skype:</strong> eduard-acevedo</p>
            </b-card-text>
        </div>
    </div>
</template>

<script>
export default {
    name:'PresentacionComponent'
}
</script>
<style scoped>
    p{
        -webkit-animation: fadein 2s; /* Safari, Chrome and Opera > 12.1 */
        -moz-animation: fadein 2s; /* Firefox < 16 */
        -ms-animation: fadein 2s; /* Internet Explorer */
        -o-animation: fadein 2s; /* Opera < 12.1 */
        animation: fadein 2s;
    }

    @keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }

    /* Firefox < 16 */
    @-moz-keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }

    /* Safari, Chrome and Opera > 12.1 */
    @-webkit-keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }

    /* Internet Explorer */
    @-ms-keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }

    /* Opera < 12.1 */
    @-o-keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }

    .titulo{
        font-family: 'ZCOOL QingKe HuangYou', cursive;
        color:white;
    }

    .presentacion{
        /*font-family: 'PT Serif', serif;*/
        font-family: 'Roboto', sans-serif;
        color:white;
    }

    .portada{
        /*background: url(https://www.piensasolutions.com/blog/wp-content/uploads/2017/10/banner-programacion.jpg) no-repeat fixed center;*/
        background: url(https://firebasestorage.googleapis.com/v0/b/gag-429cc.appspot.com/o/imagen_cv%2Fpresentacion.jpg?alt=media&token=18229708-f7b5-44ac-8efb-d77effd77163) no-repeat fixed center;
        -webkit-background-size: cover;
        -moz-background-size: cover;
        -o-background-size: cover;
        background-size: cover;
        height: 30%;
        /*width: 100% ;*/
        text-align: center;

    }
</style>
