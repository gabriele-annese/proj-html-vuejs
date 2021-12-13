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
                    <li class="search-box">
                        <button type= "submit" class="btn-search">
                             <i class="fas fa-search"></i>
                        </button>
                        <input type="text" class="input-search" placeholder="Cerca">
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
                    <button class="btn">
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
        width: 80%;
        margin: 0 auto;
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
            }
        }
    .search-box{
    width: fit-content;
    height: fit-content;
    position: relative;
    margin-right:  20px;
    }
    .input-search{
    height: 30px;
    width: 30px;
    border-style: none;
    padding: 10px;
    font-size: 18px;
    letter-spacing: 2px;
    outline: none;
    border-radius: 25px;
    transition: all .5s ease-in-out;
    background-color: transparent;
    padding-right: 40px;
    color: #000;
    }
    .input-search::placeholder{
    color: #000;
    font-size: 17px;
    letter-spacing: 2px;
    font-weight: 100;
    }
    .btn-search{
    width: 30px;
    height: 30px;
    border-style: none;
    font-size: 20px;
    font-weight: bold;
    outline: none;
    cursor: pointer;
    position: absolute;
    right: 10px;
    color:#fff;
    background-color:transparent;
    pointer-events: painted;
    }
    .btn-search:focus ~ .input-search{
    width: 300px;
    background-color: transparent;
    border:1px solid rgba($color: #8e989f, $alpha: 1.0);
    border-radius: 20px;
    transition: all 0.5s cubic-bezier(0, 0.110, 0.35, 2);
    }
    .input-search:focus{
    width: 300px;
    background-color: transparent;
    border:1px solid rgba($color: #8e989f, $alpha: 1.0);
    border-radius: 10px;
    transition: all 0.5s cubic-bezier(0, 0.110, 0.35, 2)
    }
    
    }
</style>