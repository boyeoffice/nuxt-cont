<template>
  <div class="main">
    <div class="wrapper">
      <form @submit.pevent="handleSubmit">
        <div class="form-group">
          <input type="text" class="form-control" v-model="form.name" placeholder="Full name">
        </div>
        <div class="form-group">
          <input type="email" class="form-control" v-model="form.email" placeholder="Email address">
        </div>
        <div class="form-group">
          <input type="password" class="form-control" placeholder="Password">
        </div>
        <button type="submit" class="btn">Create</button>
      </form>
    </div>
  </div>
</template>

<script>

export default {
  data(){
    return{
      form:{}
    }
  },
  methods: {
    async handleSubmit(){
      console.log('Hurray it works')
    }
  }
}
</script>

<style>
.main {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
}
.wrapper {
  width: 400px;
  margin: 0 auto;
  background: #ccc;
  padding: 15px;
}
.form-group {
  padding: 0 0 10px 0;
}
.form-control {
  width: 100%;
  height: 40px;
  color: #000;
}
.btn {
  width: 100%;
  height: 40px;
  display: block;
  background: #0333cc;
  border: #0333cc solid 1px;
  color: #fff;
}
</style>
