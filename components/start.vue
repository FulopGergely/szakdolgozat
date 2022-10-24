<template>
  <div class="w-100 p-4 d-flex align-items-center justify-content-center">
    <b-container fluid>
      <b-row>
        <b-col>
          <b class="d-flex justify-content-center">Javascript</b>
          <NuxtLink :to="'/javascript/${id[0]}'">
            <b-img
              class="w-50 p-3" center fluid
              src="JavaScript.png"
              alt="Image 1">
            </b-img>
          </NuxtLink>
        </b-col>
        <b-col>
          <b class="d-flex justify-content-center">Python</b>
          <b-img @click="asd" class="w-50 p-3" center fluid src="Python.png" alt="Image 2"></b-img>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "start",
  methods: {
    asd(){
      console.log(this.id);
    },
    data(){
      const id = [1,2];
      return {
        id,
      }
    }
  }
}
</script>

<style scoped>

</style>
