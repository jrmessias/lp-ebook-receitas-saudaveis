<script setup lang="ts">
import { Apple, UtensilsCrossed, Dumbbell, Baby, Clock } from 'lucide-vue-next'
import FaqAccordion from "./components/FaqAccordion.vue";
</script>

<template>
  <div class="min-h-screen bg-gradient-to-b from-green-50 to-green-100">
    <!-- Hero Section -->
    <section class="container mx-auto px-4 py-16 text-center">
      <h1 class="text-4xl md:text-6xl font-bold text-green-800 mb-4">
        Receitas Saudáveis para o Seu Dia a Dia
      </h1>
      <h2 class="text-xl md:text-2xl text-green-600 mb-8">
        Mais de 30 opções de receitas rápidas para café da manhã, almoço, lanche, jantar + bônus!
      </h2>
      <button class="bg-orange-500 hover:bg-orange-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out transform hover:scale-105">
        Clique aqui para baixar e se tornar um chef saudável!
      </button>
    </section>

    <!-- eBook Presentation -->
    <section class="bg-white py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-green-700 mb-6 text-center">
          Descubra receitas rápidas, fáceis e gostosas que todos vão amar!
        </h2>
        <div class="flex flex-col md:flex-row items-center justify-center mb-8">
          <img src="/assets/img/mockup.png" width="250" alt="Capa do eBook" class="rounded-lg drop-shadow-md mb-4 md:mb-0 md:mr-8" />
          <p class="text-2xl text-gray-700 max-w-2xl text-center">
            Nosso e-book tem receitas rápidas para você preparar para sua família. Imagine comer coisas gostosas e saudáveis que fazem bem para o corpo e ainda impressionam a família!
          </p>
        </div>
      </div>
    </section>

    <!-- Benefits -->
    <section class="container mx-auto px-4 py-16 bg-cover bg-center">
      <div class="bg-opacity-90 p-8 rounded-lg">
        <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-8 text-center">
          Por que você vai amar essas receitas saudáveis?
        </h2>
        <ul class="space-y-4 max-w-2xl mx-auto">
          <li class="flex items-center text-2xl text-green-700">
            <Apple class="h-8 w-8 mr-4 text-red-500" />
            Comidas rápidas, gostosas e saudáveis!
          </li>
          <li class="flex items-center text-2xl text-green-700">
            <UtensilsCrossed class="h-8 w-8 mr-4 text-orange-500" />
            Receitas fáceis para fazer junto com sua família!
          </li>
          <li class="flex items-center text-2xl text-green-700">
            <Dumbbell class="h-8 w-8 mr-4 text-blue-500" />
            Faz bem para o corpo e a saúde!
          </li>
          <li class="flex items-center text-2xl text-green-700">
            <Clock class="h-8 w-8 mr-4 text-red-500" />
            Receitas rápidas para todos horários!
          </li>
          <li class="flex items-center text-2xl text-green-700">
            <Baby class="h-8 w-8 mr-4 text-orange-500" />
            Receitas para todas idades!
          </li>
        </ul>
      </div>
    </section>

    <!-- Testimonials -->
    <section class="bg-green-50 py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-8 text-center">
          Veja o que as pessoas que já baixaram dizem!
        </h2>
<!--        <TestimonialCarousel />-->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <div class="bg-white p-6 rounded-lg shadow-md">
            <div class="flex items-center mb-4">
              <div>
                <h3 class="font-bold text-lg">Ana Carolina</h3>
                <p class="text-green-600">Estudante universitária</p>
              </div>
            </div>
            <p class="text-gray-700">"As receitas são deliciosas e práticas e facilitou muito o meu dia a dia!"</p>
          </div>
          <div class="bg-white p-6 rounded-lg shadow-md">
            <div class="flex items-center mb-4">
              <div>
                <h3 class="font-bold text-lg">Vitor Hugo</h3>
                <p class="text-green-600">Pai e entusiasta da culinária</p>
              </div>
            </div>
            <p class="text-gray-700">"Nunca pensei que comer saudável fosse tão gostoso! Tem receita para toda família!"</p>
          </div>
        </div>
      </div>
    </section>

    <!-- About the Author -->
<!--    <section class="container mx-auto px-4 py-16">-->
<!--      <div class="flex flex-col md:flex-row items-center justify-center">-->
<!--        <img src="https://placeholder.pics/svg/200" alt="Foto do Nutricionista" class="rounded-full shadow-lg mb-6 md:mb-0 md:mr-8" />-->
<!--        <div class="md:max-w-2xl">-->
<!--          <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-6 text-center md:text-left">-->
<!--            Feito por um Nutricionista Especialista em Comida Saudável!-->
<!--          </h2>-->
<!--          <p class="text-lg text-gray-700 text-center md:text-left">-->
<!--            Sou um nutricionista que adora criar receitas fáceis e saborosas. Minha missão é ajudar você e sua família a comerem melhor e com mais alegria!-->
<!--          </p>-->
<!--        </div>-->
<!--      </div>-->
<!--    </section>-->

    <!-- Special Offer -->
    <section class="bg-orange-100 py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-orange-800 mb-6 text-center">
          Baixe Hoje e Ganhe um Super Bônus!
        </h2>
        <p class="text-lg text-orange-700 max-w-3xl mx-auto text-center mb-8">
          Se você baixar agora, também vai receber um plano de refeições semanal para organizar suas refeições saudáveis!
        </p>
      </div>
    </section>

    <!-- 7-Day Guarantee Section -->
    <section class="bg-white py-16">
      <div class="container mx-auto px-4">
        <div class="flex flex-col md:flex-row items-center justify-center">
          <img src="/assets/img/selo7dias.png" width="250" alt="Selo de Garantia de 7 Dias" class="mb-8 md:mb-0 md:mr-8" />
          <div class="md:max-w-2xl">
            <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-6 text-center md:text-left">
              Garantia de Satisfação de 7 Dias
            </h2>
            <p class="text-lg text-gray-700 text-center md:text-left mb-4">
              Estamos tão confiantes de que você vai adorar nosso e-book de receitas saudáveis que oferecemos uma garantia de satisfação de 7 dias.
            </p>
            <p class="text-lg text-gray-700 text-center md:text-left">
              Se por qualquer motivo você não estiver completamente satisfeito com o conteúdo, basta solicitar o reembolso dentro de 7 dias após a compra, e nós reembolsaremos 100% do seu investimento, sem perguntas!
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- FAQ Section -->
    <section class="bg-white py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-8 text-center">
          Perguntas Frequentes
        </h2>
        <FaqAccordion />
      </div>
    </section>

    <!-- Call to Action -->
    <section class="container mx-auto px-4 py-16 text-center">
      <h2 class="text-3xl md:text-4xl font-bold text-green-800 mb-8">
        Vamos Começar?
      </h2>
      <button class="bg-orange-500 hover:bg-orange-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out transform hover:scale-105 text-xl">
        Baixe Seu E-book Agora!
      </button>
    </section>
  </div>

  <!-- Footer -->
  <footer class="bg-green-800 text-white py-8">
    <div class="container mx-auto px-4 text-center">
      <p>&copy; {{ new Date().getFullYear() }} Melli Criações. Todos os direitos reservados.</p>
    </div>
  </footer>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

body {
  font-family: 'Poppins', sans-serif;
}
</style>
