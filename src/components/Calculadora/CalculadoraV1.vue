<script> 
export default{
    data(){
        return{
            numero1:0,
            numero2:0,
            resultado:0,

        }
    },
    methods:{
        sumar() {
            this.resultado=parseFloat(this.numero1) + parseFloat(this.numero2);
        },
        restar() {
            this.resultado=parseFloat(this.numero1) - parseFloat(this.numero2);
        },
        dividir() {
            this.resultado=parseFloat(this.numero1) / parseFloat(this.numero2);
        },
        multiplicar() {
            this.resultado=parseFloat(this.numero1) * parseFloat(this.numero2);

        },
    }
}
</script>
<template>
    <div class="container mt-5">
        <div class="card shadow p-4">   
            <h1 class="text-center">  CalculadoraV1 </h1>
            <div class="mb-3">
                <label for=""> Numero 1</label>
                <input type="number" class="form-control" v-model="numero1">
            </div>
            <div class="mb-3">
                <label for=""> Numero 2</label>
                <input type="number" class="form-control" v-model="numero2">
            </div>
            <div class="d-flex justify-content-center gap-2">
            <button @click="sumar" class="btn btn-danger"> Sumar  </button>
            <button @click="restar" class="btn btn-warning"> Restar  </button>
            <button @click="dividir" class="btn btn-success"> Dividir  </button>
            <button @click="multiplicar" class="btn btn-info"> Multiplicar </button>
        </div>
        <h2 class=" text-center mt-4">Resultado:{{ resultado }}  </h2>
        </div>
    </div>
</template>