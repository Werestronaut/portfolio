<template>
<div class="portframe">
    <div class="blue-box">
        <div class="image-box">
            <div class="frame-box">

            </div>  
        </div>
    </div>
</div>



</template>

<style scoped>

.blue-box{
    background-color: #50a4ff;
    width: 500px;
    height: 500px;
}

.image-box{
    background-color: gray;
    /*background-image: ;*/
    width: 500px;
    height: 500px;
    position: absolute;
    top: 1px;
    left: -15px;

}

.frame-box{
    border: #333333 4px solid;
    position: absolute;
    width: 500px;
    height: 500px;
 
}
</style>

<script>
 export default {
    name: 'PortFrame',
 }
</script>