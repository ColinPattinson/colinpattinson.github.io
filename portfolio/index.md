---
layout: default  # Match your site's layouts
title: Product Portfolio
permalink: /portfolio/
---

<script src="https://cdn.tailwindcss.com"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<div class="bg-gray-50 min-h-screen py-12 px-4 md:px-8">
  <div class="max-w-6xl mx-auto">
    <!-- Hero -->
    <div class="text-center mb-20">
      <h1 class="text-5xl md:text-7xl font-black bg-gradient-to-r from-slate-900 via-blue-800 to-slate-500 bg-clip-text text-transparent mb-6 drop-shadow-2xl">
        Product Portfolio
      </h1>
      <p class="text-xl md:text-2xl text-gray-700 max-w-3xl mx-auto leading-relaxed">
        Senior PM | 9+ years healthtech/fintech | AI/data-driven journeys | Cleantech ready
      </p>
    </div>

    <!-- Projects Grid -->
    <div class="grid md:grid-cols-2 xl:grid-cols-3 gap-8 mb-20">
      
      {% include project-card.html 
        icon="fa-chart-line" 
        color="blue" 
        title="Kry Vitality Partnership" 
        metric="+25% activation [cite:3]" 
        desc="0→1 launch: Scoped MVP, aligned stakeholders, proved impact on retention." 
        tags="Healthtech, Partnerships, Metrics" %}

      {% include project-card.html 
        icon="fa-robot" 
        color="emerald" 
        title="AI Evals Framework" 
        metric="68% faster triage [cite:11]" 
        desc="Built hallucination mitigations; qual data → experiments → backlog." 
        tags="AI, Experiments, Leadership" %}

      {% include project-card.html 
        icon="fa-truck-ramp-box" 
        color="purple" 
        title="Fulfilment Portals" 
        metric="-20% cycle time [web:15]" 
        desc="Customer + ops portals; on-time delivery KPIs for scalable solutions." 
        tags="Fulfilment, Portals, Sustainability" %}

    </div>

    <!-- CTA -->
    <div class="text-center bg-white p-12 rounded-3xl shadow-2xl border border-gray-100">
      <h2 class="text-3xl font-bold text-gray-900 mb-4">Open to Opportunities</h2>
      <p class="text-lg text-gray-600 mb-8 max-w-2xl mx-auto">Senior PM roles in energy/cleantech. Let's chat.</p>
      <a href="mailto:your@email.com?subject=PM Role Chat" class="bg-blue-600 text-white px-10 py-4 rounded-2xl text-xl font-semibold hover:bg-blue-700 transition inline-block">
        <i class="fas fa-envelope mr-2"></i> Get in Touch
      </a>
    </div>
  </div>
</div>

<!-- Inline Project Card Include (add as _includes/project-card.html later) -->
<script>
  tailwind.config = { theme: { extend: { colors: { } } } }
</script>
