<template>
  <div :class="$style.site">
    <div v-if="!isOpen" @click="isOpen = true" :class="$style.chatVidget">
      <p>Загрузи чек сюда!</p>
      <div :class="$style.greenIcon">
        <svg width="30px" height="30px" viewBox="0 0 30 30" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <g fill="#FFFFFF" stroke="#FFFFFF" stroke-width="1" fill-rule="evenodd" >
                <path d="M21.2925249,22.480476 C23.2768482,21.8717451 25.0594814,20.6176792 26.3120832,18.9492516 C27.6075121,17.2233552 28.2923801,15.1676533 28.2923801,13.0039686 C28.2923801,7.539301 23.8471444,3.09333333 18.383209,3.09333333 L10.2958378,3.09333333 C4.8319023,3.09333333 0.386666667,7.539301 0.386666667,13.0039686 C0.386666667,16.9839626 2.75277364,20.5642368 6.41430948,22.1246814 C6.6624872,22.230468 6.82281443,22.4705927 6.82281443,22.7363406 L6.82281443,25.1042777 C6.82281443,25.7536394 7.2181417,26.3140524 7.82943477,26.5325805 C8.00037723,26.5937099 8.17534611,26.6233594 8.34775275,26.6233594 C8.79066577,26.6233594 9.21637461,26.4267939 9.51250401,26.0651426 L11.8936188,23.157657 C12.0202699,23.0031865 12.2069523,22.9146039 12.4064462,22.9146039 L17.8564719,22.9146039 C18.2448444,22.9146039 18.559276,22.6001723 18.559276,22.2117999 C18.559276,21.8237934 18.2448444,21.5089958 17.8564719,21.5089958 L12.4064462,21.5089958 C11.7838057,21.5089958 11.200698,21.7853588 10.8061028,22.2670724 L8.42498801,25.1745582 C8.41034626,25.1928604 8.37557208,25.2349554 8.30199731,25.2089662 C8.22842253,25.1826111 8.22842253,25.1277045 8.22842253,25.1042777 L8.22842253,22.7363406 C8.22842253,21.9065193 7.73243319,21.1586918 6.96520543,20.8318148 C3.82271953,19.4924606 1.79227477,16.4198892 1.79227477,13.0039686 C1.79227477,8.31421575 5.60681695,4.49894144 10.2958378,4.49894144 L18.383209,4.49894144 C23.0718637,4.49894144 26.886772,8.31421575 26.886772,13.0039686 C26.886772,14.8609087 26.2992717,16.6248737 25.1879627,18.1055207 C24.1121601,19.53785 22.5824632,20.6143847 20.8799935,21.1367292 C20.5091912,21.2505689 20.3005462,21.6436999 20.4143858,22.0145022 C20.5282255,22.3856706 20.9213565,22.5943156 21.2925249,22.480476 Z" id="Shape" stroke-width="0.3" fill-rule="nonzero"></path>
                <path d="M6.96,12.9423997 C6.96,14.1093473 7.90878547,15.0584988 9.07536692,15.0584988 C10.2419485,15.0584988 11.1911,14.1093473 11.1911,12.9423997 C11.1911,11.7758182 10.2419485,10.8266667 9.07536692,10.8266667 C7.90878547,10.8266667 6.96,11.7758182 6.96,12.9423997 Z M9.78549185,12.9423997 C9.78549185,13.3340665 9.46703381,13.6528906 9.07536692,13.6528906 C8.68406614,13.6528906 8.3656081,13.3340665 8.3656081,12.9423997 C8.3656081,12.5510988 8.68406614,12.2322748 9.07536692,12.2322748 C9.46703381,12.2322748 9.78549185,12.5510988 9.78549185,12.9423997 Z" id="Shape" stroke-width="0.3" fill-rule="nonzero"></path>
                <path d="M11.9866667,12.9423997 C11.9866667,14.1093473 12.9358183,15.0584988 14.1023998,15.0584988 C15.2686152,15.0584988 16.2177667,14.1093473 16.2177667,12.9423997 C16.2177667,11.7758182 15.2686152,10.8266667 14.1023998,10.8266667 C12.9358183,10.8266667 11.9866667,11.7758182 11.9866667,12.9423997 Z M14.8121586,12.9423997 C14.8121586,13.3340665 14.4937006,13.6528906 14.1023998,13.6528906 C13.7107329,13.6528906 13.3922748,13.3340665 13.3922748,12.9423997 C13.3922748,12.5510988 13.7107329,12.2322748 14.1023998,12.2322748 C14.4937006,12.2322748 14.8121586,12.5510988 14.8121586,12.9423997 Z" id="Shape" stroke-width="0.3" fill-rule="nonzero"></path>
                <path d="M21.6311,12.9423997 C21.6311,11.7758182 20.6823145,10.8266667 19.5157329,10.8266667 C18.3491515,10.8266667 17.4,11.7758182 17.4,12.9423997 C17.4,14.1093473 18.3491515,15.0584988 19.5157329,15.0584988 C20.6823145,15.0584988 21.6311,14.1093473 21.6311,12.9423997 Z M19.5157329,13.6528906 C19.1240661,13.6528906 18.8056081,13.3340665 18.8056081,12.9423997 C18.8056081,12.5510988 19.1240661,12.2322748 19.5157329,12.2322748 C19.9070338,12.2322748 20.2254918,12.5510988 20.2254918,12.9423997 C20.2254918,13.3340665 19.9070338,13.6528906 19.5157329,13.6528906 Z" id="Shape" stroke-width="0.3" fill-rule="nonzero"></path>
            </g>
        </svg>
      </div>
    </div>
    <div v-else :class="$style.chatBlock">
      <div :class="$style.header">
        <div :class="$style.avatar">
          <div :class="$style.pic">
            <label style="background: #63C841"></label>
          </div>
        </div>
        <p>SPLAT</p>
        <div @click="isOpen = false" :class="$style.close">
          <svg width="25px" height="25px" viewBox="0 0 25 25" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <g id="close-button" fill-rule="evenodd" stroke-width="1" fill="#FFFFFF" stroke="#FFFFFF">
                <path d="M11.4798395,23 C9.55275032,23 7.61472405,22.5195221 5.85930126,21.5311479 C5.53360882,21.3478375 5.41813971,20.9350488 5.60165042,20.6093541 C5.78495952,20.2840121 6.1973924,20.1676854 6.52343765,20.3517014 C10.4719167,22.5749134 15.4699499,21.8864787 18.67859,18.6783702 C22.6365949,14.7201356 22.6365949,8.28002822 18.67859,4.32179357 C14.7203836,0.363558919 8.27996926,0.363256509 4.32140998,4.32179357 C0.363405126,8.28002822 0.363405126,14.7201356 4.32140998,18.6783702 C4.58576419,18.9427263 4.58576419,19.3713914 4.32140998,19.6357475 C4.05740859,19.9001036 3.62874653,19.9001036 3.36439233,19.6357475 C-1.12146411,15.1495063 -1.12146411,7.85065749 3.36439233,3.36441629 C7.85024877,-1.1214721 15.1497512,-1.1214721 19.6356077,3.36441629 C24.1214641,7.85065749 24.1214641,15.1495063 19.6356077,19.6357475 C17.425919,21.8452503 14.46616,23 11.4798395,23 Z" id="Shape" stroke-width="0.5" fill-rule="nonzero"></path>
                <path d="M14.6499051,16.2916667 C14.4749862,16.2916667 14.3002199,16.2251 14.1667278,16.0916105 L6.90853333,8.83355516 C6.6416,8.56662695 6.6416,8.13379103 6.90853333,7.86686282 C7.17546665,7.59993461 7.60795462,7.59993461 7.87488795,7.86686282 L15.1331333,15.124969 C15.4000667,15.3918972 15.4000667,15.8247331 15.1331333,16.0916614 C14.9996412,16.2251509 14.824875,16.2916667 14.6499051,16.2916667 Z" id="Shape" stroke-width="0.5" fill-rule="nonzero"></path>
                <path d="M7.39171467,16.2916667 C7.2167947,16.2916667 7.04202741,16.2251 6.90853451,16.0916105 C6.64159961,15.8246823 6.64159961,15.3918463 6.90853451,15.1249181 L14.1667718,7.86686282 C14.4337067,7.59993461 14.8661973,7.59993461 15.1331322,7.86686282 C15.4000671,8.13379103 15.4000671,8.56662695 15.1331322,8.83355516 L7.87489483,16.0916614 C7.74140194,16.2251509 7.56663464,16.2916667 7.39171467,16.2916667 Z" id="Shape" stroke-width="0.5" fill-rule="nonzero"></path>
            </g>
          </svg>
        </div>
      </div>
      <div :class="$style.dialogBox">
        <div :class="$style.mover" v-for="(m,i) in messages" :key="i">
          <div :class="i%2!==0?$style.message_right:$style.message_left">
            <p v-if="i!==1">{{m}}</p>
            <img :class="$style.qrcode" v-if="!i" src="https://mbtskoudsalg.com/images/what-is-a-png-image-8.png" />
            <img :class="$style.attach" v-if="i===1" src="../assets/photo.png" />
          </div>
        </div>
      </div>
      <div :class="$style.messager">
        <div @click="openFile">
          <svg width="35px" height="35px" viewBox="0 0 35 35" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
              <defs>
                  <linearGradient x1="98.3146987%" y1="50%" x2="-2.22044605e-14%" y2="50%" id="linearGradient-1">
                      <stop stop-color="#3D57C6" offset="3.75045159%"></stop>
                      <stop stop-color="#3E6EDB" offset="97.0962789%"></stop>
                  </linearGradient>
                  <linearGradient x1="98.3146987%" y1="50%" x2="-2.22044605e-14%" y2="50%" id="linearGradient-2">
                      <stop stop-color="#3D64C6" offset="0%"></stop>
                      <stop stop-color="#3E84DB" offset="100%"></stop>
                  </linearGradient>
              </defs>
              <g id="one-clip" fill-rule="evenodd" transform="translate(25, 0) rotate(45)" stroke-width="1" fill="url(#linearGradient-1)" stroke="url(#linearGradient-2)" >
                  <path d="M6.53890535,4.04972376 C7.95353189,4.04972376 9.10619055,5.21567424 9.10619055,6.64661346 L9.10619055,25.4210661 C9.10619055,25.7655515 9.38125682,26.0570391 9.73491346,26.0570391 C10.0885701,26.0570391 10.3636364,25.7788009 10.3636364,25.4210661 L10.3636364,6.63336403 C10.3636364,4.51345406 8.64774676,2.77777778 6.55200374,2.77777778 C4.45626072,2.77777778 2.72727273,4.51345406 2.72727273,6.63336403 L2.72727273,28.508185 C2.72727273,29.4753939 2.98924061,30.4293534 3.48697957,31.2508185 C3.60486512,31.4495601 3.81443942,31.5555556 4.02401372,31.5555556 C4.14189927,31.5555556 4.24668642,31.5290567 4.35147357,31.4628095 C4.63963823,31.2773174 4.74442539,30.8930837 4.56104787,30.5883466 C4.18119445,29.9656231 3.98471854,29.2501535 3.98471854,28.508185 L3.98471854,6.63336403 C3.97162015,5.2024248 5.12427881,4.04972376 6.53890535,4.04972376 Z" id="Shape" stroke-width="0.7" fill-rule="nonzero"></path>
                  <path d="M12.1931041,3.44253545 C12.0251115,3.13745868 11.6503586,3.01808081 11.3531409,3.19051551 C11.0559231,3.3629502 10.9396205,3.74761222 11.1076131,4.05268899 C11.5211335,4.83527723 11.7537387,5.73724333 11.7537387,6.63920943 L11.7537387,28.5118874 C11.7537387,30.7137459 10.0091996,32.5044139 7.86406269,32.5044139 C7.19209208,32.5044139 6.52012147,32.318715 5.93860845,31.9871098 C5.64139068,31.8146751 5.26663784,31.9207887 5.09864518,32.2258655 C4.93065253,32.5309423 5.03403262,32.9156043 5.33125039,33.088039 C6.1066011,33.539022 6.97240938,33.7777778 7.86406269,33.7777778 C10.6811703,33.7777778 12.9813773,31.4167489 12.9813773,28.5251516 L12.9813773,6.62594522 C12.9942998,5.5117518 12.7229271,4.41082259 12.1931041,3.44253545 Z" id="Shape" stroke-width="0.7" fill-rule="nonzero"></path>
                  <path d="M6.47986449,1.27087576 C7.52750725,1.27087576 8.53634843,1.5885947 9.40291713,2.18431772 C9.68746208,2.38289206 10.0625441,2.30346232 10.256552,2.01221996 C10.4505599,1.7209776 10.3729567,1.32382892 10.0884118,1.13849287 C9.02783515,0.397148676 7.77325061,0 6.47986449,0 C2.91011878,0 0,2.97861507 0,6.63238289 L0,25.3645621 C0,25.7087576 0.271611086,26 0.62082534,26 C0.957105733,26 1.24165068,25.7219959 1.24165068,25.3645621 L1.24165068,6.63238289 C1.22871682,3.6802444 3.58267957,1.27087576 6.47986449,1.27087576 Z" id="Shape" stroke-width="0.7" fill-rule="nonzero"></path>
              </g>
          </svg>
          <input id="fileInput" type="file" style="display:none" />
        </div>
        <input placeholder="Введите сообщение..." />
        <div>
          <svg width="26px" height="23px" viewBox="0 0 26 23" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
              <defs>
                  <linearGradient x1="94.6274535%" y1="50%" x2="2.85478465%" y2="50%" id="linearGradient-1">
                      <stop stop-color="#3D57C6" offset="0%"></stop>
                      <stop stop-color="#3E6EDB" offset="100%"></stop>
                  </linearGradient>
                  <linearGradient x1="98.3146987%" y1="50%" x2="-2.22044605e-14%" y2="50%" id="linearGradient-2">
                      <stop stop-color="#3D64C6" offset="0%"></stop>
                      <stop stop-color="#3E84DB" offset="100%"></stop>
                  </linearGradient>
              </defs>
              <g stroke-width="1" fill-rule="evenodd" fill="url(#linearGradient-1)" stroke="url(#linearGradient-2)">
                  <path d="M24.6647887,10.6124714 C24.6647887,9.75880906 24.1768878,9.0256638 23.3871925,8.69926351 L2.88026343,0.162640594 C2.07547838,-0.173802779 1.16506529,0.0220373935 0.566506413,0.654751798 C-0.0320524674,1.2874662 -0.167859944,2.20640855 0.214412954,2.98976924 L3.48385222,9.64331358 C3.57942044,9.83915375 3.77055689,9.96971386 3.98684287,9.98477849 L15.5908373,10.9338501 C15.9328709,10.9639794 16.2296354,10.7078807 16.254785,10.3714373 C16.2849644,10.0349939 16.0284392,9.73370135 15.6914354,9.70859363 L4.43450456,8.78462974 L1.3209924,2.44744261 C1.07955688,1.96035295 1.37129146,1.59880186 1.46182978,1.498371 C1.557398,1.39794015 1.89943165,1.08660449 2.40242231,1.29750929 L22.9093513,9.83413221 C23.3922224,10.0349939 23.4274317,10.4819112 23.4274317,10.6124714 C23.4274317,10.7430315 23.3922224,11.1899488 22.9093513,11.3908105 L2.40242231,19.9274334 C1.89943165,20.1383382 1.557398,19.8270026 1.46182978,19.7265717 C1.36626156,19.6261408 1.07955688,19.2645898 1.3209924,18.7775001 L4.59043166,12.1239558 C4.74132886,11.8176416 4.61558119,11.451069 4.30875689,11.3004227 C4.00193259,11.1497764 3.63474941,11.275315 3.48385222,11.5816291 L0.214412954,18.2351735 C-0.167859944,19.0185342 -0.0320524674,19.932455 0.566506413,20.5701909 C0.968898938,20.9970221 1.51212885,21.228013 2.07044847,21.228013 C2.34206343,21.228013 2.61367838,21.1727761 2.87523352,21.0673237 L23.3821626,12.5307007 C24.1768878,12.1992789 24.6647887,11.4661336 24.6647887,10.6124714 Z" id="Shape" stroke-width="0.5" fill-rule="nonzero"></path>
              </g>
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  data(){
    return {
      messages: new Array(10).fill('Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'),
      isOpen: true
    }
  },
  methods: {
    openFile(){
      document.getElementById('fileInput').click()
    }
  }
}
</script>


