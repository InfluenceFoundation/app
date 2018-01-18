<template>
  <div class="topbar">
    <div class="title">
      <h1>Influence</h1>
    </div>
    <div class="profile">
      <div class="profile__info">
        <span>@scotthaley</span>
        <span>12,000</span>
        <a href='#'>logout</a>
      </div>
      <img src="http://www.evatar.io/4f42226f69844d535deb9b9d2763eee73e03f9cfc9505d565cf2e9275c14c116"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'topbar'
}
</script>

<style lang="scss">
.topbar {
  display: flex;
  flex-direction: row;
  height: 100px;
  text-align: left;
  padding: 0 20px;
  box-sizing: border-box;
}

h1 {
  font-weight: 400;
  font-size: 2.5em;
}

a {
  text-decoration: none;
}

.title {
  flex-grow: 1;
}

.profile {
  display: flex;
  flex-direction: row;

  &__info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    padding-right: 20px;
  }

  img {
    width: 80px;
    height: 80px;
    align-self: center;
  }
}
</style>
