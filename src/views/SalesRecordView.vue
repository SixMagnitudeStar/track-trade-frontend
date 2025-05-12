<template>
<form>
  <label for="datetime">日期 & 時間:</label>
  <input type="datetime-local" id="datetime" name="datetime" required>

  <label for="item">商品:</label>
  <input type="text" id="item" name="item" required>

  <label for="quantity">數量:</label>
  <input type="number" id="quantity" name="quantity" min="1" required>

  <label for="price">價格:</label>
  <input type="number" id="price" name="price" min="0" step="0.01" required>

  <button type="submit">送出</button>
</form>
</template>
<script>
 export default{
    name: 'SalesRecordView'
 }

</script>

<style>
form {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
  display: block;
  margin-bottom: 5px;
}

input[type="text"],
input[type="datetime-local"],
input[type="number"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
  box-sizing: border-box;
}

button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}

button:hover {
  background-color: #45a049;
}
</style>