<template>
  <div class="main">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>안녕하세요</h1>
    <inputCustom />

    <div class="sub">
      <card-ui :cardTitle="'안녕하세연'" :title="'Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit doloribus blanditiis sed nostrum, dolore tempora dolorem harum! Possimus dicta natus asperiores deleniti ipsa cum quasi perspiciatis! Animi veritatis minima fugit.'" :cardCount="1"/>
      <card-ui :cardTitle="'하이'" :title="'hellowordl'"/>
      <card-ui :title="'dkdfdfddf'" :cardCount="3"/>
      <card-ui />
    </div>
  </div>
</template>

<script>
  // 정의
  import InputCustom from './components/inputName.vue';
  import CardUi from './components/card-ui.vue';

  export default {
  // 등록
    components :{
    InputCustom,
    CardUi,
  }
}
</script>

<style>
.main {
  text-align: center;
}
.sub {
  display: flex;
  justify-content: space-around;
}
h1{
  margin: 50px 0;
}
</style>