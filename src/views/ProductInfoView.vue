<template>
<div class="container">
  <h1>商品成本與售價管理</h1>
  <table>
    <thead>
      <tr>
        <th>商品名稱</th>
        <th>成本價格</th>
        <th>售價</th>
        <th>利潤</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><input type="text" id="productName1"></td>
        <td><input type="number" id="costPrice1"></td>
        <td><input type="number" id="sellingPrice1"></td>
        <td id="profit1"></td>
      </tr>
      <tr>
        <td><input type="text" id="productName2"></td>
        <td><input type="number" id="costPrice2"></td>
        <td><input type="number" id="sellingPrice2"></td>
        <td id="profit2"></td>
      </tr>
      <tr>
        <td><input type="text" id="productName3"></td>
        <td><input type="number" id="costPrice3"></td>
        <td><input type="number" id="sellingPrice3"></td>
        <td id="profit3"></td>
      </tr>
    </tbody>
  </table>
  <button >計算利潤</button>
</div>
</template>

<script>
  export default {
    name: 'ProductInfoView',
    methods: {
    },
    mounted(){
    }
  }
</script>

<style>
body {
  font-family: sans-serif;
  background-image: url('https://images.unsplash.com/photo-1508701920343-80d91427d786?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTB8fGFiY3RyYWN0fGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60'); /* Unsplash background image */
  background-size: cover;
  background-attachment: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  margin: 0;
}

.container {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: left;
}

th {
  background-color: #f2f2f2;
}

input[type="number"] {
  width: 100px;
}
</style>