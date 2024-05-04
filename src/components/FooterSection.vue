<template>       
    <footer id="footer" role="contentinfo">
        <div class="footer__inner">
            <div class="footer__text">
                Copyright 2024 salute. All rights reserved.
            </div>            
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @import "@/assets/scss/mixin";

    #footer{         
         font-family: var(--mainKor-font);
         margin-bottom: 40px;
         color: var(--white);
    }

    .footer__inner{
        @include flex-center;
    }
</style>