<template>
  <div class="cardbox">
    
    <h2 v-if="cardTitle">{{cardTitle}} </h2>
    <span v-if="cardCount">{{cardCount}}</span>
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
    width: 40%;
    height: 300px;
    background: #ddd;
    border-radius: 10px;
    display: inline-block;
    margin: 0 20px;

    box-sizing: border-box;
    padding: 20px;

}
</style>