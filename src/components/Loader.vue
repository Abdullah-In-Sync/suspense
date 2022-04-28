<template>
  <h1>Hello From Loader</h1>
  {{ user }}
</template>

<script>
export default{

    async setup(){
    
        const promise = new Promise((resolve, reject) => {
          setTimeout(() => {
            resolve("success");
          }, 2000);
        });
        const user = await promise;
        return {
          user,
        };
    }
}
</script>

<style>
</style>