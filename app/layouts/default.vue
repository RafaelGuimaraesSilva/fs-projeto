<template>
  <div class="min-h-screen bg-background">
    <header class="border-b border-border bg-card/50 backdrop-blur-sm sticky top-0 z-50">
      <div class="container mx-auto px-4 py-4 flex items-center justify-between">
        <div class="flex items-center gap-2">
          <Zap class="h-8 w-8 text-primary" />
          <h1 class="text-2xl font-bold text-foreground">EnergiAcessível</h1>
        </div>
        <nav class="hidden md:flex items-center gap-6">
          <a href="#sobre" class="text-muted-foreground hover:text-primary transition-colors">
            Sobre
          </a>
          <a href="#tipos" class="text-muted-foreground hover:text-primary transition-colors">
            Tipos
          </a>
          <a href="#beneficios" class="text-muted-foreground hover:text-primary transition-colors">
            Benefícios
          </a>
          <a href="#impacto" class="text-muted-foreground hover:text-primary transition-colors">
            Impacto
          </a>
          <NuxtLink to="/login" class="text-muted-foreground hover:text-primary transition-colors">
            Login
          </NuxtLink>
        </nav>
      </div>
    </header>
    
    <slot />
  </div>
</template>

<script setup>
import { Zap } from 'lucide-vue-next'
</script>
