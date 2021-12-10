<template>
  <div class="container-grid">
      <div class="tex-ctn">
            <h2>Latest Posts</h2>
            <p>If you are planning o developing a product landing</p>
      </div>
      <div class="grid-post">
          <div class="grid-el">
              <div class="img-ctn">
                  <img src="../assets/img/19.jpg" alt="">
                  <div class="text">
                      <span>November 28, 2019</span>
                  </div>
              </div>
              <div class="tex-ctn">
                  <h4>Life Lack Meaning</h4>
                  <p>It is long established fact that a reader will be distracted by the readable.</p>
              </div>
          </div>
           <div class="grid-el">
               <div class="img-ctn">
                  <img src="../assets/img/18.jpg" alt="">
                  <div class="text">
                      <span>November 28, 2019</span>
                  </div>
              </div>
              <div class="tex-ctn">
                  <h4>Life Lack Meaning</h4>
                  <p>It is long established fact that a reader will be distracted by the readable.</p>
              </div>
          </div>
           <div class="grid-el">
               <div class="img-ctn">
                  <img src="../assets/img/17.jpg" alt="">
                  <div class="text">
                      <span>November 28, 2019</span>
                  </div>
              </div>
              <div class="tex-ctn">
                  <h4>Life Lack Meaning</h4>
                  <p>It is long established fact that a reader will be distracted by the readable.</p>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
name: 'GrdiPost',
}
</script>

<style lang="scss" scoped>
.container-grid{
    margin-top: 80px;
    .tex-ctn{
        text-align: center;
        p{
            padding-top: 10px;
            color: #495057;
            font-weight: 500;
        }
    }
    .grid-post{
        width: 90%;
        margin: 30px auto;
        display: flex;
        .grid-el{
            width: calc(100% / 3);
            margin: 10px;
            border: 1px solid rgba($color: #495057, $alpha: 0.2);
            border-radius: 5px;
            padding-top: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            cursor: pointer;
            &:hover,
            &:focus{
                box-shadow: -8px  8px 5px rgba($color: #1e1e1e, $alpha: .2);
            }
            .img-ctn{
                width: 90%;
                height: 100%;
                position: relative;
                img{
                    width: 100%;
                    height: 100%;
                    border-radius: 5px;
                }
                .text{
                    position: absolute;
                    top: 10px;
                    left: 5px;
                    background-color: #fff;
                    padding: 5px 5px;
                    border-radius: 5px;
                    span{
                        color: #495057;
                        font-weight: 500;
                    }
                }
            }
            .tex-ctn{
                padding: 10px;
                p{
                    color: #495057;
                    font-weight: 500;
                    padding-bottom: 30px;
                }
            }
        }
    }
}
</style>