<script setup>
import {carrerText} from "@/constants/index";
</script>


<template>
    <section id="carrer">
        <div class="carrer__inner">
            <h2 class="carrer__title">
                Carrer <em>참여한 작업</em>
            </h2>
            <div class="carrer__list">
                <div class="carrer__box" v-for="(carrer,key) in carrerText" :key="key">
                    <div class="title">{{carrer.title}}</div>
                    <p class="project">{{carrer.project}}</p>
                    <div class="adress">- 주소: <a :href="carrer.adress">{{carrer.adress}}</a></div>
                    <div class="join">- 참여분야: {{carrer.join}}</div>
                    <div class="lang">- 적용기술/언어: {{carrer.lang}}</div>
                    <div class="cont">- 작업내용: {{carrer.cont}}</div>                
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #carrer{
        color: var(--white);
        height: 100vh;
    }

    .carrer__inner{
        width: 100%; height: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        padding: 16px;

        @media (max-width: 800px){
            justify-content: center;
        }        

        .carrer__title{
            font-size: 10vw;
            font-weight: 700;
            text-transform: uppercase;
            line-height: 1;
            white-space: nowrap;
            text-indent: -0.5vw;
            letter-spacing: -0.3vw;
            padding-bottom: 10vh;

            em{
                font-size: 3vw;
                font-weight: 400;
            }

            @media (max-width: 800px){
                padding: 5vh 0;
            }   
        }

        .carrer__list{
            display: flex;
            flex-wrap: wrap;

            .carrer__box{
                width: calc(100% / 2 - 20px); height: 30vh;

                .title{
                    font-size: 3vw;
                    padding-bottom: 1vh;
                    font-weight: 700; 

                    @media (max-width: 800px){
                        font-size: 24px;
                    }    
                }

                .project,
                .adress,
                .join,
                .lang,
                .cont{
                    padding-left: 1vw;
                }

                @media (max-width: 800px){
                    width: 100%; height: 25vh;
                }      
            }            
        }
    }
</style>