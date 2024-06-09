<template>
    <div id="MenuPage">
        <!-- header -->
        <img class="BrowserButton" src="../assets/icons/BrowserButton.svg" alt="">

        <img class="subBackground" src="../assets/imgs/Bar.png" alt="">
        <!-- header -->
        <ul >
            <li><img src="../assets/icons/iconHome.png" alt=""></li>
            <li><img src="../assets/icons/iconFriends.png" alt=""></li>
            <li><img src="../assets/icons/iconPlus.png" alt=""></li>
        </ul>
        <!-- footer -->
        <!-- <img class="iconSetting" src="../assets/icons/iconSetting.svg" alt=""> -->
        <!-- footer -->
    </div>
</template>

<script>
export default {
    data(){
        return{
            
        }
    }
}
</script>

<style scoped>
#MenuPage{
    display: flex;
    width: 58px;
    height: 100%;
    flex-direction: column;
    align-items: flex-end;
    background:  linear-gradient(to top, #7028e4 0%, #e5b2ca 100%);
    border-top-left-radius: 16px;
    border-bottom-left-radius: 16px;

}
.BrowserButton{
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
ul{
    display: flex;
    position: relative;
    flex-direction: column;
    width: 48px;
    height: 320px;
    text-align:center;
    justify-content: center;
    align-items: center;
    gap: 20px;
}
ul li{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 4px 4px;
    width: 28px;
    height: 28px;
    background:  linear-gradient(120deg, #fccb90 0%, #d57eeb 100%);
    border-radius: 8px;
    cursor: pointer;
    /* margin-top: 20px; */
}
ul li img{
    width: 20px;
    height: 20px;
    
    align-content: center;
}
ul li:hover{
    background:  linear-gradient(120deg, #b484e2 0%, #e8ee91 100%);
}
ul li:hover img{
    transform: scale(1.1);
    transition: transform 0.5s ease-in-out;
}
.iconSetting{
    position: relative;
    margin-top: 140px;
    margin-right: 20px;
    width: 20px;
    height: 20px;
    cursor: pointer;
}
.iconSetting:hover{
    transform: rotate(90deg);
            /* Để xoay quanh trục trung tâm */
    transform-origin: center center;
            /* Bạn có thể thêm transition để hiệu ứng mượt hơn */
    transition: transform 0.5s ease-in-out;
}
</style>