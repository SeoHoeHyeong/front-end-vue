<!-- 컴포넌트 UI 정의-->
<template>
    <div class = "card">
      <div class = "card-header">
        
        <span class = "title">Exam01View</span>
        </div>
      <div class = "card-body">
        <h6>선언적 방식 화면이동(네비게이션)</h6>
        <router-link to="/menu01/exam02view" class="btn btn-info btn-sm mr-2">/menu01/exam02view</router-link>
        <router-link v-bind:to="`/menu01/exam02view`" class="btn btn-info btn-sm mr-2">/menu01/exam02view</router-link>
        <router-link :to="{path:'/menu01/exam02view'}" class="btn btn-info btn-sm mr-2">/menu01/exam02view</router-link>
        <router-link :to="{name: 'menu01_exam02view'}" class="btn btn-info btn-sm mr-2">/menu01/exam02view</router-link>
       

       <div>
         <exam-06-view prop1="value1" prop2="value2"/>
       </div>
        </div>
    </div>

</template>

<script>
import Exam06View from "./Exam06View"

export default {
  //컴포넌트의 대표이름(dvetools에 나오는 이름)
  name: "Exam01View",
  //추가하고 싶은 컴포넌트 등록
  components: {
    Exam06View
  },
  //컴포넌트에서 사용하는 데이터를 정의
  data: function(){
    return {

    };
  },
  //컴포넌트에서 사용하는 메소드
  methods:{

  }
}

</script>
//컴포넌트 스타일 정의
<style scoped>
.title{
  color: green;
}
</style>

