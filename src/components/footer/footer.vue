<template lang="html">
  <div class="footer">
    <div class="centerBox">
      <div class="left">
        <p>Copyright©2017 www.intelligentjoy.com All Right | 粤ICP备17088073号</p>
      </div>
      <div class="right">
        <a href="javascript:;">
          <i></i>
        </a>
        <span>{{ $t("footer.weChat") }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'myFooter'
}
</script>

<style lang="less">
.footer {
    height: 120px;
    background-color: #eeeeee;
    .centerBox {
        height: 120px;
        padding: 20px 0 38px 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        > div {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            height: 100%;
        }
        .left {
            display: flex;
            align-items: center;
            p {
                height: 100%;
                display: flex;
                align-items: center;
                font-size: 12px;
                color: #999;
                cursor: pointer;
            }
        }
        .right {
            position: relative;
            align-items: center;
            a {
                height: 34px;
                width: 34px;
                background-image: url("./images/weChat@2x.png");
                background-size: 100% 100%;
                position: relative;
                i {
                    position: absolute;
                    height: 120px;
                    width: 120px;
                    background-image: url("./images/weChatQrcode.jpg");
                    top: -130px;
                    left: -43px;
                    box-shadow: 0px 2px 7px RGBA(43, 63, 90, 0.3);
                    display: none;
                }
            }
            span:last-child {
                font-size: 14px;
                color: #666;
            }
            &:hover {
                a {
                    background-image: url("./images/weChatActive@2x.png");
                    i {
                        display: block;
                    }
                }
            }
        }
    }
}
</style>
