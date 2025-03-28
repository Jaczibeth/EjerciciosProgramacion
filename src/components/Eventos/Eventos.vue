<template >
 <div class="container">
    <div class="row mt-4">
        <div>
            <h4> Evento Click</h4>
            <button @click="Click" class="btn btn-danger"  type="button">Dale Clic</button>
            <button @click="soyButon" class="btn btn-warning mx-2"  type="button">Dale Clic 2</button>
        </div>
        <div>
            <h4> Evento Change</h4>
           <label class="input-group-text"   far="">Ingresa tu nombre </label>
           <input  class="form-control mt-2" type="text" id="nombre" @change="nombreE">
           <p> El nombre ingresado es: <strong>{{ nombre }}</strong></p>
        </div>
        
    </div>
     </div>
</template>
<script>
export default {
    data(){
        return{
            nombre:'',
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
    }
}
</script>
<style ></style>