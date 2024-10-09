<template>
  
  <div>
    <header class="header">
      <nav class="navbar">
        <ul>
          <li><a href="#" class="active">Dashboard</a></li>
          <li><a href="#">Manager Category</a></li>
          <li><a href="#" >Manager Product</a></li>
        </ul>
      </nav>
    </header>
    <p>Đây là trang Dashboard</p>
  </div>
</template>
<script setup></script>
<style>
.header {
  background-color: #222;
  padding: 10px 20px;
  color: white;
}

.navbar {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.navbar ul {
  list-style-type: none;
  display: flex;
  gap: 20px;
}

.navbar ul li a {
  color: #fff;
  text-decoration: none;
  padding: 10px 20px;
  display: block;
  border-radius: 4px;
  transition: background-color 0.3s ease;
}

.navbar ul li a:hover,
.navbar ul li a.active {
  background-color: #444;
}

main {
  padding: 20px;
}

.header-main {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.btn-add {
  background-color: #007bff;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

table {
  width: 100%;
  border-collapse: collapse;
  background-color: white;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

table thead {
  background-color: #f1f1f1;
}

table th,
table td {
  border: 1px solid #ddd;
  padding: 10px;
  text-align: center;
}

table img {
  width: 50px;
  height: 50px;
  object-fit: cover;
}

.btn-edit {
  background-color: #f0ad4e;
  color: white;
  border: none;
  padding: 5px 10px;
  border-radius: 4px;
  cursor: pointer;
}

.btn-delete {
  background-color: #d9534f;
  color: white;
  border: none;
  padding: 5px 10px;
  border-radius: 4px;
  cursor: pointer;
  margin-left: 5px;
}

/* Responsive design */
@media (max-width: 768px) {
  .header-main {
    flex-direction: column;
    gap: 10px;
  }

  .navbar ul {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
