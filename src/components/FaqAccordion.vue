<template>
  <div class="space-y-4">
    <article
      v-for="(item, index) in faqItems"
      :key="item.question"
      class="overflow-hidden rounded-2xl border border-[color:var(--line)] bg-white shadow-[var(--shadow-soft)]"
    >
      <h3>
        <button
          :id="`faq-trigger-${index}`"
          type="button"
          class="flex w-full items-center justify-between gap-4 px-5 py-4 text-left transition-colors duration-200 hover:bg-[color:var(--surface-2)] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[color:var(--leaf-soft)] md:px-6 md:py-5"
          :aria-expanded="openIndex === index"
          :aria-controls="`faq-panel-${index}`"
          @click="toggleItem(index)"
        >
          <span class="text-base font-semibold text-[color:var(--ink)] md:text-lg">{{ item.question }}</span>
          <ChevronDown
            class="h-5 w-5 shrink-0 text-[color:var(--leaf)] transition-transform duration-200"
            :class="{ 'rotate-180': openIndex === index }"
          />
        </button>
      </h3>
      <transition name="faq-expand">
        <div
          v-show="openIndex === index"
          :id="`faq-panel-${index}`"
          role="region"
          :aria-labelledby="`faq-trigger-${index}`"
          class="border-t border-[color:var(--line)] bg-[color:var(--surface)] px-5 py-4 md:px-6 md:py-5"
        >
          <p class="leading-relaxed text-[color:var(--ink-soft)]">{{ item.answer }}</p>
        </div>
      </transition>
    </article>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { ChevronDown } from 'lucide-vue-next'

type FaqItem = {
  question: string
  answer: string
}

  const faqItems: FaqItem[] = [
  {
    question: 'Quantas receitas estão incluídas no e-book?',
    answer: 'O e-book contém mais de 30 receitas saudáveis, incluindo opções para café da manhã, almoço, lanche e jantar, além de receitas bônus.'
  },
  {
    question: 'As receitas são adequadas para iniciantes na cozinha?',
    answer: 'Sim. Todas as receitas foram pensadas para serem simples de executar, com etapas claras para iniciantes e práticas para quem já cozinha.'
  },
  {
    question: 'Quais informações cada receita possui?',
    answer: 'Cada receita inclui ingredientes, modo de preparo, tempo estimado e porção, para facilitar o planejamento da rotina alimentar.'
  },
  {
    question: 'Como recebo o e-book após a compra?',
    answer: 'Após a confirmação do pagamento, você recebe um e-mail com o link para baixar o e-book em PDF e acessar o bônus em qualquer dispositivo.'
  },
  {
    question: 'E se eu ainda tiver dúvidas?',
    answer: 'Você pode enviar sua dúvida pelo formulário de contato indicado no material e receber orientação para aproveitar melhor o conteúdo.'
  },
  {
    question: 'Este e-book terá atualizações?',
    answer: 'Sim. Esta é a primeira versão em valor promocional. Novas atualizações poderão ser adicionadas em versões futuras.'
  }
]

const openIndex = ref<number | null>(0)

const toggleItem = (index: number) => {
  openIndex.value = openIndex.value === index ? null : index
}
</script>

<style scoped>
.faq-expand-enter-active,
.faq-expand-leave-active {
  transition: opacity 0.2s ease, transform 0.2s ease;
}

.faq-expand-enter-from,
.faq-expand-leave-to {
  opacity: 0;
  transform: translateY(-4px);
}
</style>
