<template>
    <div>
        <b-navbar toggleable="lg" type="dark" variant="dark">
            

            <b-navbar-toggle target="nav_collapse" />

            <b-collapse is-nav id="nav_collapse">
            

            <!-- Right aligned nav items -->
            <b-navbar-nav class="ml-auto mt-2 mb-2">
                <b-nav-form>
                <!--b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search" />
                <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button-->
                    <a href="#experiencia" class="ancla">Experiencia</a>
                     &nbsp; 
                    <a href="#estudios" class="ancla">Estudios</a>
                     &nbsp; 
                    <a href="#skill" class="ancla">Habilidades</a>
                     &nbsp; 
                    <a href="https://firebasestorage.googleapis.com/v0/b/gag-429cc.appspot.com/o/imagen_cv%2Fcv_Eduard_Acevedo_B_M19.pdf?alt=media&token=e9bf8132-7a68-4541-9a0a-dde520a506b6" target="_blank" class="ancla">Descargar CV</a>
                </b-nav-form>

                <!--b-nav-item-dropdown text="Lang" right><a href="#experiencia">Experiencia</a>
                <b-dropdown-item href="#">EN</b-dropdown-item>
                <b-dropdown-item href="#">ES</b-dropdown-item>
                <b-dropdown-item href="#">RU</b-dropdown-item>
                <b-dropdown-item href="#">FA</b-dropdown-item>
                </b-nav-item-dropdown-->

                <!--b-nav-item-dropdown right>
                
                <template slot="button-content"><em>User</em></template>
                <b-dropdown-item href="#">Profile</b-dropdown-item>
                <b-dropdown-item href="#">Signout</b-dropdown-item>
                </b-nav-item-dropdown-->

            </b-navbar-nav>
            </b-collapse>
        </b-navbar>
        <PresentacionComponent />
        <ExperienciaComponent />
        <EstudiosComponent />
        <SkilsComponent />
    </div>
    
</template>

<script>
import PresentacionComponent from './PresentacionComponent.vue'
import ExperienciaComponent from './ExperienciaComponent.vue'
import EstudiosComponent from './EstudiosComponent.vue'
import SkilsComponent from './SkilsComponent.vue';
export default {
    name:'MainComponent',
    components:{
        PresentacionComponent,
        ExperienciaComponent,
        EstudiosComponent,
        SkilsComponent
    }
}
</script>

<style>
    .ancla{
        color:white;
        margin-right: 1em;
    }

    a:hover { 
        color: white;
    }
</style>
