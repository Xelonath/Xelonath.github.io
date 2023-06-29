<template>
    <div id="grid-wrapper">
        <div id="TopRow">
            <h1>Test</h1>
        </div>
        <div id="LeftSide">

        </div>
        <div id="Content">

        </div>
        <div id="RightSide">

        </div>
        <div id="bottomRow">

        </div>

    </div>
</template>
<script setup lang="ts">

</script>
<style>
    #grid-wrapper{
        display:grid;
        width: 100vw;
        height: 100vh;
        grid-template-rows: 15vh 25vh 25vh 25vh 10vh;
        grid-template-columns: 5vw 90vw 5vw;
        grid-template-areas: 
            "topRow topRow topRow"
            "sideL contentArea sideR"
            "sideL contentArea sideR"
            "sideL contentArea sideR"
            "bottomRow bottomRow bottomRow";
    }
    #TopRow{
        grid-area: topRow;
    }
    #Content{
        grid-area: contentArea;
    }
    #bottomRow{
        grid-area: bottomRow;
    }
    #LeftSide{
        grid-area: sideL;
    }
    #RightSide{
        grid-area: sideR;
    }
</style>