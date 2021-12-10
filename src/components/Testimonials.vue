<template>
  <section>
     <div class="img-ctn">
         <img src="../assets/img/15.png" alt="">
     </div>
     <div class="container-testimonial">
         <div class="text-ctn">
             <h2>Our Testimonials</h2>
             <p>If you are planning on developing a product landing app or website take a look at this beautiful-crafted</p>
         </div>
         <div class="grid-ctn">
             <div class="grid-el-right">
                 <div class="card">
                     <div class="ctn-profile">
                         <img src="../assets/img/25.jpeg" alt="">
                     </div>
                     <div class="name-ctn">
                         <h3>Mac Znder</h3>
                         <span> - Manager Sofbox</span>
                     </div>
                     <div class="text">
                         <p>
                             At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.
                         </p>
                     </div>
                 </div>
             </div>
             <div class="grid-el-left">
                 <div class="card">
                     <div class="ctn-profile">
                         <img src="../assets/img/26.jpeg" alt="">
                     </div>
                     <div class="name-ctn">
                         <h3>Julia Aann</h3>
                         <span> - COO Sofbox</span>
                     </div>
                     <div class="text">
                         <p>
                             At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.
                         </p>
                     </div>
                 </div>
             </div>
         </div>
        <div class="check-ctn">
            <!-- inserire-check-box -->
        </div>
     </div>
  </section>
</template>

<script>
export default {
name: 'Testimonials',
}
</script>

<style lang="scss" scoped>
section .img-ctn img{
    background-color: #f2f7ff;
    width: 100%;
    object-fit: cover;
}
.container-testimonial{
    width: 80%;
    margin: 0 auto;
    position: relative;
    top: -10.5%;
    .text-ctn{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        p{
            color: #8e989f;
        }
    }
    .grid-ctn{
        width: 100%;
        display: flex;
        .grid-el-right{
            width: 50%;
        }
        .grid-el-left{
            width: 50%;
        }
        .card{
            width: 80%;
            height: 300px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            margin-top: 30px;
            border-radius: 5px;
            border: 1px solid rgba($color: #8e989f, $alpha: 0.2);
            padding: 30px 0;
            box-shadow: -8px  8px 5px rgba($color: #1e1e1e, $alpha: .2);
            cursor: pointer;
            .ctn-profile{
                width: 100px;
                height: 100px;
                border: 1px solid #fff;
                border-radius: 50%;
                img{
                    width: 100%;
                    height: 100%;
                    border-radius: 50%;
                }
            }
            .name-ctn{
                display: flex;
                align-items: center;
                padding: 10px 0;
                span{
                    color: #8e989f;
                    font-weight: 500;
                }
            }
            p{
                padding: 10px 0;
                text-align: center;
                color: #8e989f;
            }
        }
    }
}
</style>