<template lang="pug">

    transition( appear
                @before-enter="beforeEnter",
                @enter="enter",
                @leave="leave")
        slot


</template>
<style lang="scss">

    //DEFAULT BREAKPOINTS +++++++++++++++++++++++++++++++++++++++++++++++++++++

    /* Helper section for user convenience. Works as note.
    
    */

    //BREAKPOINTS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    //STRUCTURE  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    //BREAKPOINTS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    //DECOR: +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


</style>
<script>

    //*************************************************************************
    // CHILD COMPONENTS IMPORT
    //*************************************************************************


    //*************************************************************************
    // COMPONENT
    //*************************************************************************

    export default {

        //*********************************************************************
        // PROPERTIES
        //*********************************************************************


        //*********************************************************************
        // DATA FIELDS
        //*********************************************************************


        //*********************************************************************
        // COMPUTED FIELDS
        //*********************************************************************


        //*********************************************************************
        // WATCHED FIELDS
        //*********************************************************************


        //*********************************************************************
        // METHODS
        //*********************************************************************

        methods:{
            beforeEnter(el){
                let s = el.style;
                s.position = "absolute";
                s.top= "100%";
            },
            enter(el, done){
                Velocity(el,{
                    top: "-100%",
                },{
                    duration: 15000,
                    easy: [.45,.25,.52,.81]
                },
                )
            },
            leave(){},
        },

        //*********************************************************************
        // LIFE HOOKS
        //*********************************************************************


        //*********************************************************************
        // CHILD COMPONENTS
        //*********************************************************************


    };

</script>