<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-box">
        <router-link to="/" class="footer-logo logo">
          <img src="../assets/images/logo.png" alt="logo" />
        </router-link>
        <div class="footer-nav">
          <ul>
            <li>Ресторанам</li>
            <li>Курьерам</li>
            <li>Пресс-центр</li>
            <li>Контакты</li>
          </ul>
        </div>
        <div class="footer-social">
          <img src="../assets/images/socials/inst.png" alt="inst" />
          <img src="../assets/images/socials/fb.png" alt="vk" />
          <img src="../assets/images/socials/vk.png" alt="fb" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer {
  min-height: 156px;
  display: flex;
  align-items: center;
  padding: 60px 0;
}

.footer-box {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 36px;
  flex-wrap: wrap;
}

.footer-nav {
  flex-grow: 1;
}

.footer-nav ul {
  display: flex;
  align-items: center;
  list-style: none;
  padding: 0;
  margin: 0;
  gap: 15px;
  flex-wrap: wrap;
}

.footer-nav ul li {
  font-weight: 400;
  font-size: 18px;
  color: #595959;
}

.footer-social {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 20px;
}
</style>
