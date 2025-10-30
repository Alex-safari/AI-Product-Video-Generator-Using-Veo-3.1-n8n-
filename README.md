# AI-Product-Video-Generator-Using-Veo-3.1-n8n-
Turn a single product photo into a cinematic, high-converting AI product video — fully automated.

**This template was created by Alex Safari.** Subscribe to my YouTube channel for more AI automation tutorials:  
👉 https://www.youtube.com/@alexsafari1  

📺 **Watch the Full Tutorial Video:** https://youtu.be/Hj5svAMH2n8

## Overview
This workflow transforms a **single uploaded product photo** into a **cinematic, studio-quality product video ad** — automatically.

Using **Veo 3.1**, **Gemini 2.5 Pro**, and **n8n**, this system analyzes a product image, writes a professional creative brief, and generates a stunning **AI product video** that looks like a high-end commercial.

It's perfect for e-commerce founders, marketers, and agencies who need high-converting video ads for products on Amazon, Shopify, or any other platform, without the hassle of filming or editing.

## Workflow Breakdown

### 1. On Form Submission
* Collects the user-uploaded product image.
* Captures the desired `aspect_ratio` (e.g., "9:16" or "16:9").
* Takes a simple `Description` from the user (e.g., "Make it look cool").

### 2. Upload Product Image
* Stores the original photo in a specific Google Drive folder (“Product Photos”).

### 3. Analyze Image (Gemini 2.5 Pro)
* Performs an expert visual analysis of the product photo.
* Returns a structured YAML output detailing the product's category, materials, color palette (including HEX codes), and geometry.

### 4. Creative Director (Gemini 2.5 Pro)
* Acts as an AI Creative Director.
* Takes the detailed YAML analysis and the user's simple `Description`.
* Writes a sophisticated, cinematic timeline prompt in the style required for Veo 3.1, defining the scene, camera motion, lighting, and pacing.

### 5. Call 'Kie.ai VEO3 fast image to video subworkflow'
* Sends the product image URL and the new cinematic prompt to the Veo 3.1 model via Kie.ai.
* Generates the final CGI-quality video ad.

### 6. Download Video
* Retrieves the generated video file from the API result URL.

### 7. Upload Final Video
* Saves the final video ad to a different Google Drive folder (“Product Videos”).

### 8. Create Baserow Row
* Logs all metadata for the job in a Baserow database.
* Saves the original image link, the final video link, aspect ratio, and status.

## ⚙️ Tech Stack
* **n8n** – Automation & workflow logic
* **Veo 3.1 (Kie.ai)** – Image-to-video generation engine
* **Gemini 2.5 Pro (Google)** – Image analysis & creative direction
* **OpenRouter** – AI model routing
* **Baserow & Google Drive** – Database & file management

---

📧 **Email me directly**: contact@loopsera.com  
   For quick questions, customisation requests, or workflow troubleshooting.  

🌐 **Visit my website**: [https://loopsera.com](https://loopsera.com)  
   Explore more automation templates, services, and case studies.  

📞 **Book a Discovery Call**: [https://cal.com/loopsera/discoverycall](https://cal.com/loopsera/discoverycall)  
   For businesses that need a custom AI systems built.  

🎓 **1-on-1 Coaching Session**: [https://cal.com/loopsera/n8n-ai-agent-coaching-session](https://cal.com/loopsera/n8n-ai-agent-coaching-session)  
   Personalised coaching to help you build, troubleshoot, or optimise n8n AI workflows. Perfect for both beginners and advanced users.  

💬 **Join the AI Builder’s Boardroom (Skool Community)**: [https://www.skool.com/ai-builders-boardroom-1717](https://www.skool.com/ai-builders-boardroom-1717) — a professional community for builders creating AI agents that talk, listen, and sell, focused on deploying the digital workforce of the future.
