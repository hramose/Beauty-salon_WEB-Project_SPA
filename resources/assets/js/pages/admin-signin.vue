<template lang="pug">

    layout
        slide.ADMIN-LOGIN-SLIDE
            AdminLoginForm

</template>
<style lang="scss">

    //BREAKPOINTS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    $lgMin:1200px;      $mdMax:1199px;      $smMax:991px;       $xsMax:767px;
                        $mdMin:992px;       $smMin:768px;

    //STRUCTURE  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    //BREAKPOINTS +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    //DECOR: +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

    .ADMIN-LOGIN-SLIDE{
        &>DIV{
            &>DIV{
                vertical-align: middle;
            }
        }
    }

</style>
<script>

    //*************************************************************************
    // CHILD COMPONENTS IMPORT
    //*************************************************************************

    import Layout from "../layouts/admin-login.vue"
    import Slide from "../components/slide.vue"
    import AdminLoginForm from "../components/admin-login-slide/admin-login-form.vue"


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


        //*********************************************************************
        // LIFE HOOKS
        //*********************************************************************


        //*********************************************************************
        // CHILD COMPONENTS
        //*********************************************************************

        components:{
            Layout,
            Slide,
            AdminLoginForm,
        }

    };

</script>