
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>GoldenKey Realty — Find Your Next Home</title>

  <!-- Tailwind CDN for fast, modern styling (no build step) -->
  <script src="https://cdn.tailwindcss.com"></script>

  <style>
    /* Small custom touches */
    .brand { color: #0f172a; } /* slate-900 */
    .accent { color: #c084fc; } /* purple-300 */
    .chat-bubble {
      background: linear-gradient(135deg,#ffffff 0%, #f3e8ff 100%);
      border: 1px solid rgba(120,86,240,0.12);
      box-shadow: 0 6px 20px rgba(12,11,18,0.06);
    }
    /* Floating chat button */
    #chat-toggle { bottom: 28px; right: 28px; }
    /* Chat window */
    #chat { width: 360px; max-width: calc(100% - 40px); }
    .prop-img { height: 180px; object-fit: cover; }
  </style>
</head>
<body class="bg-gray-50 text-slate-700 antialiased">

  <!-- Header -->
  <header class="bg-white border-b">
    <div class="max-w-6xl mx-auto px-6 py-5 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="w-12 h-12 rounded-md bg-gradient-to-br from-purple-400 to-indigo-600 flex items-center justify-center text-white font-bold">GK</div>
        <div>
          <h1 class="text-xl font-semibold brand">GoldenKey Realty</h1>
          <p class="text-sm text-gray-500">Local market experts — Luxury & family homes</p>
        </div>
      </div>
      <nav class="space-x-6 text-sm">
        <a href="#listings" class="hover:text-slate-900">Listings</a>
        <a href="#services" class="hover:text-slate-900">Services</a>
        <a href="#contact" class="hover:text-slate-900">Contact</a>
        <a href="#book" class="ml-4 inline-block px-4 py-2 bg-indigo-600 text-white rounded-md text-sm">Book a Tour</a>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section class="py-12">
    <div class="max-w-6xl mx-auto px-6 grid md:grid-cols-2 gap-8 items-center">
      <div>
        <h2 class="text-4xl font-extrabold brand">Find your next home — faster with AI assistance</h2>
        <p class="mt-4 text-gray-600">Instant answers, seamless booking, and a personal assistant that pre-qualifies buyers so you only meet qualified prospects.</p>
        <div class="mt-6 flex gap-3">
          <a href="#listings" class="px-5 py-3 bg-indigo-600 text-white rounded-md shadow">Browse Listings</a>
          <a href="#services" class="px-5 py-3 border border-indigo-600 text-indigo-600 rounded-md">Our Services</a>
        </div>

        <div class="mt-8 grid grid-cols-2 gap-4">
          <div class="p-4 bg-white rounded-md shadow-sm">
            <h4 class="text-sm font-semibold">Avg. Days on Market</h4>
            <p class="mt-1 text-2xl font-bold">12</p>
          </div>
          <div class="p-4 bg-white rounded-md shadow-sm">
            <h4 class="text-sm font-semibold">Satisfaction</h4>
            <p class="mt-1 text-2xl font-bold">98%</p>
          </div>
        </div>
      </div>

      <div class="relative">
        <img src="https://images.unsplash.com/photo-1560184897-6a3f6d9e2e1c?q=80&w=1200&auto=format&fit=crop" alt="House" class="rounded-lg shadow-lg">
        <div class="absolute bottom-6 left-6 bg-white/90 p-4 rounded-lg shadow-md">
          <p class="text-sm text-gray-600">Want a quick tour?</p>
          <a href="#book" class="mt-2 inline-block px-4 py-2 bg-purple-500 text-white rounded">Schedule a Showing</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Listings -->
  <section id="listings" class="max-w-6xl mx-auto px-6 py-8">
    <h3 class="text-2xl font-bold brand">Featured Listings</h3>
    <p class="text-gray-500 mt-1">Hand-picked homes in your area.</p>

    <div class="mt-6 grid sm:grid-cols-2 lg:grid-cols-3 gap-6">
      <!-- property card (repeat) -->
      <article class="bg-white rounded-lg shadow-sm overflow-hidden">
        <img class="prop-img w-full" src="https://images.unsplash.com/photo-1599423300746-b62533397364?q=80&w=1200&auto=format&fit=crop" alt="Property 1">
        <div class="p-4">
          <div class="flex items-start justify-between">
            <div>
              <h4 class="font-semibold">Modern Family Home</h4>
              <p class="text-sm text-gray-500">3 bed • 2 bath • 2,200 sqft</p>
            </div>
            <div class="text-right">
              <p class="text-lg font-bold">$679,000</p>
              <p class="text-sm text-gray-400">Fairview</p>
            </div>
          </div>

          <div class="mt-4 flex gap-3">
            <button class="book-btn flex-1 px-3 py-2 bg-indigo-600 text-white rounded" data-title="Modern Family Home">Request Tour</button>
            <button class="details-btn px-3 py-2 border rounded text-sm" data-desc="Open-plan kitchen, large yard">Details</button>
          </div>
        </div>
      </article>

      <article class="bg-white rounded-lg shadow-sm overflow-hidden">
        <img class="prop-img w-full" src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?q=80&w=1200&auto=format&fit=crop" alt="Property 2">
        <div class="p-4">
          <div class="flex items-start justify-between">
            <div>
              <h4 class="font-semibold">Downtown Loft</h4>
              <p class="text-sm text-gray-500">2 bed • 1 bath • 1,100 sqft</p>
            </div>
            <div class="text-right">
              <p class="text-lg font-bold">$459,000</p>
              <p class="text-sm text-gray-400">Central</p>
            </div>
          </div>

          <div class="mt-4 flex gap-3">
            <button class="book-btn flex-1 px-3 py-2 bg-indigo-600 text-white rounded" data-title="Downtown Loft">Request Tour</button>
            <button class="details-btn px-3 py-2 border rounded text-sm" data-desc="City views, rooftop access">Details</button>
          </div>
        </div>
      </article>

      <article class="bg-white rounded-lg shadow-sm overflow-hidden">
        <img class="prop-img w-full" src="https://images.unsplash.com/photo-1572120360610-d971b9b6b7d4?q=80&w=1200&auto=format&fit=crop" alt="Property 3">
        <div class="p-4">
          <div class="flex items-start justify-between">
            <div>
              <h4 class="font-semibold">Cozy Cottage</h4>
              <p class="text-sm text-gray-500">2 bed • 1 bath • 900 sqft</p>
            </div>
            <div class="text-right">
              <p class="text-lg font-bold">$329,000</p>
              <p class="text-sm text-gray-400">Riverside</p>
            </div>
          </div>

          <div class="mt-4 flex gap-3">
            <button class="book-btn flex-1 px-3 py-2 bg-indigo-600 text-white rounded" data-title="Cozy Cottage">Request Tour</button>
            <button class="details-btn px-3 py-2 border rounded text-sm" data-desc="Updated interior, private garden">Details</button>
          </div>
        </div>
      </article>

    </div>
  </section>

  <!-- Services -->
  <section id="services" class="bg-white border-t">
    <div class="max-w-6xl mx-auto px-6 py-8">
      <h3 class="text-2xl font-bold brand">Services</h3>
      <div class="mt-6 grid md:grid-cols-3 gap-6">
        <div class="p-6 rounded-lg shadow-sm">
          <h4 class="font-semibold">Buyer Representation</h4>
          <p class="mt-2 text-sm text-gray-500">Full support from search to close, with AI-assisted lead prioritization.</p>
        </div>
        <div class="p-6 rounded-lg shadow-sm">
          <h4 class="font-semibold">Seller Marketing</h4>
          <p class="mt-2 text-sm text-gray-500">Professional photography, listing optimization, and AI-driven pricing suggestions.</p>
        </div>
        <div class="p-6 rounded-lg shadow-sm">
          <h4 class="font-semibold">Investment Consultation</h4>
          <p class="mt-2 text-sm text-gray-500">We identify high-ROI neighborhoods and run cashflow analyses.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Booking / Contact -->
  <section id="book" class="max-w-6xl mx-auto px-6 py-10">
    <div class="grid lg:grid-cols-2 gap-8 items-start">
      <div>
        <h3 class="text-2xl font-bold brand">Request a Showing</h3>
        <p class="text-gray-600 mt-1">Tell us which property and preferred time — our assistant will confirm availability.</p>

        <form id="booking-form" class="mt-6 space-y-4 bg-white p-6 rounded-lg shadow-sm">
          <div>
            <label class="text-sm text-gray-600">Property</label>
            <input required id="prop" name="property" class="w-full mt-1 border rounded p-2" placeholder="e.g., Modern Family Home">
          </div>

          <div class="grid grid-cols-2 gap-4">
            <div>
              <label class="text-sm text-gray-600">Date</label>
              <input required id="date" name="date" type="date" class="w-full mt-1 border rounded p-2">
            </div>
            <div>
              <label class="text-sm text-gray-600">Time</label>
              <input required id="time" name="time" type="time" class="w-full mt-1 border rounded p-2">
            </div>
          </div>

          <div>
            <label class="text-sm text-gray-600">Your Name</label>
            <input required id="name" name="name" class="w-full mt-1 border rounded p-2" placeholder="Full name">
          </div>
          <div>
            <label class="text-sm text-gray-600">Phone or Email</label>
            <input required id="contact" name="contact" class="w-full mt-1 border rounded p-2" placeholder="Phone or email">
          </div>

          <div class="flex gap-3">
            <button type="submit" class="px-4 py-2 bg-indigo-600 text-white rounded">Request Showing</button>
            <button type="button" id="open-chat" class="px-4 py-2 border rounded">Ask our Assistant</button>
          </div>

          <p id="booking-feedback" class="text-sm text-green-600 mt-2 hidden">Thanks — your request was recorded. Our assistant will follow up shortly.</p>
        </form>
      </div>

      <div>
        <h4 class="text-lg font-semibold brand">Contact</h4>
        <p class="text-gray-600 mt-1">GoldenKey Realty — downtown office</p>
        <p class="mt-4 text-sm">Phone: <strong>(555) 123-4567</strong></p>
        <p class="text-sm">Email: <strong>hello@goldenkey.example</strong></p>

        <div class="mt-6 bg-gradient-to-r from-purple-50 to-indigo-50 p-4 rounded-lg">
          <h5 class="font-semibold">Quick Mortgage Estimate</h5>
          <p class="text-sm text-gray-600 mt-1">Type your budget & down payment; the assistant will estimate monthly payment.</p>
          <div class="mt-3 flex gap-2">
            <input id="budget" placeholder="Price ($)" class="p-2 border rounded w-1/2">
            <input id="down" placeholder="Down ($)" class="p-2 border rounded w-1/2">
          </div>
          <button id="mortgage-btn" class="mt-3 px-4 py-2 bg-purple-600 text-white rounded">Estimate Payment</button>
          <p id="mortgage-result" class="mt-3 text-sm text-gray-700"></p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white border-t mt-10">
    <div class="max-w-6xl mx-auto px-6 py-6 flex items-center justify-between">
      <p class="text-sm text-gray-500">© <span id="year"></span> GoldenKey Realty. All rights reserved.</p>
      <div class="text-sm text-gray-500">Built for demo purposes • <span class="accent">AutoScale AI</span> style</div>
    </div>
  </footer>

  <!-- Floating Chat Button -->
  <button id="chat-toggle" class="fixed z-40 p-4 rounded-full shadow-lg bg-indigo-600 text-white" title="Open chat">
    💬
  </button>

  <!-- Chat Window (hidden until opened) -->
  <div id="chat-window" class="fixed z-50 bottom-20 right-6 hidden">
    <div id="chat" class="chat-bubble rounded-lg p-3">
      <div class="flex items-center justify-between">
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-md bg-gradient-to-br from-purple-400 to-indigo-600 flex items-center justify-center text-white font-bold">AI</div>
          <div>
            <div class="font-semibold">GoldenKey Assistant</div>
            <div class="text-xs text-gray-500">Here to help — ask anything</div>
          </div>
        </div>
        <button id="chat-close" class="text-gray-400 hover:text-gray-700">✕</button>
      </div>

      <div id="messages" class="mt-3 max-h-64 overflow-auto space-y-3 px-1">
        <!-- messages appear here -->
      </div>

      <form id="chat-form" class="mt-3 grid grid-cols-12 gap-2 items-center">
        <input id="chat-input" placeholder="Ask about listings, pricing, or book a tour..." class="col-span-9 p-2 border rounded" />
        <button id="send-btn" class="col-span-3 px-3 py-2 bg-indigo-600 text-white rounded">Send</button>
      </form>

      <div id="chat-hint" class="text-xs text-gray-400 mt-2">Try: "Show me 3-bed homes under $700k" or "Estimate payment for $550k with $50k down".</div>
    </div>
  </div>

  <script>
    // Small utilities
    function el(q) { return document.querySelector(q); }
    function addMessage(text, who = 'bot') {
      const container = document.createElement('div');
      container.className = who === 'bot' ? 'p-3 rounded-lg bg-white/90 shadow-sm' : 'p-3 rounded-lg bg-indigo-600 text-white self-end';
      container.innerHTML = text;
      const wrap = document.createElement('div');
      wrap.className = 'flex ' + (who === 'bot' ? '' : 'justify-end');
      wrap.appendChild(container);
      el('#messages').appendChild(wrap);
      el('#messages').scrollTop = el('#messages').scrollHeight;
    }

    // Basic demo bot (rule-based). Replace hook below with real AI if desired.
    function botReply(userText) {
      const text = userText.toLowerCase().trim();

      // quick intents
      if (/hi|hello|hey|good (morning|afternoon|evening)/i.test(text)) {
        return "Hi — I'm GoldenKey Assistant. I can help with listings, bookings, and quick mortgage estimates. Try: \"Show me 3-bed homes under $700k\" or \"Book a showing for Modern Family Home on May 10\".";
      }

      // property search intent
      const searchMatch = text.match(/(show|find|list).*(\d+)\s*-?\s*bed.*(under|below|less than)\s*\$?([\d,]+)/i) ||
                          text.match(/(show|find|list).*(under|below|less than)\s*\$?([\d,]+).*(\d+)\s*-?\s*bed/i);

      if (searchMatch) {
        // naive parse, show demo results regardless
        return "Here are 3 matching properties I found: 1) Modern Family Home — $679,000 — 3 bed. 2) Downtown Loft — $459,000 — 2 bed. 3) Cozy Cottage — $329,000 — 2 bed. Want me to schedule showings for any of these?";
      }

      // booking intent
      const bookMatch = text.match(/book|schedule|showing|tour/i) && text.match(/(on|for)\s+([a-z0-9 ,\/.-]+)/i);
      if (bookMatch) {
        // collect basic info and simulate scheduling
        return "Got it — tell me the property name, preferred date, and your contact info (phone or email) and I'll request the showing and confirm availability.";
      }

      // mortgage estimate intent: user types "$550k" or "estimate payment for 550000"
      const priceMatch = text.match(/\$?([\d,]{3,})/);
      const downMatch = text.match(/down\s*\$?([\d,]+)/i) || text.match(/with\s*\$?([\d,]+)\s*down/i);
      if (priceMatch) {
        const price = Number(priceMatch[1].replace(/,/g,'')) || 0;
        const down = downMatch ? Number(downMatch[1].replace(/,/g,'')) : Math.round(price * 0.1);
        // simple mortgage calc: 30yr fixed @ 6.5% (demo)
        const loan = price - down;
        const r = 0.065/12;
        const n = 30*12;
        const payment = (loan * r) / (1 - Math.pow(1 + r, -n));
        return `Estimated monthly payment on $${price.toLocaleString()} with $${down.toLocaleString()} down: ~$${Math.round(payment).toLocaleString()} / month (30yr fixed @ 6.5% - demo estimate).`;
      }

      // fallback
      return "Sorry — I didn't catch that. I can: 1) show listings, 2) estimate mortgage payments, 3) schedule a showing. Try: 'Estimate payment for $450k with $45k down' or 'Book a showing for Downtown Loft on June 5'.";
    }

    // Chat UI behaviour
    document.addEventListener('DOMContentLoaded', () => {
      el('#year').textContent = new Date().getFullYear();

      // open/close chat
      el('#chat-toggle').addEventListener('click', () => {
        el('#chat-window').classList.toggle('hidden');
        el('#chat-toggle').style.display = 'none';
      });
      el('#chat-close').addEventListener('click', () => {
        el('#chat-window').classList.add('hidden');
        el('#chat-toggle').style.display = 'block';
      });
      el('#open-chat').addEventListener('click', () => {
        el('#chat-window').classList.remove('hidden');
        el('#chat-toggle').style.display = 'none';
      });

      // message send
      el('#chat-form').addEventListener('submit', async (e) => {
        e.preventDefault();
        const input = el('#chat-input');
        const text = input.value.trim();
        if (!text) return;
        addMessage(text, 'user');
        input.value = '';

        // show typing placeholder
        addMessage('Typing...', 'bot');
        // simulate network delay
        await new Promise(r => setTimeout(r, 600));
        // remove the 'Typing...' (last bot message)
        const messages = el('#messages');
        if (messages.lastChild) messages.removeChild(messages.lastChild);

        // get reply from rule-based bot
        const reply = botReply(text);
        addMessage(reply, 'bot');
      });

      // property "Request Tour" quick buttons
      document.querySelectorAll('.book-btn').forEach(btn => {
        btn.addEventListener('click', () => {
          const title = btn.dataset.title || '';
          el('#prop').value = title;
          window.scrollTo({ top: document.querySelector('#book').offsetTop - 30, behavior: 'smooth' });
          el('#booking-form').querySelector('input[name="date"]').focus();
        });
      });

      // details button (demo)
      document.querySelectorAll('.details-btn').forEach(btn => {
        btn.addEventListener('click', () => {
          alert(btn.dataset.desc || 'More details coming soon — demo site.');
        });
      });

      // booking form submit (stores to localStorage as demo)
      el('#booking-form').addEventListener('submit', (e) => {
        e.preventDefault();
        const data = {
          property: el('#prop').value,
          date: el('#date').value,
          time: el('#time').value,
          name: el('#name').value,
          contact: el('#contact').value,
          timestamp: new Date().toISOString()
        };
        // store demo booking
        const bookings = JSON.parse(localStorage.getItem('demoBookings') || '[]');
        bookings.push(data);
        localStorage.setItem('demoBookings', JSON.stringify(bookings));
        el('#booking-feedback').classList.remove('hidden');

        // also show a chat assistant follow-up
        addMessage(`Thanks ${data.name}! I recorded your request for ${data.property} on ${data.date} at ${data.time}. We'll confirm availability within 24 hours.`, 'bot');
        // reset form lightly
        el('#booking-form').reset();
      });

      // mortgage quick estimate UI
      el('#mortgage-btn').addEventListener('click', () => {
        const price = Number((el('#budget').value || '').replace(/,/g,'')) || 0;
        const down = Number((el('#down').value || '').replace(/,/g,'')) || Math.round(price*0.1);
        if (!price) { el('#mortgage-result').textContent = 'Enter a price to estimate.'; return; }
        const loan = price - down;
        const r = 0.065/12; const n = 30*12;
        const payment = (loan * r) / (1 - Math.pow(1 + r, -n));
        el('#mortgage-result').textContent = `Estimated monthly payment: ~$${Math.round(payment).toLocaleString()} / month (30yr fixed @ 6.5% — demo).`;
      });

      // pre-populate a friendly greeting in chat
      setTimeout(() => {
        addMessage("Hi — I'm your GoldenKey Assistant. Ask me about listings, schedule showings, or type a price to get a quick mortgage estimate.", 'bot');
      }, 800);
    });

    /* ================================
       OPTIONAL: Integrate a real AI
       ================================
       The demo above is rule-based. To use an LLM (e.g., OpenAI's ChatGPT) you'd typically:
       1) Create a small server endpoint (Node/Express, Python Flask) that stores your API key securely.
       2) Have the chat frontend call that endpoint with the user message.
       3) The server forwards the message to the OpenAI API and returns the model's reply.

       Example server sketch (Node/Express):
       ------------------------------------------------
       // POST /api/chat
       // body: { message: "User text" }
       const express = require('express');
       const fetch = require('node-fetch');
       app.post('/api/chat', async (req, res) => {
         const user = req.body.message;
         const resp = await fetch('https://api.openai.com/v1/chat/completions', {
           method: 'POST',
           headers: { 'Content-Type': 'application/json', 'Authorization': `Bearer ${process.env.OPENAI_KEY}` },
           body: JSON.stringify({
             model: 'gpt-4o-mini', // choose model
             messages: [{ role: 'system', content: 'You are a helpful real estate assistant...' }, { role: 'user', content: user }],
             max_tokens: 400
           })
         });
         const data = await resp.json();
         return res.json({ reply: data.choices[0].message.content });
       });
       ------------------------------------------------

       Then in the browser replace botReply(text) call with a fetch to /api/chat and display the returned text.

       IMPORTANT:
       - Never expose your OpenAI API key in client-side code.
       - Add rate-limits and basic moderation (filtering) if you plan to run it publicly.
    */
  </script>
</body>
</html>
