<template>
  <div id="SubnavPage">
    <div class="body-subnav">
      <div class="formAvatar">
        <img class="avatar" src="../assets/imgs/avatarMe.jpg" alt="">
      </div>
      <div class="info">
        <p class="ten-nguoidung">Nguyễn Đức Anh</p>
        <p class="id-nguoidung">@21T_DT2</p>
      </div>
      <div class="friendUser">
        <div
          style="
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            margin-right: 10px;
            margin-top: 12px;
          "
        >
          <p class="titleFriend">Danh Sách Bạn Bè</p>
          <p class="descFriend">Tất Cả</p>
        </div>
        <div class="listfriendUser">
          <div class="avatarFriend"><img src="../assets/imgs/avatarNhat.jpg" alt="Friend Avatar 1" /></div>
          <div class="infoFriend">
            <p>Lê Quang Nhật</p>
            <p class="desc">1 phút trước</p>
          </div>
        </div>
        <div class="listfriendUser">
          <div class="avatarFriend"><img src="../assets/imgs/avatarMe.jpg" alt="Friend Avatar 2" /></div>
          <div class="infoFriend">
            <p>Nguyễn Đức Anh</p>
            <p class="desc">5 phút trước</p>
          </div>
        </div>
        <div class="listfriendUser">
          <div class="avatarFriend"><img src="../assets/imgs/avatarMe2.jpg" alt="Friend Avatar 3" /></div>
          <div class="infoFriend">
            <p>Nguyễn Ai Đó</p>
            <p class="desc">15 phút trước</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
#SubnavPage {
 display: flex;
  height: 100%;
  width: 220px;
  background: #2c2f48;
  box-shadow: 1px 0px 0px 0px rgba(255, 255, 255, 0.1) inset;
  border-bottom-right-radius: 16px;
  border-top-right-radius: 16px;
  justify-content: center;
}

.header-subnav {
  display: flex;
  padding: 5px 5px;
  box-shadow: 0px -1px 0px 0px rgba(255, 255, 255, 0.1) inset;
  align-items: center;
  justify-content: flex-end;
}
.header-subnav i {
  display: flex;
  color: white;
  font-size: 16px;
  margin-right: 10px;
  cursor: pointer;
  transition: transform 0.8s ease;
}
.header-subnav i:hover {
  transform: scale(1.1);
}
.header-subnav img {
  display: flex;
  color: white;
  width: 24px;
  height: 24px;
  padding: 5px 5px;
  border-radius: 8px;
  background-color: #724681;
  cursor: pointer;
  transition: transform 0.8s ease;
}
.header-subnav img:hover {
  border-radius: 4px;
  transform: scale(1.1);
}
.body-subnav {
  display: flex;
  /* justify-content: center; */
  flex-direction: column;
  text-align: center;
  margin-top: 30px;
  /* width: 100%; */
}
.body-subnav .formAvatar {
  width: 140px;
  height: 140px;
  margin: 0px 28px;
  margin-bottom: 12px;

}
.body-subnav .avatar {
  width: 100%;
  height: 140px;
  background-color: red;
  object-fit: cover; /* giữ đúng tỉ lệ của ảnh và lấp đầy khung hình*/
  border-radius: 999px;
}
.body-subnav .ten-nguoidung {
  color: white;
  font-size: 16px;
  margin: 2px 0;
}
.body-subnav .id-nguoidung {
  color: white;
  opacity: 50%;
  font-size: 12px;
  margin: 0 0;
}

.listfriendUser {
  background-color: rgba(255, 255, 255, 0.105);
  display: flex;
  flex-direction: row;
  width: 186px;
  height: 50px;
  margin-left: 5px;
  margin-bottom: 5px;
  border-radius: 8px;
  align-items: center;
  align-content: center;
  box-shadow: 0px -1px 0px 0px rgba(255, 255, 255, 0.1) inset;
}

.listfriendUser img {
  width: 100%;
  height: 30px;
  border-radius: 999px;
  margin-left: 10px;
}

.friendUser {
  margin-top: 20px;
}
.friendUser .titleFriend {
  display: flex;
  font-size: 10px;
  opacity: 0.7;
  color: #fff;
  margin-left: 6px;
}
.friendUser .descFriend {
  display: flex;
  margin-left: 80px;
  font-size: 8px;
  opacity: 0.3;
  color: #fff;
  margin-left: 10px;
  margin-bottom: 10px;
  cursor: pointer;
}
.infoFriend {
  display: flex;
  margin-left: 10px;
  flex-direction: column;
}
.avatarFriend {
  width: 30px;
  height: 30px;
  border-radius: 999px;
}
.infoFriend p {
  color: #fff;
  font-size: 10px;
  margin: 0;
  margin-left: 10px;
  padding: 0;
}

.infoFriend .desc {
  display: flex;
  padding: 0;
  margin: 0;
  color: #ffffff75;
  font-size: 9px;
  margin-left: 9px;
}
</style>
