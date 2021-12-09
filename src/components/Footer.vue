<template>
  <div class="footer-ctn">
      <div class="footer-content">
          <ul class="footer-text">
              <li>
                  <div class="img-ctn">
                    <img src="../assets/img/35.png" alt="">
                  </div>
                  <p>
                      It is a long established fact that a reader will be distracted by the readable content
                  </p>
                  <span>Copyright @2018 <a href="/">sofbox</a> </span>
              </li>
          </ul>

          <ul>
                <li>
                    <h4 class="title"> Menu </h4>
                </li>
                <li v-for="(elMenu, i) in Menu" :key="`el-${i}`">
                    <a href="/">
                        {{elMenu}}
                    </a>
                </li>
          </ul>

          <ul>
                <li>
                    <h4 class="title"> About US </h4>
                </li>
                <li v-for="(elAbout, i) in AboutUs" :key="`el-${i}`">
                    <a href="/">
                    {{elAbout}}
                    </a>
                </li>
          </ul>

          <ul>
                <li>
                    <h4 class="title">Quick Links</h4>
                </li>
                <li v-for="(elQuick, i) in QuickLinks" :key="`el-${i}`">
                    <a href="/">
                    {{elQuick}}
                    </a>
                </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
name: 'Footer',
data(){
    return{
        Menu:[
            'About Us',
            'Theme',
            'Featurres',
            'Pricing',
            'Blog'
        ],
        AboutUs:[
            'About Sofbox',
            'Roadmap',
            'How it Work',
            'Team',
            'News'
        ],
        QuickLinks:[
            'About Us',
            'Theme',
            'Featurres',
            'Pricing',
            'Blog'
        ]
    }
}
}
</script>

<style lang="scss" scoped>
.footer-ctn{
    border-top: 1px solid grey;
    .footer-content{
        width: 80%;
        margin: 0 auto;
        display: flex;
        padding-top: 50px;
        ul{
            list-style: none;
            width: calc(100% / 4);
        }
        .footer-text{
            margin-right:80px ;
            font-weight: 500;
            p{
                line-height: 30px;
                padding-top: 10px;
                color: #8e989f;
            }
            span{
                display: block;
                margin-top: 20px;
                a{
                    text-decoration: none;
                    color: #377dff;
                }
            }
        }
        .title {
            margin-bottom: 35px;
        }
        li{
            padding: 5px 0;
            a{
                text-decoration: none;
                color: #8e989f;
                font-weight: 500;
                &:hover{
                    text-decoration: underline;
                }
            }
        }
    }
}
</style>