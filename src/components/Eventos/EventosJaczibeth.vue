<template >
    <div class="container">
       <div class="row mt-4">
           <div>
            <h1 class="text-center">MI EJEMPLO</h1>
               <h4 class=" texto mt-2"> DATOS PERSONALES</h4>
              <label class="input-group-text"   far="">Ingresa tu nombre </label>
              <input  class="form-control mt-2" type="text" id="nombre" @change="nombreE">
              <p> El nombre ingresado es: <strong>{{ nombre }}</strong></p>
           </div>
           <div>
                
               <h4 class="texto mt-4" > MIS GUSTOS </h4>
              <label class="input-group-text"   far=""> Cuentame lo que te gusta  </label>
              <input  class="form-control mt-2" type="text" id="gusto" @change="gustoE">
              <p> Tus gustos son: <strong>{{ gusto }}</strong></p> 
           </div>
           <div>
               <button @click="Click" class="btn btn-danger  "  type="button">Ver mas informacion</button>
               <button @click="soyButon" class="btn btn-warning mx-4"  type="button">Guardar</button>
           </div>
       </div>
        </div>
   </template>
   <script>
   export default {
       data(){
           return{
               nombre:'',
               gusto:''
   
           }
           },
       methods:{
           Click(){
               alert("Gracias por darle clic")
           },
           soyButon(){
               alert("soy un boton")
           },
           nombreE(event){
               this.nombre = event.target.value
   
           },
           gustoE(event){
               this.gusto = event.target.value
           }
   
   
       }
   }
   </script>
   
   <style >
.text-center{
    font-family: 'Times New Roman', Times, serif;
    background-color: antiquewhite;
    color: brown;
}
h4{
    font-family: Georgia, 'Times New Roman', Times, serif;
}

.texto{
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    background-color: rgb(144, 209, 255);
    }
</style>