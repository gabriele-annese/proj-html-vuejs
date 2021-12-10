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

        </div>
      </section>
  </div>
</template>

<script>
export default {

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
        height: 300px;
        background-color: red;
    }
}
</style>