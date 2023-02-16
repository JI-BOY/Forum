<template>
  <div class="container">

    <span>
      网站仅因个人爱好仿twitter,无任何盈利行为，仅供学习使用
    </span>
    <span>
      <a href="#">© 2021 Twitter, Inc.</a>
    </span>
  </div>
</template>

<script>
export default {
  name: 'SideBarRightFooter'
}
</script>

<style scoped lang="scss">
.container {
  position: sticky;
  top: calc(314px + 1rem + 24px);
  width: 350px;
  margin-top: 16px;
  margin-left: 25px;
  padding-left: 16px;
  padding-right: 16px;

  span {
    margin-right: 4px;
    color: #5b7083;
    font-size: 12px;

    a {
      color: #5b7083;
      font-size: 12px;
    }
  }
}
</style>