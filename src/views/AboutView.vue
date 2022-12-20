<template>
  <div class="about">
    <h1>SCSS TEST {{ selected }}</h1>

    <el-row :gutter="20">
      <el-col :span="6" :offset="6">
        <select v-model="selected">
          <option disabled value="">Please select one</option>
          <option>A</option>
          <option>B</option>
          <option>C</option>
        </select>
      </el-col>
      <el-col :span="6">
        <el-button class="qs-button" type="primary" @click="increment">Count is: {{ count }}</el-button>
      </el-col>
    </el-row>

    <div class="qs-text">
      <label class="qs-text__label active-label">사원명</label>
      <div class="qs-text__input active-label-form el-input el-input--medium">
        <input type="text" placeholder="Please input" minlength="0" maxlength="Infinity" class="el-input__inner" />
      </div>
    </div>
  </div>
</template>

<script>
</script>

<!-- <style scoped>
.wrap {
  width: 100vw;
  height: 50vh;
  background-color: $qs-color-theme-20;
}
</style> -->
