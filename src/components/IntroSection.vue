<script setup>
import {introText} from "@/constants/index";
</script>

<template>       
    <section id="intro">
        <div class="intro__inner">
            <h2 class="intro__title">
                {{introText.title}}
            </h2>
            <div class="intro__text">
                <div class="text">
                    <div>{{introText.desc}}</div>
                </div>
                <div class="img">
                    <img src="" alt="about">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #intro{
        height: 100vh;
    }

    .intro__inner{
        width: 100%; height: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        padding: 16px;

        @media (max-width: 800px){
            justify-content: center;
        }

        .intro__title{
            font-size: 10vw;
            text-transform: uppercase;
            line-height: 1;
            font-weight: 800;
            white-space: nowrap;
            text-indent: -0.5vw;
            letter-spacing: -0.3vw;
            color: var(--white);

            @media (max-width: 320px){
                display: none;
            }
        }
        .intro__text{
            width: 100%; height: 40vh;
            background-color: var(--white);
            color: var(--black);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            position: relative;

            .text{
                font-size: 3vw;
                line-height: 1;
                font-weight: 900;
                text-transform: uppercase;
                text-decoration: underline;
                text-align: center;
                position: absolute;
                z-index: 100;
                transition: all 0.3s;
                cursor: all-scroll;

                @media (max-width: 800px){
                    font-size: 24px;
                }
            }
            .img{
                position: absolute;
                left: 50%; top: 50%;
                transform: translate(-50%, -50%);
                width: 30vh; height: 30vh;
                border-radius: 50%;
                overflow: hidden;
                filter: grayscale(100%);
                transition: all 0.3s;

                @media (max-width: 320px){
                    width: 20vh; height: 20vh;
                }
            }
            
            &:hover.text{
                opacity: 0;
            }
            &:hover .img{
                filter: grayscale(0);
            }
        }
    }
</style>