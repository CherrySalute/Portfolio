<template>
    <section id="self">
        <div class="self__inner">
            <h2 class="self__title">소개글</h2>
            <div class="self__box">                
                <div class="name">김경래</div>
                <div class="basic">Frontend junior</div>
                <div class="tech">사용 기술 : vus.js / javascript/ scss / html5 </div>
                <div class="cont">목표 : 많은 사람들이 불편함 없이 이용하고, 즐겁게 편안하게 이용할 수 있는 홈페이지를 만드는 것</div>
                <div class="iam">
                    안녕하세요. 웹퍼블리셔로 시작한지 1년이 넘은 주니어 개발자 김경래입니다.<br>
                    대학교를 다닐 무렵 그 당시 유행하던 웹게임을 하며 "이런 게임들은 어떻게 만들어질까?" 라는 막연하게 생각을 했습니다. 후에 하던일을 할 수 없는 상황이 되어 다른 직업을 찾던 중 그 때의 기억을 떠올려 6개월간의 국비교육으로 웹퍼블리셔 과정을 수료하게 되었습니다. 처음에는 낯선 코드들이 저를 힘들게 했지만 이제는 누구보다 친하게 지내며 저의 동반자가 되었습니다. 
                    그렇게 저는 첫 직장으로 "렌탈프랜드"에서 퍼블리셔로 입사하여 브랜드가 운영중인 페이지의 유지보수를 맡게 되었고, 새로운 브랜드 "niccier"의 런칭으로 온라인 판매를 위한 페이지를 제작하게 되었습니다. 회사규모상 비록 카페24를 이용하여 총괄로 퍼블리싱을 진행하였습니다.
                    현재는 최종꿈인 Frontend로 진화하기 위해서 vue.js를 독학으로 공부하며 자력으로 프로젝트 하나를 제작중입니다.
                </div>
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
        }
    }
</style>