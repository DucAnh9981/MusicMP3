<template>
  <div id="NavbarPage">
    <header>
      <h1>Ứng dụng nghe nhạc mp3</h1>
    </header>
    <main>
      <ul>
        <li>Dành cho bạn</li>
        <li>Nhạc thịnh hành</li>
        <li>Bảng xếp hạng</li>
        <li>Những bản hit mới</li>
        <li>Hot trong tháng</li>
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

}
</script>

<style scoped>
#NavbarPage{
    width: 200px;
    height: 100%;
    background:  linear-gradient(to top, #7028e4 0%, #e5b2ca 100%);;
;
}
header{
  border-bottom: 1px solid #a7bcff;
}
header h1{
  font-size: 12px;
  padding: 0px 12px;
}
main ul{
  margin-top: 60px;
}
main ul li{
   /* border: 1px solid #6e4985; */
   border-bottom: 1px solid #b5c6c6;

   padding: 8px 12px;
}
main ul li:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transform: scale(1.1);
  transition: transform 0.5s ease-in-out;
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
  bottom: -100px;
  z-index: 0;
  border-bottom-left-radius: 16px;
}
footer ul{
  position: absolute;
  display: flex;
  bottom: 96px;
  gap: 30px;
  left: 380px;
}
footer ul li i{
  font-weight: 800;
}
.iconMusicDish{
  position: absolute;
  width: 40px;
  height: 40px;
  bottom: 104px;
  left: 300px;
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