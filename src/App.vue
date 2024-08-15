<template>
  <div class="flex flex-col items-center justify-center min-h-screen bg-gray-100 p-8">
    <h1 class="text-4xl font-extrabold text-gray-900 mb-8 text-center">
      Abstract Tezkunda Ismogroup
      <span class="dot dot1">.</span>
      <span class="dot dot2">.</span>
      <span class="dot dot3">.</span>
    </h1>
    <div class="flex items-center justify-center">
      <img src="/logo.png" alt="Logo" class="rounded-full w-40 h-40 border-4 border-gray-900 shadow-lg wave-effect" />
    </div>
  </div>
</template>

<style scoped>
/* Animatsiya qo'shish */
@keyframes wave {
  0% { transform: scale(0.8); }
  50% { transform: scale(1); }
  100% { transform: scale(0.8); }
}

.wave-effect {
  animation: wave 2s infinite ease-in-out;
}

/* Rangli nuqtalar uchun animatsiya */
@keyframes dot-flashing {
  0% { color: #000000; }
  25% { color: #000000; }
  50% { color: #2b00ff; }
  75% { color: #ff0000; }
  100% { color: #000000; }
}

.dot {
  font-size: 2rem; /* Nuqtalarni kattalashtirish */
  display: inline-block;
  animation-duration: 1.5s;
  animation-timing-function: ease-in-out;
  animation-iteration-count: infinite;
}

/* Har bir nuqtaning rang o'zgarishini boshqarish */
.dot1 {
  animation-name: dot-flashing;
}

.dot2 {
  animation-name: dot-flashing;
  animation-delay: 0.5s; /* Ikkinchi nuqta kechikish bilan boshlanadi */
}

.dot3 {
  animation-name: dot-flashing;
  animation-delay: 1s; /* Uchinchi nuqta yana kechikish bilan boshlanadi */
}
</style>
