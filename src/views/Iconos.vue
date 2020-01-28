<template>
    <div>
        <b-container class="mt-5">
            <b-row>
                <b-col md="8">
                    <h2>Iconos</h2>
                    <p>Ahora BootstrapVue nos proporciona más de 300 iconos para utilizar en nuestros proyectos. Estos iconos son SVGs que son de facil manipulación y funcionan en cualquier proyecto. </p>
                </b-col>
                <b-col md="4">
                    <b-card>
                        <b-card-body class="text-center">
                            <b-icon icon="bar-chart-fill" font-scale="3"></b-icon>
                            <b-icon icon="camera" font-scale="3"></b-icon>
                            <b-icon icon="alert-circle" font-scale="3"></b-icon>
                            <b-icon icon="bell" font-scale="3"></b-icon>
                            <b-icon icon="person-fill" font-scale="3"></b-icon>
                        </b-card-body>
                    </b-card>
                </b-col>

                <b-col cols="12" class="mt-4">
                    <b-container class="d-flex justify-content-around align-items-center">
                        <h2 class="p-5 rounded-circle bg-light border border-info  ">Uso</h2>
                        <p class="pl-2" style="font-size:24px">BootstrapVue ofrece 2 manera de utilizar los iconos.</p>
                    </b-container>

                </b-col>

            <b-row class="d-flex justify-content-right align-items-center border mt-5 p-3 text-center">

        <!-- Primer Metodo -->
                <b-col md="3" class="my-2">
                        <h4>1 - Utilizando el componente individual</h4>
                        <p>Consiste en colocar el nombre del icono como parte de la etiqueta.</p>
                </b-col>

                <b-col md="6" class="my-2 text-left">
                    <kbd  class="d-block p-4">
                        <code style="font-size:14px">
                            &lt;template><br>
                                &lt;div><br>
                                &lt;b-icon-arrow-up> &lt;/b-icon-arrow-up> <br>
                                &lt;b-icon-alert-triangle-fill> &lt;/b-icon-alert-triangle-fill><br>
                                &lt;/div><br>
                            &lt;/template>
                        </code>
                    </kbd>
                </b-col>

                <b-col md="3" class="my-2">
                       <h4>Resultado:</h4>  
                        <b-icon-arrow-up font-scale="3"></b-icon-arrow-up>
                        <b-icon-alert-triangle-fill font-scale="3"> </b-icon-alert-triangle-fill>
                </b-col>
        <!-- Primer Metodo -->

        <!-- Segundo metodo -->

                <b-col md="3" class="my-2">
                        <h4>2 - Utilizando el componente  b-icon</h4>
                        <p>En este metodo se utilizan las etiquetas <code>b-icon</code>  y dentro del atributo "icon" el nombre del icono.</p>
                </b-col>

                <b-col md="6" class="my-2 text-left ">
                    <kbd  class="d-block p-4">
                        <code style="font-size:14px">
                            &lt;template><br>
                            &lt;div><br>
                                &lt;b-icon icon="arrow-up">&lt;/b-icon> <br>
                                &lt;b-icon icon="alert-triangle">&lt;/b-icon><br>
                            &lt;/div><br>
                            &lt;/template>
                        </code>
                    </kbd>
                </b-col>

                 <b-col md="3" class="my-2">
                       <h4>Resultado:</h4>  
                            <b-icon icon="arrow-up" font-scale="3"></b-icon>
                            <b-icon icon="alert-triangle" font-scale="3"></b-icon>
                </b-col>

        <!-- Segundo metodo -->


            </b-row>

              
              

            </b-row>
        </b-container>
    </div>
</template>