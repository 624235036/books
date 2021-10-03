<template>
    <div class="book-item">
        <h1>{{book.title}}</h1><br/>
        <img v-bind:src="book.thumbnailUrl" /><br/>
        <b>author:</b> {{book.author}} <br/>
        <b>category:</b> {{book.category}} <br/>
        <b>ISBN:</b> {{book.isbn}} <br/>
        <b>pages:</b> {{book.pageCount}} <br/><br/>
        <b>Description:</b><br/>
        <p>{{book.shortDescription}}</p>
    </div>
</template>

<script>


export default {
  name: 'BookItem',
  components: {

  },
    props:["book"]
}
</script>

<style>
.book-item{
    width: 70%;
    background: #f4f4ff;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}
</style>