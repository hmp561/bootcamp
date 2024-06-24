<template>
  <main>
    <img src="/logo2.svg" alt="DFINITY logo" />
    <br />
    <br />
    <form action="#" @submit="handleSubmit">
      <label for="name">Enter your name: &nbsp;</label>
      <input id="name" alt="Name" type="text" />
      <button type="submit">Click Me!</button>
    </form>
    <section id="greeting">hello world
      <br>
      {{ licznik }}
      <br><button @click="podbij">podbij</button>
    </section>
    
  </main>
</template>

<script>
  export default{
    data(){
      return{
        licznik: 0
      }
    },
    methods: {
      podbij(){
        this.licznik++
      }
    }
  }

</script>