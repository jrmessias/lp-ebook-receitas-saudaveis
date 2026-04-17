<script setup lang="ts">
import { Apple, UtensilsCrossed, Dumbbell, Baby, Clock, ArrowRight } from 'lucide-vue-next'
import FaqAccordion from './components/FaqAccordion.vue'
</script>

<template>
  <div class="min-h-screen">
    <section class="mx-auto max-w-6xl px-4 pb-10 pt-8 md:pb-14 md:pt-14">
      <div class="section-shell overflow-hidden p-6 md:p-10">
        <div class="grid items-center gap-10 md:grid-cols-[1.1fr_0.9fr]">
          <div>
            <span class="kicker fade-up">Edição Especial 2026</span>
            <h1 class="fade-up fade-up-delay-1 mt-5 text-4xl leading-tight text-[color:var(--ink)] md:text-6xl">
              Receitas saudáveis para transformar sua rotina sem complicação
            </h1>
            <p class="fade-up fade-up-delay-2 mt-5 max-w-2xl text-lg text-[color:var(--ink-soft)] md:text-xl">
              Mais de 30 receitas práticas para café da manhã, almoço, lanche e jantar, com preparo rápido e sabor que agrada toda a família.
            </p>
            <div class="fade-up fade-up-delay-3 mt-8 flex flex-wrap items-center gap-3">
              <a href="https://pay.kiwify.com.br/PEeRXnz" target="_blank" rel="noopener noreferrer" class="cta-button text-base md:text-lg">
                Baixar agora
                <ArrowRight class="h-5 w-5" />
              </a>
              <p class="text-sm font-medium text-[color:var(--leaf)] md:text-base">
                Acesso imediato + bônus de plano semanal
              </p>
            </div>
          </div>

          <div class="relative">
            <div class="rounded-[28px] border border-[color:var(--line)] bg-[color:var(--surface)] p-5 shadow-[var(--shadow-strong)]">
              <img src="/assets/img/mockup.png" width="290" alt="Capa do eBook de receitas saudáveis" class="mx-auto" />
              <div class="mt-4 grid grid-cols-3 gap-3 text-center">
                <div class="rounded-2xl bg-[color:var(--surface-2)] px-3 py-3">
                  <p class="text-xl font-bold text-[color:var(--leaf)]">30+</p>
                  <p class="text-xs uppercase tracking-wide text-[color:var(--ink-soft)]">Receitas</p>
                </div>
                <div class="rounded-2xl bg-[color:var(--surface-2)] px-3 py-3">
                  <p class="text-xl font-bold text-[color:var(--leaf)]">7 dias</p>
                  <p class="text-xs uppercase tracking-wide text-[color:var(--ink-soft)]">Garantia</p>
                </div>
                <div class="rounded-2xl bg-[color:var(--surface-2)] px-3 py-3">
                  <p class="text-xl font-bold text-[color:var(--leaf)]">1 bônus</p>
                  <p class="text-xs uppercase tracking-wide text-[color:var(--ink-soft)]">Exclusivo</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="mx-auto max-w-6xl px-4 pb-12 md:pb-16">
      <div class="section-shell p-7 md:p-10">
        <div class="grid items-center gap-10 md:grid-cols-2">
          <div>
            <span class="kicker">Prático de verdade</span>
            <h2 class="mt-5 text-3xl text-[color:var(--ink)] md:text-5xl">
              Cozinhe melhor em menos tempo, mesmo com rotina corrida
            </h2>
            <p class="mt-5 text-lg text-[color:var(--ink-soft)]">
              O e-book foi pensado para famílias reais: receitas com ingredientes acessíveis, preparo simplificado e combinações que funcionam no dia a dia.
            </p>
            <ul class="mt-6 space-y-3 text-[color:var(--ink)]">
              <li class="rounded-2xl border border-[color:var(--line)] bg-white px-4 py-3">Receitas com passo a passo objetivo e fácil de seguir.</li>
              <li class="rounded-2xl border border-[color:var(--line)] bg-white px-4 py-3">Opções para todas as refeições, da manhã à noite.</li>
              <li class="rounded-2xl border border-[color:var(--line)] bg-white px-4 py-3">Sabores equilibrados para adultos e crianças.</li>
            </ul>
          </div>

          <div class="rounded-[28px] border border-[color:var(--line)] bg-white p-6 shadow-[var(--shadow-soft)]">
            <p class="text-sm font-bold uppercase tracking-[0.14em] text-[color:var(--leaf)]">O que você recebe</p>
            <div class="mt-5 space-y-4">
              <div class="rounded-2xl bg-[color:var(--surface-2)] p-4">
                <h3 class="text-xl text-[color:var(--ink)]">E-book completo de receitas</h3>
                <p class="mt-2 text-[color:var(--ink-soft)]">Seleção autoral com pratos saudáveis e saborosos para o cotidiano.</p>
              </div>
              <div class="rounded-2xl bg-[color:var(--surface-2)] p-4">
                <h3 class="text-xl text-[color:var(--ink)]">Bônus: plano semanal</h3>
                <p class="mt-2 text-[color:var(--ink-soft)]">Uma estrutura simples para organizar refeições sem improviso.</p>
              </div>
              <div class="rounded-2xl bg-[color:var(--surface-2)] p-4">
                <h3 class="text-xl text-[color:var(--ink)]">Acesso instantâneo</h3>
                <p class="mt-2 text-[color:var(--ink-soft)]">Comprou, recebeu no e-mail e pode usar em qualquer dispositivo.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="mx-auto max-w-6xl px-4 pb-16">
      <div class="section-shell p-7 md:p-10">
        <h2 class="text-center text-3xl text-[color:var(--ink)] md:text-5xl">
          Por que tantas famílias escolhem este e-book
        </h2>
        <div class="mt-8 grid gap-4 md:grid-cols-2 lg:grid-cols-3">
          <article class="rounded-2xl border border-[color:var(--line)] bg-white p-5">
            <Apple class="h-8 w-8 text-[#d15d4f]" />
            <h3 class="mt-4 text-xl text-[color:var(--ink)]">Saúde com prazer</h3>
            <p class="mt-2 text-[color:var(--ink-soft)]">Receitas gostosas para manter consistência sem dietas radicais.</p>
          </article>
          <article class="rounded-2xl border border-[color:var(--line)] bg-white p-5">
            <UtensilsCrossed class="h-8 w-8 text-[color:var(--accent)]" />
            <h3 class="mt-4 text-xl text-[color:var(--ink)]">Facilidade real</h3>
            <p class="mt-2 text-[color:var(--ink-soft)]">Preparos claros e acessíveis para quem não quer perder tempo.</p>
          </article>
          <article class="rounded-2xl border border-[color:var(--line)] bg-white p-5">
            <Dumbbell class="h-8 w-8 text-[#3f7cbe]" />
            <h3 class="mt-4 text-xl text-[color:var(--ink)]">Mais energia</h3>
            <p class="mt-2 text-[color:var(--ink-soft)]">Comidas equilibradas para apoiar bem-estar e rotina ativa.</p>
          </article>
          <article class="rounded-2xl border border-[color:var(--line)] bg-white p-5">
            <Clock class="h-8 w-8 text-[#c76a34]" />
            <h3 class="mt-4 text-xl text-[color:var(--ink)]">Rapidez no preparo</h3>
            <p class="mt-2 text-[color:var(--ink-soft)]">Perfeito para dias corridos, com pouco tempo para cozinhar.</p>
          </article>
          <article class="rounded-2xl border border-[color:var(--line)] bg-white p-5 md:col-span-2 lg:col-span-2">
            <Baby class="h-8 w-8 text-[color:var(--leaf)]" />
            <h3 class="mt-4 text-xl text-[color:var(--ink)]">Para todas as idades</h3>
            <p class="mt-2 text-[color:var(--ink-soft)]">Pratos pensados para agradar crianças, adultos e quem busca mais equilíbrio.</p>
          </article>
        </div>
      </div>
    </section>

