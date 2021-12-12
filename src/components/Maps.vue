<template>
  <div class="conatiner-maps">
      <div class="text-ctn">
          <h4>Contact whit our team</h4>
          <p>If your are planning on developing a product landing.</p>
      </div>
      <section>
        <div class="maps-ctn">

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
        height: 300px;
        background-color: green;
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