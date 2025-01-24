<!-- pages/programs.md -->
---
layout: page
title: Our Programs
permalink: /programs/
---

<div class="container mx-auto px-4 py-8">
    <h1 class="text-4xl font-bold mb-8 text-center">Our Programs</h1>
    
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        {% for program in site.data.programs %}
        <div class="bg-white rounded-lg shadow-lg overflow-hidden">
            <div class="p-6">
                <h2 class="text-2xl font-bold mb-4">{{ program.name }}</h2>
                <p class="text-gray-600 mb-4">{{ program.description }}</p>
                
                <h3 class="font-bold mb-2">Features:</h3>
                <ul class="list-disc list-inside mb-4">
                    {% for feature in program.features %}
                    <li>{{ feature }}</li>
                    {% endfor %}
                </ul>
                
                <p class="font-semibold">Schedule: {{ program.schedule }}</p>
            </div>
        </div>
        {% endfor %}
    </div>

    <div class="mt-12 text-center">
        <h2 class="text-2xl font-bold mb-4">Schedule a Tour</h2>
        <p class="mb-4">Visit our facility and learn more about our programs</p>
        <a href="/book" class="bg-blue-600 text-white px-8 py-3 rounded-lg hover:bg-blue-700">Book Now</a>
    </div>
</div>