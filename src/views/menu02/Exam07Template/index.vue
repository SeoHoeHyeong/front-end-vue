<!-- 컴포넌트 UI 정의-->
<template>
    <div class = "card">
      <div class = "card-header">
        Exam07Template
        </div>
      <div class = "card-body">
        <button class="btn btn-info btn-sm mr-2" @click="ModalDialogTemplate=true">Show ModalDialogTemplate</button>
        <button class="btn btn-info btn-sm mr-2" @click="DialogA=true">Show DialogA</button>
        <button class="btn btn-info btn-sm mr-2" @click="DialogB=true">Show DialogB</button>
       </div>
        <modal-dialog-template v-if="ModalDialogTemplate" @close="ModalDialogTemplate=false"/>
        <dialog-a v-if="DialogA" @close="DialogA=false"/>
         <dialog-b v-if="DialogB" @close="DialogB=false"/>
    </div>

</template>

<script>
import ModalDialogTemplate from "@/components/menu02/ModalDialogTemplate.vue"
import DialogA from "./DialogA.vue";
import DialogB from "./DialogB.vue";
export default {
  //컴포넌트의 대표이름(dvetools에 나오는 이름)
  name: "Exam07Template",
  //추가하고 싶은 컴포넌트 등록
  components: {
    ModalDialogTemplate
    ,DialogA
    ,DialogB

    
  },
  //컴포넌트에서 사용하는 데이터를 정의
  data: function(){
    return {
      ModalDialogTemplate: false,
      DialogA: false,
      DialogB: false
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

