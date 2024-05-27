<template>
    <div class="Text justify-content-start">
        <div class="row justify-content-start">
            <div class="col-1"></div>
            <h1 class="col-4 Notofont">{{Title}} │ <a href="col-4"><img src="../assets/icons8-youtube-50.png" alt=""></a></h1>
        </div>

        <div class="row">
            <p v-if="secondTitle" class="offset-2 col-10">{{ secondTitle }}</p>
        </div>

        <div class="row">
            <div class="offset-2 col-10">
                <p v-if="Myli">{{ Myli }}</p>  <!-- 這裡加上 v-if -->
                <a class="v-card v-card--flat v-card--link v-theme--light v-card--border bg-surface-light v-card--density-default v-card--rounded v-card--variant-elevated d-inline-flex flex-child-1 position-relative pa-2 mb-4" style="width: 360px;" href="https://twitter.com/vuetifyjs" rel="noopener" target="_blank"><!---->
                    <div class="v-card__loader">
                        <div class="v-progress-linear v-theme--light v-locale--is-ltr" style="top: 0px; height: 0px; --v-progress-linear-height: 2px;" role="progressbar" aria-hidden="true" aria-valuemin="0" aria-valuemax="100">
                            <div class="v-progress-linear__background"></div>
                            <div class="v-progress-linear__buffer" style="width: 0%;"></div>
                            <div class="v-progress-linear__indeterminate">
                                <div class="v-progress-linear__indeterminate long"></div>
                                <div class="v-progress-linear__indeterminate short"></div>
                            </div>
                        </div>
                    </div>
                    <div class="v-lazy" style="width: 100%;">
                        <div class="d-flex ga-4">
                            <div class="v-responsive v-img rounded-s" style="height: 100px; max-width: 130px; width: 100%;">
                                <div class="v-responsive__sizer" style="padding-bottom: 76.9231%;"></div>
                                <img class="v-img__img v-img__img--cover" style="object-position: right center;" src="https://cdn.cosmicjs.com/d0c9b920-410f-11ee-82b2-d53af1858037-x.png">
                            </div>
                            <div class="d-flex align-start ga-4">
                                <div class="text-caption on-surface-light">Get updates on the latest happenings, release information and more on X (Twitter).</div>
                            </div>
                        </div>
                    </div>
                    <div class="text-uppercase position-absolute ms-auto font-weight-medium on-surface-light" style="right: 12px; bottom: 8px; font-size: 10px;">ads via vuetify</div>
                    <span class="v-card__overlay"></span>
                    <span class="v-card__underlay"></span>
                </a>
            </div>
        </div>
        
    </div>
</template>
  
<script>
    export default {
        name: 'TextBox',
        props: {
            Title: String,
            secondTitle: String,
            Myli: String,
            Myli2: String,
            Myli3: String,
            Myli4: String,
            Myli5: String,
        }
    }
</script>
  
<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@100..900&display=swap');

    .Notofont {
        font-family: "Noto Sans TC", sans-serif;
        font-optical-sizing: auto;
        font-weight: 600;
        font-style: normal;
        color: rgba(255, 255, 255, 0.829) !important;
    }

    .Text {
        padding: 1vh;
        -webkit-box-shadow: 8px 10px 32px -7px rgba(0,0,0,.3);
        box-shadow: 8px 10px 32px -7px rgba(0,0,0,.3);
        background-color: rgba(51, 51, 51, 0.685);
        font-size: 15px;
        font-family: "Microsoft JhengHei", "微軟雅黑", "generic-family";
        font-style: normal;
        color: #ffffff;
        font-weight: bold;
        animation: leftIn 2s ease-in-out 0s 1;
    }

    @keyframes leftIn {
        from {
            transform: translate3d(-5%, 0, 0);
            opacity: 0;
        }
        to {
            transform: none;
            opacity: 1;
        }
    }

    .Text p{
        font-size: 20px;
    }

</style>
  
  
  