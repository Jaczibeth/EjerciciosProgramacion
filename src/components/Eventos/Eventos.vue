<template >
 <div class="container">
    <div class="row mt-4">
        <div>
            <button @click="Click" class="btn btn-danger"  type="button">Dale Clic</button>
        </div>
       
    </div>
     </div>
</template>
<script>
export default {
    methods:{
        Click(){
            alert("Gracias por darle clic")
        }
    }
}
</script>
<style ></style>