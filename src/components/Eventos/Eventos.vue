<template >
 <div class="container">
    <div class="row mt-4">
        <div>
            <button @click="Click" class="btn btn-danger"  type="button">Dale Clic</button>
            <button @click="soyButon" class="btn btn-warning mx-2"  type="button">Dale Clic 2</button>
        </div>
       
    </div>
     </div>
</template>
<script>
export default {
    methods:{
        Click(){
            alert("Gracias por darle clic")
        },
        soyButon(){
            alert("soy un boton")
        }
    }
}
</script>
<style ></style>