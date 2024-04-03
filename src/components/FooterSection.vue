<template>       
    <footer id="footer" role="contentinfo">
        <div class="footer__inner">
            <div class="footer__text">
                2024 This is portfolio.
            </div>            
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @import "@/assets/scss/mixin";

    #footer{         
         font-family: var(--mainKor-font);
         margin-bottom: 40px;
    }

    .footer__inner{
        @include flex-center;
    }
</style>