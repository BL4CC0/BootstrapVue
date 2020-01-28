<template>
  <div>
      <form>
        <b-row class="mt-5">

          <b-col cols="12">
              <h1>Formulario de contacto</h1>
              <b-form-input type="text" v-model="texto" :state="chequear" placeholder="Nombre"></b-form-input>
              <small>Minimo 3 carácteres</small>
          
          </b-col>


          <b-col cols="6">
            <b-form-select v-model="selected" :options="options" :state="chequearSelect"></b-form-select>
            <small>Seleccionado : {{selected}}</small>
          </b-col>

          <b-col cols="6">

            <b-form-radio-group v-model="radio" :options="options2"></b-form-radio-group>
            <small>Seleccionado : {{radio}}</small>

          </b-col>
          <b-col cols="6">

            <b-form-checkbox-group v-model="checkbox" :options="options2"></b-form-checkbox-group>
            <small>Seleccionado : {{checkbox}}</small>

          </b-col>

        </b-row>
      </form>
  </div>
</template>

<script>
export default {
  name:"Form",
  data(){
    return{
      texto:"",

      selected:null,
      options:[
        {value:"null", text:"Animal Preferido"},
        {value:"Perros", text:"Prefiero los perros"},
        {value:"Gatos", text:"Prefiero los Gatos"},
        {value:"Conejos", text:"Prefiero los Conejos"}
        ],

        radio:"",
         options2:[
        {value:"Perros", text:"Perros"},
        {value:"Gatos", text:"Gatos"},
        {value:"Conejos", text:"Conejos"}
        ],

        checkbox:[],
        options2:[
        {value:"Perros", text:"Perros"},
        {value:"Gatos", text:"Gatos"},
        {value:"Conejos", text:"Conejos"}
        ],
        


    }
  },
  computed:{
    chequear(){
      return this.texto.length > 2 ? true : false
    },
    chequearSelect(){
      return this.selected != null ? true : false
    }
  }
}
</script>
