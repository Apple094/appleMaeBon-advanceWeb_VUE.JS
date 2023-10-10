<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const Book = ref('')

</script>
<template>
  <div class="p-3 mb-2 bg-secondary text-white">
<blockquote class="blockquote"><h1>List of Books</h1></blockquote>
    <select v-model="Book" class="form-select" aria-label="Default select example">
        <option value="bok1">To Kill a Mockingbird</option>
        <option value="bok2">1984</option>
        <option value="bok3">Pride and Prejudice</option>
        <option value="bok4">The Great Gatsby</option>
        <option value="bok5">The Catcher in the Rye</option>
        <option value="bok6">The Hobbit</option>
        
       
    </select>
    <p v-if="Book == 'bok1'">
      <h5>To Kill a Mockingbird </h5>
    <p>Date Published: 1960</p>
    <p>Author: Harper Lee</p>
    <p>Number of Pages: 281</p>
    <p>Category: Fiction</p>
    </p>
    <p v-if="Book == 'bok2'">
      <h5>1984</h5>
    <p>Date Published: 1949</p>
    <p>Author: George Orwell</p>
    <p>Number of Pages: 328</p>
    <p>Category: Science Fiction/Dystopian</p>
  </p>
  <p v-if="Book == 'bok3'">
    <h5>Pride and Prejudice</h5>
    <p>Date Published: 1813</p>
    <p>Author: Jane Austen</p>
    <p>Number of Pages: 432</p>
    <p>Category: Classic Literature/Romance</p>
  </p>
  <p v-if="Book == 'bok4'">
    <h5>The Great Gatsby</h5>
    <p>Date Published: 1925</p>
    <p>Author: F. Scott Fitzgerald</p>
    <p>Number of Pages: 180</p>
    <p>Category: Fiction/Literary</p>
  </p>
  <p v-if="Book == 'bok5'">
    <h5>The Catcher in the Rye</h5>
    <p>Date Published: 1951</p>
    <p>Author: J.D. Salinger</p>
    <p>Number of Pages: 224</p>
    <p>Category: Fiction/Coming-of-Age</p>
  </p>
  <p v-if="Book == 'bok6'">
    <h5>The Hobbit</h5>
    <p>Date Published: 1937</p>
    <p>Author: J.R.R. Tolkien</p>
    <p>Number of Pages: 310</p>
    <p>Category: Fantasy/Adventure</p>
  </p>
</div>
    <!-- <p v-else>3</p> -->
</template>