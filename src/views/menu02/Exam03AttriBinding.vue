<!-- 컴포넌트 UI 정의-->
<template>
    <div class = "card">
      <div class = "card-header">
        Exam03AttriBinding
        </div>
      <div class = "card-body">
        <p>
          <img v-bind:src="require(`@/assets/photos/${imgName1}`)" height="150" class="mr-2"/>
          <img :src="require(`@/assets/photos/${imgName2}`)" height="150" class="mr-2"/>
        </p>
        <div>
            <p :class="className">아름다운 풍경</p>
            <p :style="css">가을에는 Vue를 공부하고 싶어요.</p>
        </div>
        <hr/>
        <button class="btn btn-info btn-sm mr-2" @click="changeData1">클래스 변경</button>
         <button class="btn btn-info btn-sm" @click="changeData2">CSS 변경</button>
        </div>
    </div>

</template>

<script>

export default {
  //컴포넌트의 대표이름(dvetools에 나오는 이름)
  name: "Exam03AttriBinding",
  //추가하고 싶은 컴포넌트 등록
  components: {

  },
  //컴포넌트에서 사용하는 데이터를 정의
  data: function(){
    return {
      imgName1: "photo1.jpg",
      imgName2: "photo2.jpg",
      className: "class1",
      css: "color:blue;",
      toggle: true
    };
  },
  //컴포넌트에서 사용하는 메소드
  methods:{
    changeData1(){
      if(this.className === "class1"){
        this.className = "class2";
      }else{
        this.className = "class1";
      }
    },
        changeData2(){
      if(this.css === "color:blue;"){
        this.css = "color:red;";
      }else{
        this.css = "color:blue;";
      }
    }
    
  }
}

</script>
//컴포넌트 스타일 정의
<style scoped>
  .class1{
    color: red
  }
  .class2{
    color: green
  }
</style>

