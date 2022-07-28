<template>
<p class="count">Count: <strong>{{ count }}</strong></p>

<p class="desc">Hisoblaning!</p>

<button id="plus" class="me-4 btn btn-primary" @click="increment">Count YES</button>

<button id="minus" class="ms-3 btn btn-warning" @click="decrement">count NO</button>
</template>

<script>
 export default {
 data () {
  return {
     count: 0
  }
 },
 methods: {
   increment() {
      this.count++;
   },
   decrement() {
      // this.count--;
      if(this.count > 0) {

         this.count--;
         // const elMinus = document.querySelector("#minus")
         // elMinus.setAttribute("disabled")
      }
   }
 }
 }
</script>


<style>
.message {
 margin: 0;
 padding: 0;
}

.desc {
 margin: 0;
 padding: 0;
}
</style>