<template>
    <div>
        <b-jumbotron>
            
            <h1 variant="primary" class="titulo">Experiencia</h1>
            <hr>
            <b-container>
                <b-row>
                    <b-col md="4" v-for="(project, index) in proyectos" :key="project.index">
                        <b-card                            
                            v-bind:img-src="project.images.img1"
                            img-alt="Image"
                            img-top
                            tag="article"
                            style="max-width: 20rem;"
                            class="mb-2"
                        >
                            <h4 class="card-title">{{ project.nombre }}</h4>
                            
                            <b-card-text class="cortar">                              
                                {{ project.descripcion }}
                            </b-card-text>
                            <b-card-text>
                                <strong><em>"{{ project.lenguajes }}"</em></strong>
                                <br>
                                A&ntilde;o: {{ project.anio }}
                            </b-card-text>
                            <p class="text-left">
                                
                                <ol>
                                    <div class="col-md-6">
                                        <li v-for="link in project.links" :key="link.id">
                                            <a v-bind:href="link" >Ver Site</a>
                                        </li>
                                    </div>
                                </ol>
                                
                            </p>
                            <b-button v-b-modal.modallg variant="primary" @click="getExp( index )"> <i class="search"></i>  Ver mas</b-button>
                            
                        </b-card>
                    </b-col>
                </b-row>
            </b-container>
            
        </b-jumbotron>

        <b-modal id="modallg" size="lg" title="Large Modal">
            <div>
                <b-carousel
                    id="carousel-no-anim"
                    style="text-shadow: 0px 0px 2px #000"
                    no-animation
                    indicators
                    img-width="1024"
                    img-height="480"
                >
                    <b-carousel-slide caption="" 
                        v-for="image in objProyecto.images"
                        :key="image.id"
                        :img-src="image" 
                    />
                </b-carousel>
                
                <h5 class="mt-2 justify">
                    <strong>Nombre del proyecto: <small>{{ objProyecto.nombre }}</small> - <small>{{ objProyecto.anio }}</small></strong>
                </h5>
                <p class="mt-3 justify">
                    Descripcion: {{ objProyecto.descripcion }}
                </p>

            </div>
        </b-modal>
        
    </div>
</template>

<script>
import axios from 'axios';

export default {
    name:'ExperienciaComponent',
    data(){
        return {
            proyectos:[],
            objProyecto:{}
        }
    },

    methods:{
        getExperiencia(){
            axios.get(`https://gag-429cc.firebaseio.com/experiencia/.json`)
                .then( (resp)=>{
                    this.proyectos = resp.data;
                    
                })
                .catch( err => console.log( err ) );
        },
        getExp( proyecto ){
            
            axios.get(`https://gag-429cc.firebaseio.com/experiencia/${ proyecto }/.json`)
                .then( (resp)=>{
                    this.objProyecto = resp.data;
                    console.log( resp.data );
                })
                .catch( err => console.log( err ) );
        }
    },
    
    created(){
      this.getExperiencia();
    }
}
</script>

<style scoped>
    .titulo{
        font-family: 'Roboto', sans-serif;
    }

    .col{
        width: 100%;
    }

    .cortar{
        
        height:20px;
        padding:20px;
        text-overflow:ellipsis;
        white-space:nowrap; 
        overflow:hidden;
        -webkit-transition: all 1s;
        -moz-transition: all 1s;
        transition: all 1s;
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box;
    }
</style>
