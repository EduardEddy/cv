<template>
    <div>
        <b-jumbotron>
            
            <h1 variant="primary" class="titulo">Experiencia</h1>
            <hr>
            <b-container>
                <b-row>
                    <b-col>
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
                            
                            <b-button v-b-modal.modallg variant="primary">lg modal</b-button>
                            
                        </b-card>
                    </b-col>

                    <b-col>
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

                    <b-col>
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
                </b-row>
            </b-container>
            
        </b-jumbotron>

        <b-modal id="modallg" size="lg" title="Large Modal">
            Hello Large Modal!
        </b-modal>
    </div>
</template>

<script>
export default {
    name:'ExperienciaComponent'    
}
</script>

<style scoped>
    .titulo{
        font-family: 'Roboto', sans-serif;
    }
</style>
