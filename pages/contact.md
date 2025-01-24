<!-- pages/contact.md -->
---
layout: page
title: Contact Us
permalink: /contact/
---

<div class="container mx-auto px-4 py-8">
    <h1 class="text-4xl font-bold mb-8 text-center">Contact Us</h1>
    
    <div class="max-w-4xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8">
        <div>
            <h2 class="text-2xl font-bold mb-4">Get in Touch</h2>
            <form class="space-y-4" netlify>
                <div>
                    <label class="block text-sm font-medium mb-1">Name</label>
                    <input type="text" name="name" required class="w-full p-2 border rounded">
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Email</label>
                    <input type="email" name="email" required class="w-full p-2 border rounded">
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Phone</label>
                    <input type="tel" name="phone" class="w-full p-2 border rounded">
                </div>
                <div>
                    <label class="block text-sm font-medium mb-1">Message</label>
                    <textarea name="message" rows="4" required class="w-full p-2 border rounded"></textarea>
                </div>
                <button type="submit" class="bg-blue-600 text-white px-6 py-2 rounded hover:bg-blue-700">
                    Send Message
                </button>
            </form>
        </div>
        
        <div>
            <h2 class="text-2xl font-bold mb-4">Location & Hours</h2>
            <div class="space-y-4">
                <div>
                    <h3 class="font-bold">Address</h3>
                    <p>{{ site.business.address }}</p>
                </div>
                <div>
                    <h3 class="font-bold">Phone</h3>
                    <p>{{ site.business.phone }}</p>
                </div>
                <div>
                    <h3 class="font-bold">Email</h3>
                    <p>{{ site.business.email }}</p>
                </div>
                <div>
                    <h3 class="font-bold">Hours</h3>
                    <p>{{ site.business.hours }}</p>
                </div>
            </div>
        </div>
    </div>
</div>
