<template>
    <section>
        <div class="marketOnline">

            <div class="marketOnline-ctn">
                <div class="img-ctn">
                    <img src="../assets/img/24.png" alt="">
                </div>
                <div class="text-ctn">
                    <h2>Online Marketing</h2>
                    <p>It is a long established fact a reader will be distracted</p>
                    <ul>
                        <li v-for="(elMarketing, el) in marketingOnline" :key="`el-${el}`">
                            <i class="fas fa-check"></i>
                            <span>{{elMarketing}}</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="marketOnline-ctn">
                <div class="img-ctn">
                    <img src="../assets/img/24.png" alt="">
                </div>
                <div class="text-ctn">
                    <h2>Online Marketing</h2>
                    <p>It is a long established fact a reader will be distracted</p>
                    <ul>
                        <li v-for="(elMarketing, el) in marketingOnline" :key="`el-${el}`">
                            <i class="fas fa-check"></i>
                            <span>{{elMarketing}}</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="marketOnline-ctn">
                <div class="img-ctn">
                    <img src="../assets/img/24.png" alt="">
                </div>
                <div class="text-ctn">
                    <h2>Online Marketing</h2>
                    <p>It is a long established fact a reader will be distracted</p>
                    <ul>
                        <li v-for="(elMarketing, el) in marketingOnline" :key="`el-${el}`">
                            <i class="fas fa-check"></i>
                            <span>{{elMarketing}}</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'GridMarketing',
data(){
    return{
        marketingOnline:[
            'SEO',
            'SEM',
            'Web Strategy',
            'Social Management',
        ]
    }
}
}
</script>

<style lang="scss" scoped>
.marketOnline{
    display: flex;
}
 .marketOnline-ctn{
     margin-top: 80px;
     display: flex;
     width: calc(100% / 3);
     margin-right: 20px;
    .img-ctn{
        width: 110px;
        height: 80px;
        img{
            width: 100%;
            height: 100%;
        }
    }
    .text-ctn{
        margin-left: 20px;
        h2{
            font-weight: 500;
        }
        p{
            margin-top: 10px;
            line-height: 25px;
            color: #8e989f;
            font-size: 18px;
        }
        ul{
            list-style: none;
            li{
                margin-top: 20px
            }
            i{
                color: #377dff;
                font-size: 20px;
            }
            span{
                margin-left: 10px;
                font-size: 15px;
                font-weight: 500;
                color: #1e1e1e;
            }
        }
    }
 }
</style>