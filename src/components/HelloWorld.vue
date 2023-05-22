<script setup>

</script>

<template>
  <el-container style="width: 60%;margin: 0 auto;">
	  <el-main>
		  <el-row v-for="(i, index1) in 4" :key="i" :span="24">
			  <el-col v-for="(j, index2) in 8" :key="`${index1}-${index2}`" :span="3">
				  <div style="aspect-ratio:1/1;width: 100%;background-color: beige;"
				  v-if="index2 % 2 === 0">
					  1
				  </div>
				  <div v-else style="aspect-ratio:1/1;width: 100%;background-color: bisque;">
					  2
				  </div>
			  </el-col>
		  </el-row>
	  </el-main>
  </el-container>
</template>

<style scoped>

</style>