<!--    <section class="mx-auto max-w-6xl px-4 pb-12 md:pb-16">-->
<!--      <div class="section-shell p-7 md:p-10">-->
<!--        <div class="flex flex-wrap items-end justify-between gap-4">-->
<!--          <div>-->
<!--            <span class="kicker">Opiniões</span>-->
<!--            <h2 class="mt-5 text-3xl text-[color:var(&#45;&#45;ink)] md:text-5xl">Quem comprou percebeu mudança nas primeiras semanas</h2>-->
<!--          </div>-->
<!--          <p class="rounded-full border border-[color:var(&#45;&#45;line)] bg-white px-4 py-2 text-sm font-semibold text-[color:var(&#45;&#45;leaf)]">Avaliação média 4.9/5</p>-->
<!--        </div>-->
<!--        <div class="mt-8 grid grid-cols-1 gap-5 md:grid-cols-2">-->
<!--          <article class="rounded-3xl border border-[color:var(&#45;&#45;line)] bg-white p-6 shadow-[var(&#45;&#45;shadow-soft)]">-->
<!--            <div class="flex items-center gap-4">-->
<!--              <div class="flex h-12 w-12 items-center justify-center rounded-full bg-[color:var(&#45;&#45;surface-2)] text-sm font-bold text-[color:var(&#45;&#45;leaf)]">AC</div>-->
<!--              <div>-->
<!--                <h3 class="text-lg font-bold text-[color:var(&#45;&#45;ink)]">Ana Carolina</h3>-->
<!--                <p class="text-sm text-[color:var(&#45;&#45;leaf-soft)]">Estudante universitária</p>-->
<!--              </div>-->
<!--            </div>-->
<!--            <p class="mt-5 text-lg leading-relaxed text-[color:var(&#45;&#45;ink-soft)]">As receitas são práticas, saborosas e finalmente consegui manter uma rotina alimentar com constância durante a semana.</p>-->
<!--          </article>-->
<!--          <article class="rounded-3xl border border-[color:var(&#45;&#45;line)] bg-white p-6 shadow-[var(&#45;&#45;shadow-soft)]">-->
<!--            <div class="flex items-center gap-4">-->
<!--              <div class="flex h-12 w-12 items-center justify-center rounded-full bg-[color:var(&#45;&#45;surface-2)] text-sm font-bold text-[color:var(&#45;&#45;leaf)]">VH</div>-->
<!--              <div>-->
<!--                <h3 class="text-lg font-bold text-[color:var(&#45;&#45;ink)]">Vitor Hugo</h3>-->
<!--                <p class="text-sm text-[color:var(&#45;&#45;leaf-soft)]">Pai e entusiasta da culinária</p>-->
<!--              </div>-->
<!--            </div>-->
<!--            <p class="mt-5 text-lg leading-relaxed text-[color:var(&#45;&#45;ink-soft)]">Passei a cozinhar melhor para minha família sem perder tempo. O e-book equilibra sabor, praticidade e organização.</p>-->
<!--          </article>-->
<!--        </div>-->
<!--      </div>-->
<!--    </section>-->

    <section class="mx-auto max-w-6xl px-4 pb-12 md:pb-16">
      <div class="grid gap-6 lg:grid-cols-[1.1fr_0.9fr]">
        <div class="section-shell p-7 md:p-10">
          <span class="kicker">Oferta especial</span>
          <h2 class="mt-5 text-3xl text-[color:var(--ink)] md:text-5xl">Baixe hoje e receba o plano semanal como bônus</h2>
          <p class="mt-5 text-lg text-[color:var(--ink-soft)]">
            Além do e-book completo, você recebe um plano de refeições semanal para facilitar compras, preparos e manter alimentação equilibrada sem improviso.
          </p>
          <div class="mt-7 flex flex-wrap items-center gap-4">
            <a href="https://pay.kiwify.com.br/PEeRXnz" target="_blank" rel="noopener noreferrer" class="cta-button">
              Quero meu acesso agora
              <ArrowRight class="h-5 w-5" />
            </a>
            <p class="text-sm font-semibold text-[color:var(--leaf)]">Entrega imediata no e-mail após a compra</p>
          </div>
        </div>

        <div class="rounded-[30px] border border-[color:var(--line)] bg-[color:var(--ink)] p-7 text-white shadow-[var(--shadow-strong)] md:p-9">
          <p class="text-xs uppercase tracking-[0.2em] text-[#d8e7dd]">Conteúdo incluso</p>
          <ul class="mt-5 space-y-3 text-sm text-[#edf4ef] md:text-base">
            <li class="rounded-xl border border-white/20 px-3 py-2">+30 receitas para todas as refeições</li>
            <li class="rounded-xl border border-white/20 px-3 py-2">Modo de preparo simples e direto</li>
            <li class="rounded-xl border border-white/20 px-3 py-2">Plano semanal para organizar a rotina</li>
            <li class="rounded-xl border border-white/20 px-3 py-2">Garantia de 7 dias sem risco</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="mx-auto max-w-6xl px-4 pb-16">
      <div class="section-shell p-7 md:p-10">
        <div class="grid items-center gap-8 md:grid-cols-[0.7fr_1.3fr]">
          <div class="mx-auto w-full max-w-[240px]">
            <img src="/assets/img/selo7dias.png" width="250" alt="Selo de garantia de 7 dias" class="mx-auto" />
          </div>
          <div>
            <span class="kicker">Compra sem risco</span>
            <h2 class="mt-5 text-3xl text-[color:var(--ink)] md:text-5xl">Garantia incondicional de 7 dias</h2>
            <p class="mt-5 text-lg text-[color:var(--ink-soft)]">
              Se o material não atender sua expectativa, basta solicitar reembolso dentro de 7 dias. Você recebe 100% do valor de volta, sem burocracia.
            </p>
            <p class="mt-4 text-base font-medium text-[color:var(--leaf)]">
              Você testa com tranquilidade e decide com segurança.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="mx-auto max-w-6xl px-4 pb-16">
      <div class="section-shell p-7 md:p-10">
        <span class="kicker">Dúvidas comuns</span>
        <h2 class="mt-5 text-3xl text-[color:var(--ink)] md:text-5xl">Perguntas frequentes</h2>
        <p class="mt-4 max-w-3xl text-lg text-[color:var(--ink-soft)]">
          Reunimos as respostas mais importantes para você comprar com total segurança e saber exatamente o que vai receber.
        </p>
        <div class="mt-8">
          <FaqAccordion />
        </div>
      </div>
    </section>

    <section class="mx-auto max-w-6xl px-4 pb-20">
      <div class="section-shell p-7 text-center md:p-12">
        <span class="kicker">Pronto para começar</span>
        <h2 class="mx-auto mt-5 max-w-3xl text-3xl text-[color:var(--ink)] md:text-5xl">
          Receba hoje seu e-book e comece uma rotina mais leve e gostosa
        </h2>
        <p class="mx-auto mt-5 max-w-2xl text-lg text-[color:var(--ink-soft)]">
          Clique no botão abaixo para liberar acesso imediato e levar também o plano semanal de refeições.
        </p>
        <div class="mt-8">
          <a href="https://pay.kiwify.com.br/PEeRXnz" target="_blank" rel="noopener noreferrer" class="cta-button w-full max-w-sm text-base sm:w-auto md:text-lg">
            Baixar meu e-book agora
            <ArrowRight class="h-5 w-5" />
          </a>
        </div>
      </div>
    </section>
  </div>

  <footer class="footer-shell py-10 text-white">
    <div class="mx-auto max-w-6xl px-4 text-center">
      <p class="text-sm text-white/80">&copy; {{ new Date().getFullYear() }} Melli Criações. Todos os direitos reservados.</p>
    </div>
  </footer>
</template>
