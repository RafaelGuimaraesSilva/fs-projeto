<template>
  <div class="min-h-screen flex items-center justify-center bg-background">
    <div class="max-w-md w-full space-y-8 p-8 bg-card rounded-lg shadow-lg">
      <div>
        <h2 class="mt-6 text-center text-3xl font-bold text-foreground">
          Entre na sua conta
        </h2>
      </div>
      <form class="mt-8 space-y-6" @submit.prevent="handleLogin">
        <div class="rounded-md shadow-sm -space-y-px">
          <div>
            <label for="email" class="sr-only">Email</label>
            <input
              id="email"
              v-model="email"
              name="email"
              type="email"
              required
              class="appearance-none rounded-none relative block w-full px-3 py-2 border border-muted placeholder-muted-foreground text-foreground rounded-t-md focus:outline-none focus:ring-primary focus:border-primary focus:z-10 sm:text-sm"
              placeholder="Email"
            />
          </div>
          <div>
            <label for="password" class="sr-only">Senha</label>
            <input
              id="password"
              v-model="password"
              name="password"
              type="password"
              required
              class="appearance-none rounded-none relative block w-full px-3 py-2 border border-muted placeholder-muted-foreground text-foreground rounded-b-md focus:outline-none focus:ring-primary focus:border-primary focus:z-10 sm:text-sm"
              placeholder="Senha"
            />
          </div>
        </div>

        <div>
          <button
            type="submit"
            class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-primary hover:bg-primary/90 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary"
          >
            Entrar
          </button>
        </div>
      </form>
      
      <div class="text-center">
        <p class="text-sm text-muted-foreground">
          Não tem uma conta?
          <NuxtLink to="/register" class="font-medium text-primary hover:text-primary/90">
            Registre-se
          </NuxtLink>
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
const email = ref('');
const password = ref('');
const router = useRouter();

definePageMeta({
  layout: 'default'
});

async function handleLogin() {
  try {
    const response = await fetch('http://localhost:5000/api/auth/login', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
      },
      body: JSON.stringify({
        email: email.value,
        password: password.value,
      }),
    });

    const data = await response.json();

    if (!response.ok) {
      throw new Error(data.error || 'Login failed');
    }

    // Store the token in localStorage
    localStorage.setItem('token', data.token);
    localStorage.setItem('user', JSON.stringify(data.user));

    // Redirect to home page
    router.push('/');
  } catch (error) {
    console.error('Login error:', error);
    alert(error.message);
  }
}
</script>
