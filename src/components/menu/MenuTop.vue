<template>
  <nav>
    <ul>
      <li>
        <a href="#">
          Скилы
        </a>
      </li>
      <li>
        <a href="#">
         Проекты
        </a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'MenuTop'
}
</script>

<style lang="scss" scoped>
  nav{
    ul{
      padding: 0;
      margin: 0;
      display: flex;
      align-items: center;
      gap: 20px;
      li{
        list-style: none;
        a{
          font-family: 'Poppins', sans-serif;
          color: #f7f474;
          text-decoration: none;
          font-size: 20px;
        }
      }
    }
  }
</style>
