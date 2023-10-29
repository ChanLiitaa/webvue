<script setup> 
    import AppHeader from '@/components/header.vue';
    import AppMain from '@/components/main.vue';
    import AppFooter from '@/components/footer.vue';
    import AppSidebar from '@/components/sidebar.vue';

</script>
<template>
   <div class="container">
        <div class="con_left">
            <AppSidebar></AppSidebar>
        </div>
        <div class="con_right">
            <div class="header">
                <AppHeader></AppHeader>
            </div>
            <div class="main">
                <AppMain></AppMain>
            </div>
            <div class="footer">
                <AppFooter></AppFooter>
            </div>
        </div>
        
   </div>
</template>
<style scoped>
    .container{
        width: 100%;
        height: 100vh;
        background-color: aqua;
        display: flex;
        justify-content: center;
    }
    .con_left{
        width: 20%;
        height: 100%;
        background-color: blueviolet;
    }
    .con_right{
        width: 80%;
        height: 100%;
        background-color: rgb(104, 226, 43);
    }
    .header{
        width: 100%;
        height: 20%;
        background-color: brown;
    }
    .main{
        width: 100%;
        height: 60%;
        /* background-color: rgb(92, 89, 92); */
    }
    .footer{
        width: 100%;
        height: 20%;
        background-color: brown;
    }
</style>