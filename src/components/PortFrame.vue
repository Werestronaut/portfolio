<template>

<div class="portframe">
    <div class="blue-box">
        <h3>Type</h3>
        <div class="image-box">
            <h2>Titel</h2>
            <div class="frame-box">
                <i class="fas fa-level-up-alt fa-6x"></i>
            </div>  
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
.blue-box{
    background-color: #50a4ff;
    width: 500px;
    height: 500px;

    h3 {
        font-size: 600%;
        line-height: 110%;
        font-family: halyard-display,sans-serif;
        font-weight: 600;
        font-style: normal;
        color: #3A3A3A;
        position: absolute;
        transform: rotate(-90deg);
        opacity: 80%;
        right: 43.5vw;
        top: 36vh;
    }    
}

.portframe:hover{
.image-box {
    opacity: 100%;

    i {
        left: 51vh;
    }
}
}


.image-box{
    background-color: #D9D9D9;
    /*background-image: ;*/
    width: 100%;
    height: 100%;
    position: relative;
    top: -2em;
    left: -2em;
    opacity: 80%;
    transition: 300ms;


h2{
    font-size: 300%;
    line-height: 110%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
    position: absolute;
    top: 48vh;
    width: 50vh; 
    line-height: 80%;
}

}

.frame-box{
    border: #333333 4px solid;
    position: relative;
    width: 100%;
    height: 100%;
    top: -2em;
    left: -2em;

    i {
        color: #3A3A3A;
        transform: rotate(90deg);
        transition: 300ms;
        position: absolute;
        left: 49vh;
        top: 56vh;
    }

    
}



</style>

<script>
 export default {
    name: 'PortFrame',
 }
</script>