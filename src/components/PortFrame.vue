<template>
<div>
<div class="portframe" v-for="project in projects" :key="project.id">
    <div class="blue-box">
        <div class="image-box">
              <v-img :src="project.projectThumb" alt="" />
            <h2>   
                <router-link id="" :to="{name: 'ProjectDetails', params: {
                id: project.id,
                projectTitle: project.projectTitle,
                projectContext: project.projectContext,
                projectCover: project.projectCover,
                projectThumb: project.projectThumb,
                projectLosning: project.projectLosning,
                projectResultat: project.projectResultat,
                projectLosTit: project.projectLosTit,
                projectLos2: project.projectLos2,
                projectLosTit2: project.projectLosTit2,
                projectLos3: project.projectLos3,
                projectResultatText: project.projectResultatText,
                projectResultatImg: project.projectResultatImg,
                projectResultatImg2: project.projectResultatImg2,
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
                    projectThumb: require("../assets/thumbnails/thumb-small-7k.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-7k.jpg"),
                    projectLosning: "",
                    projectResultat: "",
                },
                 {
                    id:2,
                    projectTitle: "Polaroid Sign-up",
                    projectContext: "Jeg fik en assigment hvor jeg skulle lave en sign-up screen til en app.",
                    projectThumb: require("../assets/thumbnails/thumb-small-polaroid.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-polaroid.jpg"),
                    projectLosning:"Mit koncept var at lave et sign-up screen til en photo gallery app, så som Instagram, men at det skulle være i stil af gamle polaroids hvor man ikke kunne redigere dem. Ud over selve konceptet, så har flowet på opsætningen også sat op med standarden for sign up screens, for at minimere irritationer for brugerens flow." ,
                    projectLosTit: "Polaroid:" ,
                    projectLos2: "Øverst er den en polaroid, som skifter imellem forskellige billeder der er blevet taget af brugerbasen." ,
                    projectLosTit2: "Sign-up knap:" ,
                    projectLos3: "Nederst på siden er sign-up knappen, der er blevet lavet efter en gammeldags polaroid kamera. Dette ville skabe noget brand identitet, samt vil give en sjov detalje for dem der havde en af deres gamle kameraer." ,
                },
                {
                    id:3,
                    projectTitle: "Adastra Merch Koncept",
                    projectContext: "Efter at have færdiggjort at læse Adastra, fik jeg inspirationen til at lave et merchandise koncept for spillet. Deres nuværende merchandise for spillet passer godt til målgruppen, men for folk som er mere fashion orienteret eller vil være mere ”low-key” med deres support kunne godt dækkes.",
                    projectThumb: require("../assets/thumbnails/thumb-small-adastra.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-adastra.jpg"),
                    projectLosning:"Designet er inspireret af 90’s sweatshirt design, samt en illustration fra spillets artist, Haps, hvor en af spillets hovedpersoner Amicus har et outfit inspireret af samme tidsperiode.",
                    projectLosTit: "Front design:" ,
                    projectLos2: "Pil-tegnet er taget fra den imperial families pande symbol. ”Gud wolf” kommer fra den tidligere nævnte illustration, hvor det står på den jakke Amicus har på. " ,
                    projectLosTit2: "Ryg Design:" ,
                    projectLos3: "Citatet er fra en politisktale som Amicus holde i spillet. Her har jeg forsøgt at holde stort fokus på ”Beyond”, da dette er hvad Amicus tilføjer på citatet fra en tidligere kongelig. Dette har jeg gjort ved at gøre ordet større end de andre." ,
                    projectResultatText: "3. Resultat",
                    projectResultatImg:require("../assets/AdastraFB.svg"), 
                    projectResultatImg2:require("../assets/AdastraBB.svg"), 
                },
                {
                    id:4,
                    projectTitle: "Allinkpop Ad",
                    projectContext: "Jeg fik en assignment, hvor vi skulle designe en reklame af et produkt eller virksomhed. Udover dette, skulle vi også finde ud af hvor det bedst ville give mening at kører reklamen.",
                    projectThumb: require("../assets/thumbnails/thumb-small-aik.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-aik.jpg"),
                    projectLosning:"Jeg valgte at lave en reklame for butikken ved navn ”AllinKpop”, som er en butik fra København der specialisere sig i kpop albums og merchandise." ,
                    projectLosTit: "Platform:" ,
                    projectLos2: "Den typiske kpop-fan er typisk hørt af unge og siden de fleste unge bruger mere instagram, giver det mening at tage til denne platform." ,
                    projectLosTit2: "Film stil:" ,
                    projectLos3: "Jeg valgte at gøre det meget simpelt og til pointen. For at sikre at de fleste som er til kpop der bare scroller igennem deres feed vil lægge mærke til det, så havde jeg valgt at vise frem nogle albums, for at skabe et godt førstehånds indtryk. Derefter viser jeg forskellige mængder af album covers, for at vise hvor mange forskellige grupper de egentligt har. For at gøre det endnu mere personligt for seeren, anvender jeg nogle forskellige kpop gruppers fandom navne for at vise noget autenticitet fra steder, så man ved butikken ved noget om kpop kulturen.",
                    projectResultatText: "3. Resultat",
                    projectResultat:"Se det endelige resultat her: https://www.youtube.com/watch?v=aq83xs8094w" ,
                },
                {
                    id:5,
                    projectTitle: "EASV Studerende Subpage",
                    projectContext: "ProjectDesc",
                    projectThumb: require("../assets/thumbnails/thumb-small-easv.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-easv.jpg"),
                    projectLosning:"" ,
                    projectResultat:"" ,
                },
                {
                    id:6,
                    projectTitle: "Idea House Logo",
                    projectContext: "Jeg fik som opgave at lave et logo for EASV’s afdeling ’Idea House’, som havde et forældet logo. De ville gerne have, at Idea House’s nye identitet skulle bygge sig op af EASV’s, for at vise de hører sammen.",
                    projectThumb: require("../assets/thumbnails/thumb-small-ih.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-ih.jpg"),
                    projectLosning:"Jeg fik som opgave at lave et logo for EASV’s afdeling ’Idea House’, som havde et forældet logo. De ville gerne have, at Idea House’s nye identitet skulle bygge sig op af EASV’s, for at vise de hører sammen." ,
                    projectLos2: "Typografien har jeg valgt også at kører meget simpel, for ikke at tage for meget væk fra selve logoet. Derfor valgte jeg ’Coolvetica’ som er en sans serif font, der både giver en moderne sjæl til designet, men også giver det noget robust intelligens. ",
                },
                {
                    id:7,
                    projectTitle: "Comet Magazine",
                    projectContext: "Jeg satte mig ud for at lave et logo til et modeblad, der har et navn med rumtema.",
                    projectThumb: require("../assets/thumbnails/thumb-small-comet.jpg"),
                    projectCover: require("../assets/thumbnails/thumb-big-comet.jpg"),
                    projectLosning: "Processen startede ud med at brainstorme navne, hvilket ende op med at lande på ”Comet”, da jeg kom i tanke på at O’et lignede en komet. Dette ender også op med at blive highlightet af designet og giver logoet et stort statement. " ,
                    projectLos2: "Jeg valgte at gå med en serif font, da det både er en klassiker for det moderelaterede markedet, men giver designet en sofistiskhed og hjælper at grounde designet." ,
                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.portframe{
    display: flex;
    justify-content: center;
}
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
        opacity: 0.8;
         
        
        right: -100px;
        bottom: 80px  
    }    
}

.portframe:hover{
.image-box {
    opacity: 1;

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
    
    position: relative;
    
    line-height: 80%;
    a {
    position: relative;
    bottom: 10vh;
    left: 3vw;
    width: 0vh; 
        color: #3A3A3A;
        text-decoration: none;
    }
}

}

.frame-box{
    border: #333333 4px solid;
    position: absolute;
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
