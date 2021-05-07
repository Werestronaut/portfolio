<template>
<div>
<div class="portframe" v-for="project in projects" :key="project.id">
    <div class="blue-box">
        <div class="image-box">
              <v-img :src="project.projectThumb" alt="" style="text-decoration: none;"/>
            <h2>   
                <router-link id="" :to="{name: 'ProjectDetails', params: {
                id: project.id,
                projectTitle: project.projectTitle,
                projectContext: project.projectContext,
                projectCover: project.projectCover,
                projectThumb: project.projectThumb,
                projectLøsning: project.projectLosning,
                projectResultat: project.projectResultat,
                }}">
                {{project.projectTitle}}
            </router-link></h2>
            <div class="frame-box">
                <i class="fas fa-level-up-alt fa-6x"></i>
            </div>  
        </div>
    </div>
    <div>
        <!--
    <div v-for="project in projects" :key="project.id">
            Test:{{project.id}}
            img: {{project.projectCover}}
            <router-link id="" :to="{name: 'ProjectDetails', params: {
                id: project.id,
                projectTitle: project.projectTitle,
                projectDesc: project.projectDesc,
                projectCover: project.projectCover,
                }}">
                {{project.projectTitle}}
            </router-link>

    </div>
    -->
    </div>
</div>
</div>
</template>

<script>
export default {
    name: 'PortFrame',
    data() {
        return {
            projects: [
                {
                    id:1,
                    projectTitle: "7-Kanten Spil",
                    projectContext: "ProjectDesc" ,
                    ProjectThumb: require("../assets/thumbnails/thumb-small-7k.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-7k.jpg"),
                    ProjectLosning: "",
                    ProjectResultat: "",
                },
                 {
                    id:2,
                    projectTitle: "Polaroid Sign-up",
                    projectContext: "ProjectDesc",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-polaroid.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-polaroid.jpg"),
                    ProjectLosning:"" ,
                    ProjectResultat:"" ,
                },
                {
                    id:3,
                    projectTitle: "Adastra Merch Koncept",
                    projectContext: "Efter at have færdiggjort at læse Adastra, fik jeg inspirationen til at lave et merchandise koncept for spillet. Deres nuværende merchandise for spillet passer godt til målgruppen, men for folk som er mere fashion orienteret eller vil være mere ”low-key” med deres support kunne godt dækkes.",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-adastra.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-adastra.jpg"),
                    ProjectLosning:"",
                    ProjectResultat:"" ,  
                },
                {
                    id:4,
                    projectTitle: "Allinkpop Ad",
                    projectContext: "ProjectDesc",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-aik.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-aik.jpg"),
                    ProjectLosning:"" ,
                    ProjectResultat:"" ,
                },
                {
                    id:5,
                    projectTitle: "EASV Studerende Subpage",
                    projectContext: "ProjectDesc",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-easv.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-easv.jpg"),
                    ProjectLosning:"" ,
                    ProjectResultat:"" ,
                },
                {
                    id:6,
                    projectTitle: "Idea House Logo",
                    projectContext: "ProjectDesc",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-ih.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-ih.jpg"),
                    ProjectLosning:"" ,
                    ProjectResultat:"" ,
                },
                {
                    id:7,
                    projectTitle: "Comet Magazine",
                    projectContext: "ProjectDesc",
                    ProjectThumb: require("../assets/thumbnails/thumb-small-comet.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-comet.jpg"),
                    ProjectLosning:"" ,
                    ProjectResultat:"" ,
                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.blue-box{
    background-color: #50a4ff;
    width: 500px;
    height: 500px;
    position:relative;
    margin-top:150px;

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
         
        
        right: -100px;
        bottom: 80px  
    }    
}

.portframe:hover{
.image-box {
    opacity: 100%;

    i {
        right: -2vh;
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
     z-index:500034;
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
        right: 0vh;
        top: 50.7vh;
    }

    
}



</style>
