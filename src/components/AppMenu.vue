<template>
    <ul class="nav flex-column">
    <li class="nav-item">
      <h6 class="text-white">Vue Home</h6>
      <router-link to="/" class="nav-link text-warning">Home</router-link>
      <router-link to="/about" class="nav-link text-warning">Abount</router-link>
    </li>
    <li class="nav-item mt-2">
        <h6 class="text-white">Menu01: Routing</h6>
        <router-link to="/menu01/exam01view" class="nav-link text-warning">선언적  방식 화면(뷰) 이동</router-link>
        <router-link to="/menu01/exam02view" class="nav-link text-warning">프로그램 방식 화면(뷰) 이동</router-link>
        <router-link to="/menu01/exam03view" class="nav-link text-warning">중첩된 라우트</router-link>
        <router-link to="/menu01/exam04view" class="nav-link text-warning">이름이 있는 뷰</router-link>
        <router-link to="/menu01/exam05view" class="nav-link text-warning">URL 데이터 전달</router-link>

    </li>
    <li class="nav-item mt-2">
        <h6 class="text-white">Menu02: Component</h6>
        <router-link to="/menu02/exam01Expressions" class="nav-link text-warning">표현식 바인딩</router-link>
        <router-link to="/menu02/exam02Directives" class="nav-link text-warning">디렉티브 바인딩</router-link>
        <router-link to="/menu02/exam03AttriBinding" class="nav-link text-warning">속성 바인딩</router-link>
        <router-link to="/menu02/exam04FormBinding" class="nav-link text-warning">양방향 바인딩</router-link>
        <router-link to="/menu02/exam05ForRepeatBinding" class="nav-link text-warning">반복 바인딩</router-link>
        <router-link to="/menu02/exam06ComputedBinding" class="nav-link text-warning">계산된 바인딩</router-link>
        <router-link to="/menu02/exam07Template" class="nav-link text-warning">템플릿 컴포넌트</router-link>
    </li>
    <li class="nav-item mt-2">
        <h6 class="text-white">Menu03: EventHandling & Watch</h6>
        <router-link to="/menu03/exam01EventHandling" class="nav-link text-warning">이벤트 처리</router-link>
        <router-link to="/menu03/exam02Watch" class="nav-link text-warning">데이터 변경 감시 </router-link>
        
    </li>
        <li class="nav-item mt-2">
        <h6 class="text-white">Menu04: EventHandling & Watch</h6>
        <router-link to="/menu04/exam01Props" class="nav-link text-warning">부모에서 자식으로 전달(Props)</router-link>
    </li>
    
  </ul>
</template>