<style module lang="stylus">

// variables
height = 45px

headerHeight = 61px
messagerHeight = 53px
chatBlockHeight = 550px

center()
  display flex
  justify-content center
  align-items center

@font-face
  font-family: "FuturaBookC"
  src: url('/static/fonts/futurabookc.otf') format("otf"), url('/static/fonts/futurabookc.woff') format("woff")

body
  margin 0

mes()
  width 75%
  background: #4363BE
  font-family 'FuturaBookC'
  color white
  padding 4px
  margin-top 4px
  border-radius: 8px
  font-size: 1.2em
  font-weight light
  letter-spacing: 0
  line-height: 1.2em
  position relative
  .qrcode
    width 60%
    margin-left 5%
    margin-bottom 10%
    filter invert(100%)
  .attach
    position relative
    width 95%
    margin-left 2.5%
    margin-right 2.5%
    margin-top 2%
    margin-bottom 2%
    z-index 100
before()
  position: absolute
  top calc(50% - 10px)
  content: '\00a0'
  transform: rotate(45deg) //skew(-35deg)
  border-radius 4px
  background #4363BE
  display: block
  width: 20px
  height: 20px


.mover
  display block
  width 100%
.message_left
  mes()
  left 12px
  p
    width 80%
    margin-left 5%
    margin-top 5%
  &:before
    before()
    left - 8px

