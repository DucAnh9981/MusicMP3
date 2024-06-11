<template>
  <div id="NavbarPage">
    <header>
      <h1>Ứng dụng nghe nhạc mp3</h1>
    </header>
    <main>
      <ul>
        <li :class="{selectNav : selected === 1}" @click="selectedNavbar(1)">Dành cho bạn</li>
        <li :class="{selectNav : selected === 2}" @click="selectedNavbar(2)">Nhạc thịnh hành</li>
        <li :class="{selectNav : selected === 3}" @click="selectedNavbar(3)">Bảng xếp hạng</li>
        <li :class="{selectNav : selected === 4}" @click="selectedNavbar(4)">Những bản hit mới</li>
        <li :class="{selectNav : selected === 5}" @click="selectedNavbar(5)">Hot trong tháng</li>
      </ul>
    </main>
    <footer>
      <img class="FooterNavbar" src="../assets/imgs/FooterNavbar.svg" alt="">
      <img class="Footer" src="../assets/imgs/Footer.svg" alt="">

      <img class="iconMusicDish" src="../assets/icons/iconMusicDish.svg" alt="">
      <ul>
        <li><i class="ti-control-backward"></i></li>
        <li><i class="ti-control-pause"></i></li>
        <li><i class="ti-control-forward"></i></li>
      </ul>
    </footer>
  </div>
</template>

<script>
export default {
  data(){
    return{
      selected: 1
    }
  },
  methods:{
      selectedNavbar(index){
        this.selected = index;
    }
  }
}
</script>

<style scoped>
#NavbarPage{
    width: 200px;
    height: 100%;
    background:   #2c2f48;
  box-shadow: 1px 0px 0px 0px rgba(255, 255, 255, 0.1) inset;

}
header{
  border-bottom: 1px solid #a7bcff;
}
header h1{
  font-size: 12px;
  padding: 0px 12px;
  color: #FFF;
}
main ul{
  margin-top: 60px;
  height: 180px;
}
main ul li{
  border-bottom: 1px solid #838686;
  cursor: pointer;
  padding: 8px 12px;
  color: #Fff;
  font-size: 16px;
  font-weight: 500;
}
.selectNav{
  box-shadow: 0 8px 12px rgba(145, 39, 141, 0.2);
  transition: transform 0.5s ease-in-out;
  color: #c699d8;
  transform: translateX(5px);
  font-weight: 600;
  width: 170px;
}
main ul li:hover{
  width: 160px;
  box-shadow: 0 8px 12px rgba(145, 39, 141, 0.2);
  transition: transform 0.5s ease-in-out;
  color: #c699d8;
  transform: translateX(3px);
  font-weight: 600;
}
footer .FooterNavbar{
  position: relative;
  width: 258px;
  left: -59px;
  bottom: -132px;
  z-index: 100;
}
footer .Footer{
  position: relative;
  width: 258px;
  left: -59px;
  bottom: -110px;
  z-index: 0;
  border-bottom-left-radius: 16px;
}
footer ul{
  position: absolute;
  display: flex;
  bottom: 86px;
  gap: 30px;
  left: 340px;
}
footer ul li i{
  font-weight: 800;
  cursor: pointer;
}
.iconMusicDish{
  position: absolute;
  width: 40px;
  height: 40px;
  bottom: 96px;
  left: 260px;
  transform-origin: center center;
  transition: transform 0.5s ease-in-out;
  animation: spin 2s linear infinite;
}
@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
</style>