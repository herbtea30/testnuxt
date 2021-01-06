<template>
  <div id="app-7">
    <ol>
      <!--
      이제 각 todo-item 에 todo 객체를 제공합니다.
      화면에 나오므로, 각 항목의 컨텐츠는 동적으로 바뀔 수 있습니다.
      또한 각 구성 요소에 "키"를 제공해야합니다 (나중에 설명 됨).
     -->
      <todo-item
        v-for="item in groceryList"
        :key="item.id"
        :todo="item"
      ></todo-item>
    </ol>
  </div>
</template>

<script>
import todoItem from '~/components/todo-item.vue'
export default {
  components: { todoItem },
  data() {
    return {
      groceryList: [
        { id: 0, text: 'Vegitables' },
        { id: 1, text: 'Cheese' },
        { id: 2, text: 'Whatever else humans are supposed to eat' },
        { id: 3, text: 'ricepaper' },
      ],
    }
  },
}
</script>

<style></style>
