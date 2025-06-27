<script setup lang="ts">
import 'mathlive'
defineProps<{ msg: string }>()
</script>

<template>
  <h1>{{ msg }}</h1>
  <div>
    <!-- 
    mathlive官网：https://cortexjs.io/mathfield/
    使用方式：步骤一：npm install mathlive
      步骤二：import 'mathlive';
      步骤三：<math-field>f(x)= x+1</math-field>
    -->
    <div class="bt10">
      <!-- 最简单的数学表达式：x + 1 -->
      <math-field>x+1</math-field>
    </div>

    <div class="bt10">
      <!-- 表达一个函数 f(x) = x + 1 -->
      <math-field>f(x)= x+1</math-field>
    </div>

    <div class="bt10">
      <!-- 一元二次方程的求根公式（经典的 quadratic formula）：
     x = [-b ± √(b² - 4ac)] / (2a) -->
      <math-field> x=\frac{-b\pm\sqrt{b^2-4ac}}{2a} </math-field>
    </div>
  </div>
</template>

<style scoped>
.text {
  text-align: left;
}

.bt10 {
  margin-bottom: 10px;
}
</style>
