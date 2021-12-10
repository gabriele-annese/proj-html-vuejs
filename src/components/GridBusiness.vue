<template>
  <section>
    <div class="img-ctn">
        <img src="../assets/img/14.png" alt="">
    </div>
    <div class="grid">
        <div class="header-grid">
            <div class="tex-ctn">
                <h1>Popular features that your business needs</h1>
                <p>Faff about only a quid blower i don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny</p>
            </div>
            <div class="btn-ctn">
                <button class="btn">
                    explore More Feaure
                </button>
            </div>
        </div>
        <div class="grid-ctn">
            <div class="elGrid" v-for="(eltitle, i) in TitleGrid" :key="`el-${i}`">
                <h4>{{eltitle.title}}</h4>
                <div>
                    <i :class="eltitle.icon"></i>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
name: 'GridBusiness',
data(){
    return{
        TitleGrid:[
            {
                title: 'Customized Invoices',
                icon:'fas fa-chart-bar iconAnalytics'
            },
            {
                title: 'Stock Management',
                icon:'fas fa-paper-plane iconPLane'
            },
            {
                title: 'Receivable & Payables',
                icon:'fas fa-user-tie iconManager'
            },
            {
                title: 'Receivable & Payables',
                icon:'fas fa-thumbs-up iconLike'
            },
            {
                title: 'Manage Buying',
                icon:'fas fa-virus iconVirus'
            },
            {
                title: 'Powerful & Secure',
                icon:'fas fa-user-tie iconManager'
            },
            {
                title: 'Fostest Return Filing',
                icon:'far fa-edit iconAnalytics'
            },
            {
                title: 'Monrhly Detailed',
                icon:'far fa-thumbs-up iconLike'
            },
        ]
    }
}

}
</script>

<style lang="scss" scoped>
section{
    width: 100%;
    position: relative;
    img{
        position: relative;
        left: -24%;
        top: -10%;
    }
    .grid{
        position: absolute;
        top: 80px;
        left: 13%;
        width: 80%;
        .header-grid{
            display: flex;
            align-items: center;
        }
        .tex-ctn{
            width: 50%;
            p{
                padding-top: 20px;
                line-height: 25px;
                color: #495057;
                font-weight: 500;
            }
        }
        .btn-ctn{
            width: 50%;
            margin-left: 20px;
            display: flex;
            justify-content: center;
        }
        .grid-ctn{
            width: 100%;
            margin-top: 30px;
            display: flex;
            flex-wrap: wrap;
            .elGrid{
                width: calc(100% / 4 - 30px);
                margin: 20px 10px;
                height: 160px;
                padding: 20px 15px;
                border-radius: 5px;
                cursor: pointer;
                border: 1px solid rgba($color: #000008, $alpha: 0.2);
                i{
                    font-size: 40px;
                    padding-top: 20px;
                }
                &:hover{
                    box-shadow: -8px  8px 5px rgba($color: #1e1e1e, $alpha: .2);
                }
            }
        }
    }
    .iconAnalytics{
        color: #377dff;
    }
    .iconPLane{
        color: #ff796d;
    }
    .iconManager{
        color: #6cdac1;
    }
    .iconLike{
        color: #377dff;
    }
    .iconVirus{
        color: #ff796d;
    }
    .iconLike{
        color: #ff796d;
    }
}
</style>