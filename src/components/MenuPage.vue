<template>
  <div id="MenuPage">
    <!-- header -->
    <img class="BrowserButton" src="../assets/icons/BrowserButton.svg" alt="" />

    <img class="subBackground" src="../assets/imgs/Bar.png" alt="" />
    <!-- header -->
    <ul>
      <li :class="{ active: selectedIndex === 0 }" @click="selectItem(0)">
        <img src="../assets/icons/iconHome.png" alt="" />
      </li>
      <li :class="{ active: selectedIndex === 1 }" @click="selectItem(1)">
        <img src="../assets/icons/iconFriends.png" alt="" />
      </li>
      <li :class="{ active: selectedIndex === 2 }" @click="selectItem(2)">
        <img src="../assets/icons/iconPlus.png" alt="" />
      </li>
    </ul>
    <!-- footer -->
    <!-- <img class="iconSetting" src="../assets/icons/iconSetting.svg" alt=""> -->
    <!-- footer -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedIndex: 0, // Ban đầu chọn thẻ đầu tiên
    };
  },
  methods: {
    selectItem(index) {
      this.selectedIndex = index;
    },
  },
};
</script>

<style scoped>
#MenuPage {
  display: flex;
  width: 58px;
  height: 100%;
  flex-direction: column;
  align-items: flex-end;
  background: #1d203e;
  border-top-left-radius: 16px;
  border-bottom-left-radius: 16px;
  box-shadow: 1px 0px 0px 0px rgba(255, 255, 255, 0.1) inset;
}
.BrowserButton {
  width: 40px;
  height: 20px;
  margin-right: 8px;
}
.subBackground {
  margin-top: 30px;
  position: absolute;
  width: 48px;
  /* height: 480px; */
}
ul {
  display: flex;
  position: relative;
  flex-direction: column;
  width: 48px;
  height: 320px;
  text-align: center;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
ul li {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 4px 4px;
  width: 28px;
  height: 28px;
  background: linear-gradient(43deg, #4158d0 0%, #c850c0 46%, #ffcc70 100%);
  border-radius: 8px;
  cursor: pointer;
  position: relative;
}
.active{
  transition: transform 0.2s ease-in-out;
}
.active img {
  animation: pulse 2s infinite;
  transition: transform 0.2s ease-in-out;
}
.active::after {
  position: absolute;
  left: -12px;
  bottom: -4px;
  content: url('../assets/icons/Selected.svg');
  display: block;

}
@keyframes pulse {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
ul li img {
  width: 20px;
  height: 20px;
  align-content: center;
}
ul li:hover {
  background: linear-gradient(45deg, #fbda61 0%, #ff5acd 100%);
}
ul li:hover img {
  transform: scale(1.2);
  transition: transform 0.2s ease-in-out;
}
.iconSetting {
  position: relative;
  margin-top: 140px;
  margin-right: 20px;
  width: 20px;
  height: 20px;
  cursor: pointer;
}
.iconSetting:hover {
  transform: rotate(90deg);
  /* Để xoay quanh trục trung tâm */
  transform-origin: center center;
  /* Bạn có thể thêm transition để hiệu ứng mượt hơn */
  transition: transform 0.5s ease-in-out;
}
</style>