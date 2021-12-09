<template>
  <header>
        <div class="left-header">
            <div class="img-ctn">
                <img src="../assets/img/logo-2.png" alt="">
            </div>
        </div>
        <div class="left-right">
            <ul>
                <li v-for="(elNav, i) in navBar" :key="`el-${i}`">
                    <a href="/">
                        {{elNav}}
                    </a>
                </li>
                <ul class="search-ctn">
                    <li>
                        <i class="fas fa-search"></i>
                    </li>
                    <li>
                        <div class="cart-ctn">
                            <i class="fas fa-shopping-cart"></i>
                            <div class="notification">
                                <span>10</span>
                            </div>
                        </div>
                    </li>
                </ul>
                <ul class="btn-ctn">
                    <button>
                        Get Started
                    </button>
                </ul>
            </ul>
        </div>
  </header>
</template>

<script>
export default {
name: 'Header',
data(){
    return{
        navBar: [
            'Home',
            'About us',
            'Feature',
            'Testimonials',
            'Contact US'
        ]
    }
}
}
</script>

<style lang="scss" scoped>
    header{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 30px;
        height: 85px;
        position: relative;
        .img-ctn{
            width: 50px;
            height: 50px;
            img{
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }
        ul{
            list-style: none;
            display: flex;
            align-items: center;
            li{
                padding: 0 10px;
                &:hover a{
                    color: #377dff;
                    border-bottom: 2px solid #377dff;
                }
                a{
                    text-decoration: none;
                    font-size: 13px;
                    color: #1e1e1e;
                    font-weight: 500;
                    padding: 10px 0;
                    border-bottom: 2px solid transparent;
                }
            }
            .search-ctn{
                margin-left: 20px;
                i{
                    color: #000;
                    cursor: pointer;
                }
                .cart-ctn{
                    width: 30px;
                    height: 30px;
                    display: flex;
                    align-items: center;
                    position: relative;
                    &:hover .notification{
                        display: block;
                    }
                    .notification{
                        position: absolute;
                        top: -5px;
                        right:  4px;
                        width: 15px;
                        height: 15px;
                        display: none;
                        span{
                            cursor: pointer;
                            color: #fff;
                            background-color: rgba($color: #377dff, $alpha: 0.8);
                            border-radius: 50%;
                            padding: 0 2px;
                            font-weight: 500;
                        }
                    }
                }
            }
            .btn-ctn{
                margin-left: 20px;
                button{
                    padding: 13px 8px;
                    font-weight: 500;
                    cursor: pointer;
                    color: #fff;
                    background-color: #377dff;
                    border: 0;
                    border-radius: 5px;
                    &:hover{
                        background-color: #1e1e1e;
                    }
                }
            }
        }
    }
</style>