<template>
  <div>
    <NuxtLayout>
      <NuxtLoadingIndicator />
      <!-- Optional: loading indicator -->
      <NuxtPage />
    </NuxtLayout>

    <!-- Optional: error handling -->
    <NuxtErrorBoundary>
      <template #error="{ error }">
        <div class="container mx-auto px-4 py-8">
          <h1 class="text-2xl font-bold text-red-600">Terjadi kesalahan</h1>
          <p>{{ error }}</p>
          <button
            class="mt-4 px-4 py-2 bg-blue-500 text-white rounded"
            @click="error.value = null"
          >
            Coba lagi
          </button>
        </div>
      </template>
    </NuxtErrorBoundary>
  </div>
</template>
