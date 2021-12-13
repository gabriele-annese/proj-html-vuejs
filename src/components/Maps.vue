<template>
  <div class="conatiner-maps">
      <div class="text-ctn">
          <h4>Contact whit our team</h4>
          <p>If your are planning on developing a product landing.</p>
      </div>
      <section>
        <div class="maps-ctn">
            <img src="../assets/img/StaticMapService.GetMapIma.png" alt="">
            <div class="card-address">
                <div class="left">
                    <h4>Storey Ave</h4>
                    <p>San Fransisco California 94129</p>
                    <a href="/">Visualizza mappa piú grande</a>
                </div>
                <div class="right">
                    <div class="img-ctn">
                        <img src="../assets/img/Arrow.png" alt="">
                    </div>
                </div>
            </div>
            <div class="point-ctn">
                <img src="../assets/img/pointRed.png" alt="">
            </div>
            <div class="info">
                <span>Dati mappa @2020</span>
                <span>Termini e condizioni d'uso</span>
                <span>Segnala un errore nella mappa</span>
            </div>
            <div class="btn-ctn">
                <div class="zoom">
                    <div class="plus">
                        <i class="fas fa-plus"></i>
                    </div>
                    <div class="minus">
                        <i class="fas fa-minus"></i>
                    </div>
                </div>
            </div>
        </div>
        <div class="info-ctn">
            <div class="brand">
                <img src="../assets/img/35.png" alt="">
            </div>
            <div class="info">
                <h4>9840 Shore St. Found Du Lac, WI 54935</h4>
                <p>0 1223 456 789</p>
                <a href="/">mail@sofboz.com</a>
            </div>
            <div class="info-social">
                <div v-for="(elSocial, i) in socialIcon" :key="`el-${i}`">
                    <i :class="elSocial"></i>
                </div>
            </div>
            <form class="message-ctn">
                <div class="name-ctn">
                    <input type="name" placeholder="Your Name" class="name">
                    <input type="mail" placeholder="Your Email" class="mail">
                </div>
                <div class="message-area">
                    <input type="text"  placeholder="Your Subject" class="text">
                    <textarea name="messaggio" rows="5" cols="30" placeholder="Your Message"></textarea>
                </div>
                <div class="btn-ctn">
                    <button class="btn">
                        Send Message
                    </button>
                </div>
            </form>
        </div>
      </section>
  </div>
</template>

<script>
export default {
    name: 'Maps',
    data(){
        return{
            socialIcon:[
                'fab fa-twitter',
                'fab fa-facebook-f',
                'fab fa-instagram',
                'fab fa-github'
            ]
        }
    }

}
</script>
<style lang="scss" scoped>
.conatiner-maps{
    width: 80%;
    margin: 0 auto;
    .text-ctn{
        text-align: center;
        h4{
            font-size: 20px;
        }
        p{
            color: #495057;
            padding: 20px;
            font-weight: 500;
        }
    }
    section{
        display: flex;
    }
    .maps-ctn{
        width: 50%;
        height: 500px;
        background-color: green;
        position: relative;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .card-address{
            width: 70%;
            background-color: #fff;
            border-radius: 5px;
            position: absolute;
            top: 10px;
            left: 10px;
            padding: 15px 10px;
            display: flex;
            .left{
                width: 50%;
                p{
                padding: 10px 0;
                }
                a{
                    padding: 20px 0;
                    color: #377dff;
                }
            }
            .right{
                width: 50%;
                display: flex;
                justify-content: flex-end;
                align-items: center;
                .img-ctn{
                    width: 80px;
                    height: 80px;
                    margin-right: 30px;
                    img{
                        width: 100%;
                        height: 100%;
                    }
                }
            }
        }
        .point-ctn{
            width: 100px;
            height: 100px;
            position: absolute;
            top: 40%;
            left: 45%;
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }
        .info{
            width: 100%;
            position: absolute;
            bottom: 0;
            right: 0;
            display: flex;
            justify-content: flex-end;
            span{
                border: 1px solid #00000014;
                background: #f2f7ff;
                padding: 0 5px;
                font-weight: bold;
                font-size: 10px;
                cursor: pointer;
            }
        }
        .btn-ctn{
            position: absolute;
            right: 10px;
            bottom: 50px;
            display: flex;
            flex-direction: column;
            .zoom{
                background: #f2f7ff;
                .plus,
                .minus{
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    width: 40px;
                    height: 37px;
                    cursor: pointer;
                    padding: 10px 0;
                    i{
                        color: #495057;
                        font-size: 23px;
                    }
                }
                .plus{
                    border-bottom: 1px solid #000;
                }
            }

        }
    }
    .info-ctn{
        width: 50%;
        padding: 0 20px;
        .info{
            padding: 20px 0;
            p{
                color: #495057;
                padding: 10px 5px;
                cursor: pointer;
                font-weight: 500;
            }
            a{
                color: #495057;
                text-decoration: none;
                font-weight: 500;
                &:hover,
                &:focus{
                    text-decoration: underline;
                }
            }
        }
    .info-social{
        display: flex;
        div{
            width: 30px;
            height: 30px;
            border: 1px solid #f2f7ff;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 3px;
            i{
            cursor: pointer; 
            padding: 0 10px;
            color: #377dff;
            }
        }
    }
    .message-ctn{
        display: flex;
        flex-direction: column;
        .name-ctn{
            display: flex;
            padding: 10px 0;
                input{
                  margin-right: 10px;
                  outline: none;
                  padding: 8px 5px;
                  border: 1px solid #f2f7ff;
                  border-radius: 5px;
                &:focus{
                    border: 1px solid #495057;
                }
                &::placeholder{
                    color: #495057;
                    font-weight: 500;
                    font-size: 16px;
                }
                }
        }
        .message-area{
            display: flex;
            flex-direction: column;
            input,
            textarea{
                margin-right: 10px;
                outline: none;
                padding: 8px 5px;
                border: 1px solid #f2f7ff;
                margin-bottom: 10px;
                border-radius: 5px;
                &:focus{
                    border: 1px solid #495057;
                }
                &::placeholder{
                    color: #495057;
                    font-weight: 500;
                    font-size: 16px;
                }
            }
        }
        .btn-ctn{
            margin-top: 10px;
        }
    }
    }
}
</style>