.message_right
  mes()
  background #D1D7E2
  color #454545
  float right
  left -12px
  p
    width 80%
    margin-left 10%
  &:before
    before()
    background #D1D7E2
    color #454545
    right -8px

.site
  width 100vw
  height 100vh

.chatBlock
  width 355px
  height chatBlockHeight
  position absolute
  bottom 0
  left 45px
  .header
    width 100%
    height headerHeight
    background-image: linear-gradient(-269deg, #3D64C6 2%, #3E84DB 100%)
    border-top-left-radius: 20px
    border-top-right-radius: 20px
    font-family: Futura-CondensedMedium
    font-size: 20px
    color: #FFFFFF
    letter-spacing: 0
    display flex
    .avatar
      width headerHeight
      height headerHeight
      center()
      .pic
        width 45px
        height 45px
        background url('../assets/avatar.jpg') no-repeat center center
        background-size cover
        border-radius 50%
        position relative
        label
          width 10px
          height 10px
          border 1px solid white
          border-radius 50%
          position absolute
          right 2px
          bottom 2px
    .close
      width headerHeight
      height headerHeight
      cursor pointer
      center()
    p
      margin 0
      line-height headerHeight
      flex 2
      text-align center
      font-family 'FuturaBookC'
      position relative
      top 4px
  .dialogBox
    width 100%
    height "calc(%s - %s - %s)" % (chatBlockHeight messagerHeight headerHeight )
    background ghostwhite
    display flex
    flex-direction column
    overflow-y scroll
    /* background url('../assets/clouds.jpg') no-repeat center center
    background-size cover */
    &::-webkit-scrollbar
      width: .5em
    &::-webkit-scrollbar-thumb
      background: #4363BE
      border-radius: 100px
      outline: 1px solid slategrey

  .messager
    width 100%
    height messagerHeight
    background: #FFFFFF
    box-shadow: 0 -2px 4px 0 rgba(0,0,0,0.05)
    font-family: FuturaPTBook
    font-size: 18px
    color: #A2A2A2
    letter-spacing: 0
    display flex
    input
      flex 2
      font-size 1em
      font-family 'FuturaBookC'
      outline none
      border none
    div
      cursor pointer
      width messagerHeight
      height messagerHeight
      center()

.chatVidget
  width: 249px
  height: height
  border-radius: 22.5px
  background-image: linear-gradient(-269deg, #3D64C6 2%, #3E84DB 100%)
  display: flex
  cursor pointer
  position absolute
  bottom 0
  left 45px
  p
    font-family 'FuturaBookC'
    color: white
    line-height: height
    width: calc(100% - height)
    margin: 0
    flex 2
    text-align center
  .greenIcon
    width: height
    height: height
    background: #36CA67
    border-radius: 50%
    center()

@media (orientation : portrait )
  chatBlockHeight = 100%
  .chatVidget
    left 0
    width 100%
    border-radius 0
    .greenIcon
      border-radius 0
  .chatBlock
    left 0
    width 100%
    height chatBlockHeight
    .dialogBox
      height "calc(%s - %s - %s)" % (chatBlockHeight messagerHeight headerHeight )

</style>
