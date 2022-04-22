<template>
    <section class="home" id="home">
        <h1><span>Sarah zenati johnson</span>Welcome to my portfolio</h1>
        <h2>Front end developer</h2>
        <div class="scroll">
            <v-icon>mdi-arrow-down</v-icon>
            <span>Scroll</span>
        </div>
    </section>
</template>

<style lang="scss">


    h1{
        display: flex;
    flex-direction: column;
    align-items: center;
        font-size: 6vw;
            span{
     font-size: 1.5vw;
    text-transform: uppercase;
    display: flex;
    justify-content: center;
    }
    }

    h2{
        display: flex;
    justify-content: center;
    text-transform: uppercase;
    font-size: 1.5vw;
    }

.scroll{
    display: flex;
    flex-direction: column;
    text-transform: uppercase;
    align-items: center;
    position: relative;
    top: 8rem;
    span{
        margin-top: 0.7rem;
    }
}

</style>

<script>
export default {
    
}
</script>