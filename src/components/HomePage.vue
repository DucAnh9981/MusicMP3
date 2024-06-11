<template>
  <div id="HomePage">
    <header>
      <div class="slidePage">
        <img
          class="HomePageImg"
          src="../assets/imgs/headerHomePage.png"
          alt=""
        />
      </div>
    </header>
    <main>
        <div>
            <h1>Nổi bật</h1>

        </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#HomePage {
  width: 520px;
  height: 100%;
  background-color: #1D203E;
  box-shadow: 1px 0px 0px 0px rgba(255, 255, 255, 0.10) inset;

  border-right: 1px solid #4f5151;
  border-left: 1px solid #4f5151;

}
.slidePage {
  width: 100%;
  height: 140px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
}
.HomePageImg {
  width: 96%;
  height: 100%;
  object-fit: cover;
  border-radius: 6px;
}
</style>