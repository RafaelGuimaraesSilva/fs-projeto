<template>
  <div class="min-h-screen bg-background">
    <!-- Header -->
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
        </nav>
        <button class="btn btn-primary btn-md">Saiba Mais</button>
      </div>
    </header>

    <!-- Hero Section -->
    <section class="py-20 px-4 bg-gradient-to-br from-card to-background">
      <div class="container mx-auto text-center max-w-4xl">
        <span class="badge bg-secondary/10 text-secondary border border-secondary/20 mb-6">
          Futuro Sustentável
        </span>
        <h2 class="text-5xl md:text-6xl font-bold mb-6 text-balance">
          Energia Limpa e <span class="text-primary">Acessível</span> para Todos
        </h2>
        <p class="text-xl text-muted-foreground mb-8 text-pretty max-w-2xl mx-auto">
          Descubra como a energia renovável está transformando o mundo e criando um futuro mais sustentável e
          econômico para todas as comunidades.
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <button class="btn btn-primary btn-lg">
            <Sun class="mr-2 h-5 w-5" />
            Explorar Soluções
          </button>
          <button class="btn btn-outline btn-lg">
            <Globe class="mr-2 h-5 w-5" />
            Ver Impacto Global
          </button>
        </div>
      </div>
    </section>

    <!-- Tipos de Energia -->
    <section id="tipos" class="py-20 px-4">
      <div class="container mx-auto">
        <div class="text-center mb-16">
          <h3 class="text-4xl font-bold mb-4">Tipos de Energia Limpa</h3>
          <p class="text-xl text-muted-foreground max-w-2xl mx-auto">
            Conheça as principais fontes de energia renovável que estão moldando o futuro energético mundial
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="card p-6 hover:shadow-lg transition-shadow">
            <div class="mb-4">
              <Sun class="h-12 w-12 text-primary mb-4" />
              <h4 class="text-xl font-semibold mb-2">Energia Solar</h4>
              <p class="text-muted-foreground mb-4">Aproveitamento da luz solar através de painéis fotovoltaicos</p>
            </div>
            <ul class="space-y-2 text-sm text-muted-foreground">
              <li>• Redução de até 90% na conta de luz</li>
              <li>• Tecnologia cada vez mais acessível</li>
              <li>• Manutenção mínima necessária</li>
              <li>• Vida útil de 25+ anos</li>
            </ul>
          </div>

          <div class="card p-6 hover:shadow-lg transition-shadow">
            <div class="mb-4">
              <Wind class="h-12 w-12 text-secondary mb-4" />
              <h4 class="text-xl font-semibold mb-2">Energia Eólica</h4>
              <p class="text-muted-foreground mb-4">Geração de eletricidade através da força dos ventos</p>
            </div>
            <ul class="space-y-2 text-sm text-muted-foreground">
              <li>• Uma das fontes mais baratas</li>
              <li>• Não produz poluição</li>
              <li>• Aproveitamento de áreas rurais</li>
              <li>• Crescimento exponencial no Brasil</li>
            </ul>
          </div>

          <div class="card p-6 hover:shadow-lg transition-shadow">
            <div class="mb-4">
              <Leaf class="h-12 w-12 text-chart-1 mb-4" />
              <h4 class="text-xl font-semibold mb-2">Biomassa</h4>
              <p class="text-muted-foreground mb-4">Energia obtida através de materiais orgânicos</p>
            </div>
            <ul class="space-y-2 text-sm text-muted-foreground">
              <li>• Aproveitamento de resíduos</li>
              <li>• Geração contínua de energia</li>
              <li>• Reduz impacto ambiental</li>
              <li>• Fortalece economia local</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Benefícios -->
    <section id="beneficios" class="py-20 px-4 bg-card/30">
      <div class="container mx-auto">
        <div class="text-center mb-16">
          <h3 class="text-4xl font-bold mb-4">Por Que Energia Limpa?</h3>
          <p class="text-xl text-muted-foreground max-w-2xl mx-auto">
            Os benefícios vão muito além da economia na conta de luz
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="text-center">
            <div class="bg-primary/10 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <TrendingUp class="h-8 w-8 text-primary" />
            </div>
            <h4 class="text-xl font-semibold mb-2">Economia</h4>
            <p class="text-muted-foreground">Redução significativa nos custos de energia a longo prazo</p>
          </div>

          <div class="text-center">
            <div class="bg-secondary/10 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <Leaf class="h-8 w-8 text-secondary" />
            </div>
            <h4 class="text-xl font-semibold mb-2">Sustentabilidade</h4>
            <p class="text-muted-foreground">Zero emissões de gases poluentes durante a operação</p>
          </div>

          <div class="text-center">
            <div class="bg-chart-1/10 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <Users class="h-8 w-8 text-chart-1" />
            </div>
            <h4 class="text-xl font-semibold mb-2">Acessibilidade</h4>
            <p class="text-muted-foreground">Democratização do acesso à energia limpa</p>
          </div>

          <div class="text-center">
            <div class="bg-chart-4/10 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <Heart class="h-8 w-8 text-chart-4" />
            </div>
            <h4 class="text-xl font-semibold mb-2">Saúde</h4>
            <p class="text-muted-foreground">Melhoria da qualidade do ar e saúde pública</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Estatísticas -->
    <section id="impacto" class="py-20 px-4">
      <div class="container mx-auto">
        <div class="text-center mb-16">
          <h3 class="text-4xl font-bold mb-4">Impacto Global</h3>
          <p class="text-xl text-muted-foreground max-w-2xl mx-auto">
            Números que mostram a revolução energética em curso
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="card text-center p-6">
            <div class="text-4xl font-bold text-primary mb-2">85%</div>
            <p class="text-muted-foreground">Redução no custo da energia solar na última década</p>
          </div>

          <div class="card text-center p-6">
            <div class="text-4xl font-bold text-secondary mb-2">12M</div>
            <p class="text-muted-foreground">Empregos criados no setor de energias renováveis</p>
          </div>

          <div class="card text-center p-6">
            <div class="text-4xl font-bold text-chart-1 mb-2">30%</div>
            <p class="text-muted-foreground">Da matriz energética mundial já é renovável</p>
          </div>

          <div class="card text-center p-6">
            <div class="text-4xl font-bold text-chart-4 mb-2">2030</div>
            <p class="text-muted-foreground">Meta para triplicar a capacidade renovável global</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to Action -->
    <section class="py-20 px-4 bg-primary/5">
      <div class="container mx-auto text-center max-w-3xl">
        <h3 class="text-4xl font-bold mb-6">Faça Parte da Mudança</h3>
        <p class="text-xl text-muted-foreground mb-8">
          Junte-se a milhões de pessoas ao redor do mundo que já escolheram um futuro mais limpo e sustentável
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <button class="btn btn-primary btn-lg">
            <Zap class="mr-2 h-5 w-5" />
            Calcular Economia
          </button>
          <button class="btn btn-outline btn-lg border-secondary text-secondary hover:bg-secondary/10">
            Encontrar Fornecedores
          </button>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 px-4 border-t border-border">
      <div class="container mx-auto text-center">
        <div class="flex items-center justify-center gap-2 mb-4">
          <Zap class="h-6 w-6 text-primary" />
          <span class="text-xl font-bold">EnergiAcessível</span>
        </div>
        <p class="text-muted-foreground mb-4">Promovendo energia limpa e acessível para um futuro sustentável</p>
        <div class="flex justify-center gap-6 text-sm text-muted-foreground">
          <a href="#" class="hover:text-primary transition-colors">
            Sobre
          </a>
          <a href="#" class="hover:text-primary transition-colors">
            Contato
          </a>
          <a href="#" class="hover:text-primary transition-colors">
            Recursos
          </a>
          <a href="#" class="hover:text-primary transition-colors">
            Blog
          </a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { 
  Zap, 
  Sun, 
  Wind, 
  Leaf, 
  Users, 
  TrendingUp, 
  Globe, 
  Heart 
} from 'lucide-vue-next'

// Meta tags para SEO
useHead({
  title: 'EnergiAcessível - Energia Limpa para Todos',
  meta: [
    { 
      name: 'description', 
      content: 'Descubra como a energia renovável está transformando o mundo e criando um futuro mais sustentável e econômico para todas as comunidades.' 
    }
  ]
})
</script>

