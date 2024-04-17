<script setup>
import {careerText} from "@/constants/index";
</script>


<template>
    <section id="career">
        <div class="career__inner">
            <h2 class="career__title">
                career <em>참여한 작업</em>
            </h2>
            <div class="career__list">
                <div class="career__box" v-for="(career,key) in careerText" :key="key">
                    <div class="title">{{career.title}}</div>
                    <p class="project">{{career.project}}</p>
                    <div class="adress">- 주소: <a :href="career.adress">{{career.adress}}</a></div>
                    <div class="join">- 참여분야: {{career.join}}</div>
                    <div class="lang">- 적용기술/언어: {{career.lang}}</div>
                    <div class="cont">- 작업내용: {{career.cont}}</div>                
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #career{
        color: var(--white);
        height: 100vh;
    }

    .career__inner{
        width: 100%; height: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        padding: 16px;

        @media (max-width: 800px){
            justify-content: center;
        }        

        .career__title{
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

        .career__list{
            display: flex;
            flex-wrap: wrap;

            .career__box{
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