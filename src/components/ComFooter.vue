<template>
  <footer class="bg-gray-100 text-gray-700 py-6 mt-8 border-t">
    <div class="max-w-6xl mx-auto px-4 grid grid-cols-1 md:grid-cols-3 gap-6">
      
      <!-- Cột 1: Logo và mô tả -->
      <div>
        <h2 class="text-xl font-bold text-red-600 mb-2">Vietnam is awesome</h2>
        <p class="text-sm">
          Chúng tôi mang đến những sản phẩm và trải nghiệm tuyệt vời cho bạn trên khắp Việt Nam.
        </p>
      </div>

      <!-- Cột 2: Liên kết nhanh -->
      <div>
        <h3 class="text-lg font-semibold mb-2">Liên kết</h3>
        <ul class="space-y-1 text-sm">
          <li><router-link to="/" class="hover:text-red-600">Trang chủ</router-link></li>
          <li><router-link to="/about" class="hover:text-red-600">Về chúng tôi</router-link></li>
          <li><router-link to="/products" class="hover:text-red-600">Sản phẩm</router-link></li>
          <li><router-link to="/contact" class="hover:text-red-600">Liên hệ</router-link></li>
        </ul>
      </div>

      <!-- Cột 3: Thông tin liên hệ -->
      <div>
        <h3 class="text-lg font-semibold mb-2">Liên hệ</h3>
        <p class="text-sm">Hotline: 0123-456-789</p>
        <p class="text-sm">Email: info@example.com</p>
        <p class="text-sm">Địa chỉ: 123 Đường ABC, Quận 1, TP.HCM</p>
      </div>
    </div>

    <!-- Dòng dưới cùng -->
    <div class="text-center text-xs text-gray-500 mt-6">
      &copy; {{ new Date().getFullYear() }} Vietnam is awesome. All rights reserved.
    </div>
  </footer>
</template>

<script setup>
// Không cần script nếu không có logic động
</script>

<style scoped>
/* Bạn có thể thêm các hiệu ứng nếu cần */
</style>
