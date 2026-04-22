<template>
  <div class="min-h-screen bg-[#fdfcfb] pb-24 px-6 pt-8 max-w-2xl mx-auto">
    <section :style="{ marginBottom: '2.5rem' }">
      <h2
        class="font-serif font-bold text-gray-900"
        :style="{ fontSize: '1.25rem', marginBottom: '1rem' }"
      >
        Badges
      </h2>
      <div
        class="flex overflow-x-auto pb-2 scrollbar-hide"
        :style="{ gap: '0.75rem' }"
      >
        <BadgeCard
          icon="👨‍🍳"
          title="Palais Curieux"
          subtitle="Premier avis publié"
          active
        />
        <BadgeCard
          icon="👨‍🍳"
          title="Palais Confirmé"
          subtitle="10 avis publiés"
          active
        />
        <BadgeCard
          icon="🥈"
          title="Palais d'Argent"
          subtitle="50 avis utiles"
        />
        <BadgeCard icon="🥇" title="Palais d'Or" subtitle="100 avis utiles" />
      </div>
    </section>

    <section :style="{ marginBottom: '2.5rem' }">
      <div
        class="flex justify-between items-center"
        :style="{ marginBottom: '1rem' }"
      >
        <h2
          class="font-serif font-bold text-gray-900"
          :style="{ fontSize: '1.25rem' }"
        >
          Mes goûts
        </h2>
        <button
          class="text-[#c41e3a] font-bold"
          :style="{ fontSize: '0.875rem' }"
        >
          Modifier
        </button>
      </div>
      <div class="flex flex-wrap" :style="{ gap: '0.5rem' }">
        <TasteTag label="Japonaise" selected />
        <TasteTag label="Italienne" selected />
        <TasteTag label="Française" />
        <TasteTag label="Bistronomique" selected />
        <TasteTag label="Végétarienne" />
      </div>
    </section>

    <section
      class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden"
    >
      <MenuItem label="Mes adresses sauvegardées" />
      <MenuItem label="Mes listes" />
      <MenuItem label="Mon historique" />
      <MenuItem label="Notifications" />
    </section>

    <button
      class="w-full flex justify-center items-center text-[#c41e3a] font-bold transition-opacity hover:opacity-80"
      :style="{ marginTop: '3rem', gap: '0.5rem' }"
    >
      <svg
        class="rotate-180"
        width="18"
        height="18"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="2.5"
      >
        <path
          d="M15 3h4a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2h-4M10 17l5-5-5-5M13.8 12H3"
        />
      </svg>
      <span :style="{ fontSize: '1rem' }">Se déconnecter</span>
    </button>
  </div>
</template>

<script setup></script>
