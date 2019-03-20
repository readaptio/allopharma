<template>
  <div class="home">
      <h1>{{msg}}</h1>
    <search
        source="https://jsonplaceholder.typicode.com/posts"
        placeholder="What TV Serie you are looking for... Now!"
        filter-key="body"
        :start-at="2"
        >
    </search>   
  </div>
  
</template>

<script>
import Search from './Search.vue';

export default {
  name: 'Home',
  
  data () {
    return {
      msg: 'Welcome to Your First Vue.js Home App Example',
      series: [
                    { id: 1, title: 'Game of Thrones', body: 'You know nothing, Jon Snow' },
                    { id: 2, title: 'Suits', body: 'You always have a choice'  },
                    { id: 3, title: 'Dr House', body: 'If nobody hates you, you are doing something wrong' },
                    { id: 4, title: 'Breaking Bad', body: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry' },
                    { id: 5, title: 'Arrow', body: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry' },
                    { id: 6, title: 'Silicon Valley', body: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry' }
                ]
    }
  },
  components : { Search },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.home {
  font-size: 1em;
}

</style>
