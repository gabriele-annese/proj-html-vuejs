<template>
    <div class="container">
        <div class="left">
            <h2>Get tips tricks on how to skyrocket your sales.</h2>
            <p>Faff about only a quid blower i don't want no agro bleeding chimney pot burke tosser crass nice one boot fanny.!</p>
            <ul class="info-ctn">
                <li class="active">
                    <div class="imgCtn-list">
                        <img src="../assets/img/510.png" alt="">
                    </div>
                    <div class="text-ctn">
                        <h3>Reporting Analysis</h3>
                        <p>{{textAnalysis}}</p>
                    </div>
                </li>
                <li>
                    <div class="imgCtn-list">
                        <img src="../assets/img/511.png" alt="">
                    </div>
                    <div class="text-ctn">
                        <h3>Reporting Analysis</h3>
                        <p>{{textAnalysis}}</p>
                    </div>
                </li>   
            </ul>

        </div>
        <div class="right">
            <div class="img-ctn">
                <img src="../assets/img/509.jpeg" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'Analysis',
data(){
    return{
        textAnalysis: 'It is a long established fact a reader will be distracted by the readable contnt of a page when looking at its layout.'
    }
},
methods:{
    Addstyle(){
        this.document.querySelector(".box").classList.add = "active"   
    }
}
}
</script>

<style lang="scss" scoped>
.container{
    width: 80%;
    margin: 50px auto;
    display: flex;
    padding-top: 50px;
    .left{
        width: 40%;
        h2{
            line-height: 40px;
        }
        p{
            line-height: 25px;
            color: #495057;
            font-weight: 500;
            margin-top: 10px;
        }
        .info-ctn{
            list-style: none;
            li{
                display: flex;
                align-items: center;
                margin-top: 30px;
                cursor: pointer;
                .imgCtn-list{
                    width: 100px;
                    height: 100px;
                    margin-right: 20px;
                    img{
                        width: 100%;
                        height: 100%;
                        object-fit: contain;
                    }
                }
            }
        }
        .active{
            border: 1px solid lightgray;
            padding: 10px 0;
            box-shadow: -10px  10px 5px rgba($color: #1e1e1e, $alpha: .2);
            h3{
                color: #377dff;
            }
        }
    }
    .right{
        width: 60%;
        .img-ctn{
            margin-left: 40px;
        }
    }
}
</style>
