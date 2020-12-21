<template>
  <div>
      <span v-html='rawHTML'></span>
      MVC 패턴에서 컨트롤러는 모델의 데이터를 조회하거나 업데이트 하는 역할을 하며, 모델의 변화는 뷰에 반영
      모델 : 애플리케이션의 데이터를 의미한다. 모델이 변경 될 경우 컨트롤러와 뷰에 통보하여 컨트롤러와 뷰가 알고 있는 데이터를 갱신 할 수 있도록 한다.
      뷰 : 사용자에게 제공되는  UI 인터페이스를 제공한다
      컨트롤러 : 모델의 상태를 변경하는 대부분의 로직을 의미한다.

      Flux 패턴
      MVC패턴을 가진 애플리케이션이 커지면 커질수록 상태관리의 흐름이 너무 복잡해지는 것을 해결하고자 만든 패턴
      데이터의 흐름이 양방향이 아닌 단방향으로 흐른다는 것
      Action, Dispatcher ,Store, View순으로 흐른다...
  </div>
</template>

<script>
export default {
data(){
    return {
        rawHTML : '<span style="color: red">Hello</span>'
    }
}
}
</script>

<style>

</style>