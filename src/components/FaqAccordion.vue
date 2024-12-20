<template>
  <div class="space-y-4">
    <div v-for="(item, index) in faqItems" :key="index" class="border border-green-200 rounded-lg overflow-hidden">
      <button
          @click="toggleItem(index)"
          class="flex justify-between items-center w-full p-4 text-left bg-green-50 hover:bg-green-100 transition-colors duration-200"
      >
        <span class="font-semibold text-green-800">{{ item.question }}</span>
        <ChevronDown
            :class="{'transform rotate-180': openIndex === index}"
            class="w-5 h-5 text-green-600 transition-transform duration-200"
        />
      </button>
      <div
          v-show="openIndex === index"
          class="p-4 bg-white"
      >
        <p class="text-gray-700">{{ item.answer }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { ChevronDown } from 'lucide-vue-next'

const faqItems = [
  {
    question: "Quantas receitas estão incluídas no e-book?",
    answer: "O e-book contém mais de 30 receitas saudáveis, incluindo opções para café da manhã, almoço, lanche e jantar, além de receitas bônus."
  },
  {
    question: "As receitas são adequadas para iniciantes na cozinha?",
    answer: "Sim! Todas as receitas são projetadas para serem fáceis de seguir, com instruções passo a passo, tornando-as ideais tanto para iniciantes quanto para cozinheiros experientes."
  },
  {
  question: "Quais informações as receitas possuem?",
    answer: "Cada receita possui a lista de ingredientes e modo de preparo, além de informações de tempo para produção e porção."
  },
  {
    question: "Como recebo o e-book após a compra?",
    answer: "Após a compra, você receberá um e-mail com um link para baixar o e-book em formato PDF. Você pode salvá-lo em qualquer dispositivo para acesso fácil e offline."
  },
  {
    question: "Fiquei com dúvida! E agora?",
    answer: "Você poderá solicitar auxílio, reclamar ou contribuir no formulário de feedback no link disponível no e-book."
  },
  {
    question: "Este e-book terá atualizações?",
    answer: "Sim. Esta é primeira versão a um valor acessível, após, este e-book será atualizado e consequentemente aumentará seu valor."
  }
]

const openIndex = ref(null)

const toggleItem = (index) => {
  openIndex.value = openIndex.value === index ? null : index
}
</script>
