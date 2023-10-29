<script setup>
    import Button from 'primevue/button';
    import {ref} from 'vue';
    const name =ref('click');
    // const name1 = ref('save');
    const handleClick = () =>{
        name.value ='dbclick';
    }
</script>
<template>
    <Button :label="name" @click="handleClick" icon="pi pi-check" rounded /> 
    <Button label="save" icon="pi pi-check" />
    <div class="grid mt-4">
    <div class="col-6 col-offset-3">
        <div class="text-center p-3 border-round-sm bg-primary font-bold">6</div>
    </div>
</div>

<div class="grid ">
    <div class="col-4 ">
        <div class="text-center p-3 border-round-sm bg-primary font-bold">4</div>
    </div>
    <div class="col-4 col-offset-4">
        <div class="text-center p-3 border-round-sm bg-primary font-bold">4</div>
    </div>
</div>
</template>
<style scoped>
    /* .p-button{
        background-color: rgb(255, 0, 212);
        margin: 30px;
    } */
    :deep(.p-button){
        background-color: blueviolet !important;
    }

</style>