<script>
import Lists from '@/components/SideBarLeft/SideBarLeftLists'
import Icons from '@/components/Icons'

export default {
  name: 'SideBarLeft',
  components: {
    Lists,
    Icons
  }
}
</script>

<template>
  <div id="sidebar-left">
    <router-link to="/" tag="a">
      <span class="1024">
        <svg class="icon" width="48px" height="48.00px" viewBox="0 0 1024 1024" version="1.1"
          xmlns="http://www.w3.org/2000/svg">
          <path fill="#1da1f2"
            d="M853.333333 896h-42.666666v-192h-85.333334v-42.666667h128c-20.693333-12.458667-30.72-33.28-34.304-56.533333L802.112 490.666667H725.333333v-42.666667h70.229334l-3.946667-21.333333h43.178667l26.410666 171.669333C867.050667 636.437333 899.84 664.576 938.666667 661.333333v42.666667h-85.333334v192z m-170.666666 0h256v42.666667H85.333333v-42.666667h42.666667V405.333333H42.666667v-42.666666c38.570667 3.242667 71.36-24.896 77.226666-62.997334L146.304 128H189.44l-3.925333 21.333333h439.36l-3.946667-21.333333h43.178667l26.410666 171.669333C696.384 337.770667 729.173333 365.909333 768 362.666667v42.666666h-85.333333v490.666667z m-42.666667-490.666667H170.666667v490.666667h469.333333V405.333333z m-405.333333 64h149.333333v149.333334h-149.333333v-149.333334z m0 192h149.333333v149.333334h-149.333333v-149.333334z m192-192h149.333333v149.333334h-149.333333v-149.333334z m0 192h149.333333v149.333334h-149.333333v-149.333334z m-149.333334-149.333333v64h64v-64h-64z m0 256h64v-64h-64v64z m192-256v64h64v-64h-64z m0 256h64v-64h-64v64z m179.029334-461.866667L631.445333 192H178.986667l-16.896 114.133333a120.426667 120.426667 0 0 1-28.16 60.8h542.592a120.426667 120.426667 0 0 1-28.16-60.8z" />
        </svg>
      </span>
    </router-link>
    <lists />
  </div>
</template>

<style scoped lang="scss">
#sidebar-left {
  position: sticky;
  top: 15px;
  left: 0;
  max-width: 251px;
  max-height: 100vh;
  padding-left: 12px;
  padding-right: 12px;

  a {
    font-size: 30px;
    padding: 0.7rem;
    color: #1da1f2;
  }

  .twitter-icon {
    padding: 0.7rem;
    width: 50px;
    height: 50px;

    &:hover {
      background-color: rgba(#1da1f2, 0.2);
      border-radius: 100px;
    }
  }
}

@media (max-width: 1264px) {
  html {
    font-size: 14px;
  }

  #sidebar-left {
    width: 88px;
    height: 598px;
    // overflow-x: auto;
  }
}

@media (max-width: 476px) {
  #sidebar-left {
    padding: 0;
    display: none;
  }
}
</style>