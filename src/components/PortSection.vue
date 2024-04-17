<script setup>
import {portText} from "@/constants/index";
</script>

<template>
    <section id="port">
        <div class="port__inner">
            <h2 class="port__title">
                Portfolio <em>제작한 작업물</em>
            </h2>
            <div class="port__list">
                <div class="port__box" v-for="(port,key) in portText" :key="key">
                    <div class="title">{{port.title}}</div>
                    <div class="adress"><a :href="port.adress">✨click here</a></div>
                    <div class="cont__box">                        
                        <div class="time">- 제작기간: {{port.time}}</div>
                        <div class="lang">- 적용기술/언어: {{port.lang}}</div>
                        <div class="cont">- 작업내용: {{port.cont}}</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>



<style lang="scss" scoped>
    #port{
        color: var(--white);
        padding-top: 20vh;
    }

    .port__inner{
        width: 100%; height: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        padding: 16px;

        @media (max-width: 800px){
            justify-content: center;
        }        

        .port__title{
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

        .port__list{
            display: flex;
            flex-wrap: wrap;

            .port__box{
                width: calc(100% / 3 - 20px); height: 40vh;
                border: 1px solid var(--white);
                border-radius: 20px;
                padding: 20px;
                margin: 30px 10px;
                transition: all 0.3s ease-out;

                .title{
                    font-size: 3vw;
                    font-weight: 700;

                    @media (max-width: 800px){
                        font-size: 24px;
                        margin-bottom: 10px;
                    }  
                }

                .adress{
                    font-weight: 500;

                    a:hover{
                        color: #a7272e;
                    }
                }

                .cont__box{
                    margin-top: 2vh;
                    padding-left: 1vw;
                }

                &:hover{
                    transform: translateY(-20px);
                }

                @media (max-width: 800px){
                    width: calc(100% / 2 - 20px);
                }  

                @media (max-width: 500px){
                    width: 100%; height: 100%;
                    margin: 20px 10px;
                }
            }
        }
    }
</style>