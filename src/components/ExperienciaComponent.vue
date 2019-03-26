<template>
    <div>
        <b-jumbotron>
            
            <h1 variant="primary" class="titulo">Experiencia</h1>
            <hr>
            <b-container>
                <b-row>
                    <b-col md="4" v-for="project in proyectos" :key="project.index">
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
                            
                            <p>
                                Link: <a v-bind:href="link" v-for="link in project.links" :key="link.id">link</a>
                                
                            </p>
                            <b-button v-b-modal.modallg variant="primary">lg modal</b-button>
                            
                        </b-card>
                    </b-col>

                    <!--b-col md="4">
                        <b-card
                            title="Card Title"
                            img-src="https://picsum.photos/600/300/?image=25"
                            img-alt="Image"
                            img-top
                            tag="article"
                            style="max-width: 20rem;"
                            class="mb-2"
                        >
                            <b-card-text>
                            Some quick example text to build on the card title and make up the bulk of the card's content.
                            </b-card-text>

                            <b-button href="#" variant="primary">Go somewhere</b-button>
                        </b-card>
                    </b-col>

                    <b-col md="4">
                        <b-card
                            title="Card Title"
                            img-src="https://picsum.photos/600/300/?image=25"
                            img-alt="Image"
                            img-top
                            tag="article"
                            style="max-width: 20rem;"
                            class="mb-2"
                        >
                            <b-card-text>
                            Some quick example text to build on the card title and make up the bulk of the card's content.
                            </b-card-text>

                            <b-button href="#" variant="primary">Go somewhere</b-button>
                        </b-card>
                    </b-col-->
                </b-row>
            </b-container>
            
        </b-jumbotron>

        <b-modal id="modallg" size="lg" title="Large Modal">
            Hello Large Modal!
        </b-modal>
    </div>
</template>

<script>
import axios from 'axios';
export default {
    name:'ExperienciaComponent',
    data(){
        return {
            proyectos:[]
        }
    },

    methods:{
        getExperiencia(){
            axios.get(`https://gag-429cc.firebaseio.com/experiencia/.json`)
                .then( (resp)=>{
                    this.proyectos = resp.data;
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
