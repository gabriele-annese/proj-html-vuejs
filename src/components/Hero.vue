<template>
    <div class="hero-ctn">
        <div class="tex-ctn">
            <h1>
                The biggest platform for your growth.
            </h1>
            <p>
                there are many variations of passages of Lorem ipsum available, but the majority have suffere alteration in some form.
            </p>
            <button class="btn">
                Read More
            </button>
        </div>
        <div class="hero-img">
            <img src="../assets/img/27-1.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
name: 'Hero',
}
</script>

<style lang="scss" scoped>
    .hero-ctn{
        width: 100%;
        height: 500px;
        background-color: #f2f7ff;
        border-radius: 8px;
        margin: 30px;
        display: flex;
        .tex-ctn{
            height: 200px;
            width: 40%;
            padding: 50px 30px;
            h1{
                line-height: 50px;
            }
            p{
                margin-top: 20px;
                line-height: 23px;
                color: #8e989f;
                font-weight: 500;
            }
            button{
                margin-top: 30px;
            }
        }
        .hero-img{
            width: 60%;
            position: relative;
            img{
                position: absolute;
                right: 50px;
                bottom: -30px;
            }
        }
    }
</style>