---
layout: default  # Or 'page/single'; check your _layouts folder
title: Product Portfolio
permalink: /portfolio/
---

{% include nav.html %}  <!-- If you have a nav include; skip otherwise -->

<div class="max-w-6xl mx-auto px-4 py-12 bg-gray-50 min-h-screen">
  <header class="text-center mb-16">
    <h1 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent mb-4">
      Product Portfolio
    </h1>
    <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
      9+ years as Senior PM in healthtech/fintech. Data/AI-driven journeys, fulfilment mastery, sustainability focus.<br>
      Targeting cleantech/energy roles.
    </p>
  </header>

  <section class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
    <!-- Case 1: Your Kry win [cite:3] -->
    <article class="bg-white p-8 rounded-2xl shadow-xl hover:shadow-2xl transition-all duration-300 border border-gray-100 group">
      <div class="flex items-start gap-4 mb-6">
        <i class="fas fa-chart-line text-3xl text-blue-500 group-hover:scale-110 transition"></i>
        <div>
          <h2 class="text-2xl font-bold text-gray-900 mb-1">Kry Partnership Launch</h2>
          <p class="text-blue-600 font-semibold text-lg">+15% activation</p>
        </div>
      </div>
      <p class="text-gray-700 mb-6 leading-relaxed">Led 0→1 wellness app integration. Reduced drop-offs 68% via clinician-aligned onboarding experiments.</p>
      <ul class="flex flex-wrap gap-2 text-sm text-gray-500 mb-4">
        <li class="px-3 py-1 bg-blue-100 rounded-full">#Healthtech</li>
        <li class="px-3 py-1 bg-blue-100 rounded-full">#Retention</li>
        <li class="px-3 py-1 bg-blue-100 rounded-full">#Partnerships</li>
      </ul>
      <a href="#kry-details" class="text-blue-600 hover:underline font-medium">Details →</a>
    </article>

    <!-- Case 2: AI example [cite:11] -->
    <article class="bg-white p-8 rounded-2xl shadow-xl hover:shadow-2xl transition-all duration-300 border border-gray-100 group">
      <div class="flex items-start gap-4 mb-6">
        <i class="fas fa-robot text-3xl text-green-500 group-hover:scale-110 transition"></i>
        <div>
          <h2 class="text-2xl font-bold text-gray-900 mb-1">AI Insights Engine</h2>
          <p class="text-green-600 font-semibold text-lg">68% triage speed</p>
        </div>
      </div>
      <p class="text-gray-700 mb-6 leading-relaxed">Built evals for hallucination mitigation; turned ticket data into prioritized backlog via experiments.</p>
      <ul class="flex flex-wrap gap-2 text-sm text-gray-500 mb-4">
        <li class="px-3 py-1 bg-green-100 rounded-full">#AI/ML</li>
        <li class="px-3 py-1 bg-green-100 rounded-full">#Metrics</li>
        <li class="px-3 py-1 bg-green-100 rounded-full">#Experiments</li>
      </ul>
      <a href="#ai-details" class="text-green-600 hover:underline font-medium">Details →</a>
    </article>

    <!-- Case 3: Fulfilment for energy role [web:15] -->
    <article class="bg-white p-8 rounded-2xl shadow-xl hover:shadow-2xl transition-all duration-300 border border-gray-100 group">
      <div class="flex items-start gap-4 mb-6">
        <i class="fas fa-truck text-3xl text-purple-500 group-hover:scale-110 transition"></i>
        <div>
          <h2 class="text-2xl font-bold text-gray-900 mb-1">Fulfilment Optimisation</h2>
          <p class="text-purple-600 font-semibold text-lg">-20% cycle time</p>
        </div>
      </div>
      <p class="text-gray-700 mb-6 leading-relaxed">Portals + metrics dashboard cut order-to-delivery; scalable for clean-tech hardware.</p>
      <ul class="flex flex-wrap gap-2 text-sm text-gray-500 mb-4">
        <li class="px-3 py-1 bg-purple-100 rounded-full">#Fulfilment</li>
        <li class="px-3 py-1 bg-purple-100 rounded-full">#Portals</li>
        <li class="px-3 py-1 bg-purple-100 rounded-full">#Sustainability</li>
      </ul>
      <a href="#fulfil-details" class="text-purple-600 hover:underline font-medium">Details →</a>
    </article>
  </section>

  <div id="kry-details" class="mt-16 p-8 bg-white rounded-2xl shadow-lg hidden">
    <!-- Expand with full STAR story + metrics/charts -->
    <h3>Kry Details</h3>
    <p>Full case study here...</p>
  </div>

  <!-- Add Tailwind CDN to your site's _includes/head.html or layout -->
</div>

<script src="https://cdn.tailwindcss.com"></script>
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
