# uptslide1redirect

A lightweight redirect proxy configured to seamlessly route Vercel-hosted domain requests to a custom domain.

## 🎯 Purpose
This repository exists solely to handle safe routing for the `Unit Penyaringan` presentation slides. It ensures that visitors trying to access the presentation via the default Vercel URLs (e.g., `uptslide1.vercel.app`) are automatically redirected to the canonical URL at **[syariefazman.com/uptslide1](https://syariefazman.com/uptslide1)** while avoiding server-side infinite proxy loops.

## ⚙️ How It Works
It utilizes Vercel's `redirects` config in `vercel.json` to catch all incoming traffic `/(.*)` and redirect it to the custom domain, preserving the URL path for sub-resources if necessary.
