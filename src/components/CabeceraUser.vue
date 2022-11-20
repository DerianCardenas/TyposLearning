<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
    <nav class="menu">
        <div class="logo-name">
            <svg class="logo-icon" width="80" height="51" viewBox="0 0 80 51" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M38.8144 0.87278C39.5196 0.353667 40.4804 0.353667 41.1856 0.872779L69.736 21.8893C71.2912 23.0341 70.4815 25.5 68.5504 25.5H11.4496C9.51852 25.5 8.70879 23.0341 10.264 21.8893L38.8144 0.87278Z" fill="#FF6868"/>
                <path d="M60 31C60 33.6264 59.4827 36.2272 58.4776 38.6537C57.4725 41.0802 55.9993 43.285 54.1421 45.1421C52.285 46.9993 50.0802 48.4725 47.6537 49.4776C45.2272 50.4827 42.6264 51 40 51V36C40.6566 36 41.3068 35.8707 41.9134 35.6194C42.52 35.3681 43.0712 34.9998 43.5355 34.5355C43.9998 34.0712 44.3681 33.52 44.6194 32.9134C44.8707 32.3068 45 31.6566 45 31H60Z" fill="#FF6868"/>
                <path d="M60 31C60 27.0444 58.827 23.1776 56.6294 19.8886C54.4318 16.5996 51.3082 14.0362 47.6537 12.5224C43.9991 11.0087 39.9778 10.6126 36.0982 11.3843C32.2186 12.156 28.6549 14.0608 25.8579 16.8579C23.0608 19.6549 21.156 23.2186 20.3843 27.0982C19.6126 30.9778 20.0087 34.9991 21.5224 38.6537C23.0362 42.3082 25.5996 45.4318 28.8886 47.6294C32.1776 49.827 36.0444 51 40 51V36C39.0111 36 38.0444 35.7068 37.2221 35.1573C36.3999 34.6079 35.759 33.827 35.3806 32.9134C35.0022 31.9998 34.9031 30.9945 35.0961 30.0245C35.289 29.0546 35.7652 28.1637 36.4645 27.4645C37.1637 26.7652 38.0546 26.289 39.0245 26.0961C39.9945 25.9031 40.9998 26.0022 41.9134 26.3806C42.827 26.759 43.6079 27.3999 44.1573 28.2221C44.7068 29.0444 45 30.0111 45 31H60Z" fill="#ADA9FF"/>
                </svg>
                
            <span class="logo-1">Typos</span><span class="logo-2">Learning</span>
        </div>
        <div class="cont-links">
            <RouterLink class="link" to="/">Tablero</RouterLink>
            <RouterLink class="link" to="/blog">Blog</RouterLink>
            <RouterLink class="link" to="/about">Lecciones</RouterLink>
        </div>
        <div class="cont-info">
            <div class="info">
                Lvl. 10<br/>
                1000 Pts.
            </div>
            <svg class="icon-triangle" width="21" height="19" viewBox="0 0 21 19" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12.2321 18C11.4622 19.3333 9.53775 19.3333 8.76795 18L0.540707 3.75C-0.229094 2.41667 0.733158 0.75 2.27276 0.75L18.7272 0.75C20.2668 0.75 21.2291 2.41667 20.4593 3.75L12.2321 18Z" fill="#D9D9D9"/>
                </svg>
                
            <svg class="logo-user" width="50" height="60" viewBox="0 0 50 60" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M19.8745 3.55102C22.9577 1.41496 27.0423 1.41496 30.1255 3.55102L42.7761 12.3156C45.2028 13.9969 46.6506 16.7614 46.6506 19.7136V40.2864C46.6506 43.2386 45.2028 46.0031 42.7761 47.6844L30.1255 56.449C27.0423 58.585 22.9577 58.585 19.8745 56.449L7.22391 47.6844C4.79722 46.0031 3.34937 43.2386 3.34937 40.2864V19.7136C3.34937 16.7614 4.79722 13.9969 7.22391 12.3156L19.8745 3.55102Z" fill="#D9D9D9"/>
                <path d="M10.7143 41.0185C12.0317 33.052 17.5783 29.5775 24.9999 29.5775C32.4215 29.5775 37.9679 33.0518 39.2857 41.0185C39.2857 41.0185 33.4416 48.1691 24.3507 48.1691C17.2078 48.1691 10.7143 41.0185 10.7143 41.0185Z" fill="#FF7979"/>
                <path d="M25.0001 11.8309C29.9233 11.8309 33.9286 15.622 33.9286 20.2819C33.9286 24.9415 29.9233 28.7323 25.0001 28.7323C20.077 28.7323 16.0714 24.9415 16.0714 20.2819C16.0714 15.622 20.077 11.8309 25.0001 11.8309Z" fill="#FF7979"/>
                </svg>
                    
                
        </div>
    </nav>
</template>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Open Sans");
@import url("https://fonts.googleapis.com/css?family=Cedarville+Cursive");
@import url("https://fonts.googleapis.com/css?family=Baloo Da 2");
.menu{
    display:flex;
    justify-content:space-around;
}
.logo-name{
    color:#0E1D47;
    display:flex;
    margin: auto 0;
    font-size: 26px;
}
.logo-icon{
    height:50px;
    width: 50px;
}
.logo-1{
    font-family: "Cedarville Cursive";
}
.logo-2{
    font-family: 'Open Sans';
}
.menu a.router-link-exact-active {
    color: #FF6868;
    font-weight: bold;
  }
.menu a.router-link-exact-active:hover {
    background-color: transparent;
  }
.link {
    border-left: 1px solid #CED5E9;
    display: inline-block;
    color: #0E1D47;
    font-size: 20px;
    font-weight: bold;
    padding: 0 1rem;
    text-decoration: none;
  }
  .link, .register-btn, .login-btn{
    font-family: "Baloo Da 2";
  }
.menu a:first-of-type {
    border: 0;
  }
  .cont-links, .cont-info {
    padding: 2em 0;
  }
  .cont-info{
    display: flex;
    justify-content:space-around;
    width:18%;
  }
  .info {
    border-right: 2px solid #CED5E9;
    padding: 0 1em;
    text-align: right;
  }
  .icon-triangle{
    margin: auto .1em;
    height:30px;
    padding:0;
    width: 30px;
  }
  .icon-triangle:hover,.logo-user:hover{
    cursor:pointer;
  }
  .logo-user{
    height:50px;
    width: 50px;
  }
</style>