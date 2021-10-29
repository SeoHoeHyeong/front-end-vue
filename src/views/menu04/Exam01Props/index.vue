<!-- 컴포넌트 UI 정의-->
<template>
    <div class = "card">
      <div class = "card-header">
        Exam01Props
        </div>
      <div class = "card-body">
        <child-a  :prop1="data1"
                  prop2="value2"
                  productNo="1"
                  productKind="bag"
                  :productPrice="1000"
        ></child-a>
        </div>
    </div>

</template>

<script>
import ChildA from "./ChildA.vue";
export default {
  //컴포넌트의 대표이름(dvetools에 나오는 이름)
  name: "Exam01Props",
  //추가하고 싶은 컴포넌트 등록
  components: {
    ChildA
  },
  //컴포넌트에서 사용하는 데이터를 정의
  data: function(){
    return {
      data1: "1"
    };
  },
  //컴포넌트에서 사용하는 메소드
  methods:{

  }
}

</script>
//컴포넌트 스타일 정의
<style scoped>

</style>

