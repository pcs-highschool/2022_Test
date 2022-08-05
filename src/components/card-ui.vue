<template>
  <div class="cardbox">
    
    <h2 v-if="cardTitle || cardCount">
      <span v-if="cardTitle">{{cardTitle}}</span>
      <span v-else>제목 없음</span>
      <span v-if="cardCount"> | </span>
      <span v-if="cardCount">{{cardCount}}</span>
    </h2>
    <h2 v-else>제목 없슴</h2>
    <p v-if="title">{{title}}</p>
    <p v-else>내용 없슴</p>
  </div>
</template>

<script>

export default {
    props: {
        cardTitle : String,
        title: String,
        cardCount : Number,
    }
}
</script>

<style>
.cardbox {
    width: 500px;
    height: 500px;
    background: #ddd;
    border-radius: 10px;
    display: inline-block;
    margin: 20px;

    box-sizing: border-box;
    padding: 20px;
}
.cardbox > *{
  padding: 10px;
}
.cardbox p{
  font-size: 20px;
}
</style>