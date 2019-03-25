<template>
    <div>
        <div class="jumbo">
            <h2 class="titulo">
               <strong>Back-End</strong>
            </h2>
            <b-card-group deck class="p-5">
                <b-container>
                    <b-row>
                        <b-col>
                            <b-card
                                border-variant="primary"
                                header="PHP"
                                header-bg-variant="primary"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/php.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valuePhp" :max="max" show-value class="mb-3" />
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="danger"
                                header="Laravel"
                                header-bg-variant="danger"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/laravel.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueLav" :max="max" show-value class="mb-3" variant="danger"/>
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="success"
                                header="NodeJs"
                                header-bg-variant="success"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/Nodejs.svg" 
                                    alt="Image 3" />
                                <br><br>
                                <b-card-text>
                                    <b-progress :value="valueNode" :max="max" show-value class="mb-3" variant="success"/>
                                </b-card-text>
                            </b-card>
                        </b-col>
                    </b-row>
                </b-container>
            </b-card-group>

            <h2 class="titulo">
               <strong>Front-End</strong>
            </h2>
            <b-card-group deck class="p-5">
                <b-container>
                    <b-row>
                        <b-col>
                            <b-card
                                border-variant="danger"
                                header="Angular"
                                header-bg-variant="danger"
                                header-text-variant="white"
                                align="center"
                                class="card"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/angular.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueAng" :max="max" show-value class="mb-3" variant="danger"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="success"
                                header="Vue Js"
                                header-bg-variant="success"
                                header-text-variant="white"
                                align="center"
                                class="card"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/vue.jpeg" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueVue" :max="max" show-value class="mb-3" variant="success"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="primary"
                                header="JQuery"
                                header-bg-variant="primary"
                                header-text-variant="white"
                                align="center"
                                class="card"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/jquery.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueJq" :max="max" show-value class="mb-3"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="warning"
                                header="JavaScript"
                                header-bg-variant="warning"
                                header-text-variant="white"
                                align="center"
                                class="card"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/javascript.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueJs" :max="max" show-value class="mb-3" variant="warning"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>
                    </b-row>
                </b-container>
            </b-card-group>

            <h2 class="titulo">
               <strong>Bases de Datos</strong>
            </h2>
            <b-card-group deck class="p-5">
                <b-container>
                    <b-row>
                        <b-col>
                            <b-card
                                border-variant="primary"
                                header="Mysql"
                                header-bg-variant="primary"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/mysql.jpg" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueMsql" :max="max" show-value class="mb-3"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="danger"
                                header="SQL Server"
                                header-bg-variant="danger"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/sql_server.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueSqlS" :max="max" show-value class="mb-3" variant="danger"/>
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="info"
                                header="Postgre SQL"
                                header-bg-variant="info"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/postgresql.jpg" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valuePosg" :max="max" show-value class="mb-3" variant="info"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="success"
                                header="Mongo DB"
                                header-bg-variant="success"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/mongodb.png"
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueMongo" :max="max" show-value class="mb-3" variant="success"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>
                    </b-row>
                </b-container>
            </b-card-group>

            <h2 class="titulo">
               <strong>App (Hibrida) - CSS - Control de Versiones</strong>
            </h2>
            <b-card-group deck class="p-5">
                <b-container>
                    <b-row>
                        <b-col>
                            <b-card
                                border-variant="primary"
                                header="IONIC"
                                header-bg-variant="primary"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/ionic.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueIonic" :max="max" show-value class="mb-3"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="info"
                                header="Bootstrap"
                                header-bg-variant="info"
                                header-text-variant="white"
                                align="center"
                            >
                                <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/bootstrap.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueBoots" :max="max" show-value class="mb-3" variant="info"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>

                        <b-col>
                            <b-card
                                border-variant="danger"
                                header="GIT"
                                header-bg-variant="danger"
                                header-text-variant="white"
                                align="center"
                            >
                            <img thumbnail 
                                    fluid 
                                    width="150"
                                    src="@/assets/logos/git.png" 
                                    alt="Image 3" />
                                    <br><br>
                                <b-card-text>
                                    <b-progress :value="valueGit" :max="max" show-value class="mb-3" variant="danger"/> 
                                </b-card-text>
                            </b-card>
                        </b-col>
                    </b-row>
                </b-container>
            </b-card-group>
        </div>
    </div>
</template>
<script>
export default {
    name:'SkilsComponent',
     data() {
      return {
        max: 100,
        
        valuePhp: 95,
        valueLav:95,
        valueNode:85,
        
        valueAng:80,
        valueVue:75,
        valueJq:85,
        valueJs:85,

        valueMsql:95,
        valueSqlS:90,
        valueMongo:80,
        valuePosg:80,

        valueIonic:80,
        valueBoots:90,
        valueGit:80
      }
    }
}
</script>

<style scoped>
    titulo{
        font-family: 'Josefin Sans', sans-serif;
        font-size: 2.3em;
    }

    .card{
        height: 19em;
    }

    .jumbo{
        background-color: #e9ecef;
        padding-top: 2rem;
    }
</style>
