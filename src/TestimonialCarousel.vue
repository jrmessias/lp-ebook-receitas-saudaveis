<template>
  <div class="relative">
    <div class="overflow-hidden">
      <div class="flex transition-transform duration-300 ease-in-out" :style="{ transform: `translateX(-${currentIndex * 100}%)` }">
        <div v-for="(testimonial, index) in testimonials" :key="index" class="w-full flex-shrink-0 px-4">
          <div class="bg-white p-6 rounded-lg shadow-md">
            <div class="flex items-center mb-4">
<!--              <img :src="testimonial.avatar" :alt="testimonial.name" class="rounded-full w-16 h-16 mr-4" />-->
              <div>
                <h3 class="font-bold text-lg">{{ testimonial.name }}</h3>
                <p class="text-green-600">{{ testimonial.title }}</p>
              </div>
            </div>
            <p class="text-gray-700">{{ testimonial.content }}</p>
          </div>
        </div>
      </div>
    </div>
    <button @click="prevSlide" class="absolute left-0 top-1/2 transform -translate-y-1/2 bg-white bg-opacity-50 hover:bg-opacity-75 rounded-full p-2 focus:outline-none" aria-label="Previous testimonial">
      <ChevronLeft class="h-6 w-6 text-green-800" />
    </button>
    <button @click="nextSlide" class="absolute right-0 top-1/2 transform -translate-y-1/2 bg-white bg-opacity-50 hover:bg-opacity-75 rounded-full p-2 focus:outline-none" aria-label="Next testimonial">
      <ChevronRight class="h-6 w-6 text-green-800" />
    </button>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue'
import { ChevronLeft, ChevronRight } from 'lucide-vue-next'

const testimonials = [
  {
    name: "Maria Silva",
    title: "Mãe de 2 filhos",
    content: "As receitas são deliciosas e fáceis de fazer. Meus filhos adoram ajudar na cozinha agora!",
    // avatar: "/placeholder.svg?height=60&width=60"
  },
  {
    name: "João Santos",
    title: "Pai e entusiasta da culinária",
    content: "Nunca pensei que comer saudável pudesse ser tão gostoso. Essas receitas mudaram nossa rotina familiar!",
    // avatar: "/placeholder.svg?height=60&width=60"
  },
  {
    name: "Ana Oliveira",
    title: "Estudante universitária",
    content: "Ótimo para quem tem pouco tempo! As receitas são rápidas e nutritivas, perfeitas para minha rotina agitada.",
    // avatar: "/placeholder.svg?height=60&width=60"
  },
  {
    name: "Carlos Mendes",
    title: "Professor e atleta amador",
    content: "As refeições são equilibradas e saborosas. Ajudaram muito no meu desempenho nos treinos!",
    // avatar: "/placeholder.svg?height=60&width=60"
  }
]

const currentIndex = ref(0)

const visibleTestimonials = computed(() => {
  return [
    testimonials[currentIndex.value],
    testimonials[(currentIndex.value + 1) % testimonials.length]
  ]
})

const nextSlide = () => {
  currentIndex.value = (currentIndex.value + 1) % testimonials.length
}

const prevSlide = () => {
  currentIndex.value = (currentIndex.value - 1 + testimonials.length) % testimonials.length
}
</script>

