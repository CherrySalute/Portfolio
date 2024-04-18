<template>
    <section id="self">
        <div class="self__inner">
            <h2 class="self__title">소개글</h2>
            <div class="self__box">                
                <div class="name">김경래</div>
                <div class="basic">Frontend junior</div>
                <div class="tech">사용 기술 : vue.js / javascript / scss / html5 </div>
                <div class="cont">목표 : 많은 사람들이 불편함 없이 이용하고, 즐겁게 편안하게 이용할 수 있는 홈페이지를 만드는 것</div>
                <div class="iam">
                    안녕하세요. 웹퍼블리셔로 시작한지 1년이 넘은 주니어 개발자 김경래입니다.<br>
                     대학 시절 웹 게임에 흥미를 느껴 IT 분야로의 전환을 결심하고, 6개월간 국비 지원 교육을 통해 웹 퍼블리싱을 전문적으로 배웠습니다. 제 첫 직장인 "렌탈프랜드"에서는 웹 페이지 유지보수 및 신규 브랜드 "niccier"의 온라인 판매 페이지 제작을 담당했습니다. 현재는 프론트엔드 개발자로의 경력 전환을 목표로 하여 vue.js를 독학하며 개인 프로젝트를 진행 중입니다. 이러한 경험을 통해 프로젝트에 실질적인 기여를 할 수 있는 역량을 갖추고 있습니다.
                </div>
                <img src="@/assets/img/flower.jpg" alt="flower">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #self{
        color: var(--white);
        padding-top: 10vh;
    }  

    .self__inner{
        width: 100%; height: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        padding: 20px;
        margin-bottom: 50px;
        position: relative;        

        @media (max-width: 800px){
            justify-content: center;
        }

        .self__title{
            font-size: 6vw;
            text-transform: uppercase;
            line-height: 1;
            font-weight: 900;
            white-space: nowrap;
            text-indent: -0.5vw;
            letter-spacing: -0.3vw;
            color: var(--white);

            @media (max-width: 320px){
                display: none;
            }
        }

        .self__box{
            margin-top: 3vw;
            margin-left: 2vw;
    

            .name{
                font-size: 2vw;
                @media (max-width: 800px){
                    font-size: 24px;
                }
            }
            .basic{
                font-size: 1.5vw;
                @media (max-width: 800px){
                    font-size: 20px;
                }
            }
            .tech{
                margin-top: 3vw;      
                @media (max-width: 800px){
                    font-size: 16px;
                }       
            }
            .cont{
                margin-top: 1vw;
                margin-bottom: 2vw;
            }
            .iam{
                padding: 20px;
                width: 1200px;
                margin: 0 auto;
                border: 1px solid white;
                border-radius: 10px;
                line-height: 2;
                @media (max-width: 1200px){
                    width: 100%;
                }
            }

            img{
                width: 50vw;
                position: absolute;
                top: 0; right: 0;
                z-index: -1;
                opacity: 0.5;

                @media (max-width: 800px){
                    width: 300px;
                }
            }
        }
    }
</style>