<template>
  <div class="banner">
    <header>
      <div class="container">
        <div class="banner-top">
          <div class="top_name">
            Vladimir Gutman
          </div>
          <MenuTop></MenuTop>
        </div>
        <div class="banner-body">
          <div class="body-row row justify-content-between d-flex">
            <div class="body-row_image col-4">
              <img src="@/assets/my_face.jpg" alt="">
            </div>
            <div class="body-row_text col-5">
              Вот такой вот я красавчик!!
              Возьмите меня на работу =)
            </div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script>

import MenuTop from '@/components/menu/MenuTop'
export default {
  name: 'BannerComponent',
  components: { MenuTop },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">
  .banner{
    background-color: rgba(0,47,60,var(--bg-opacity));
    height: 100vh;
    .banner-top{
      display: flex;
      align-items: center;
      justify-content: space-between;
      .top_name{
        font-family: 'Poppins', sans-serif;
        color: #f7f474;
        font-size: 50px;
      }
    }
    .banner-body{
      display: flex;
      align-items: center;
      height: 100vh;
      .body-row{
        width: 100%;
        align-items: center;
        .body-row_image{
          position: relative;
          &:after{
            content: '';
            display: block;
            width: calc(100% + 20px);
            height: calc(100% + 20px);
            top:-10px;
            bottom: -10px;
            left:-10px;
            right: -10px;
            position: absolute;
            border-radius: 50%;
            border-top: 5px solid #f7f474;
            background: transparent;
          }
          &:before{
            content: '';
            display: block;
            width: calc(100% + 20px);
            height: calc(100% + 20px);
            top:-10px;
            bottom: -10px;
            left:-10px;
            right: -10px;
            position: absolute;
            border-radius: 50%;
            border-top: 5px solid #0ff;
            background: transparent;
            transform: rotate(180deg);
          }
          img{
            width: 100%;
            border-radius: 50%;
            height: 432px;
            object-fit:cover;
          }
        }
        .body-row_text{
          font-size: 40px;
          color: #0ff;
        }
      }
    }
  }
</style>
