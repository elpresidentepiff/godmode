# GodMode — Discovered Tools Catalogue

New tools and skills found during GodMode bootstrap. Each entry includes a description and install command.

---

## 1. God's Eye View
**Type:** MCP server + 3D globe  
**Stars:** #1 GitHub Trending  
**What it does:** Real-time 3D globe with live aircraft, ships, satellites, weather and public cameras. Exposes an MCP tool surface so agents can query the globe.  
**Install:**
```bash
git clone https://github.com/bilawalsidhu/gods-eye-view
cd gods-eye-view && npm install && npm run dev
```
**MCP config:** Add `gods-eye-view` server to your `claude_desktop_config.json`.

---

## 2. Dream Loop
**Type:** Claude Code skill — 3D visual fidelity loop  
**What it does:** Iterative 3D visual generation skill; runs a refinement loop to improve visual fidelity of rendered scenes.  
**Install:**
```bash
npx skills add achimala/dream-loop
```

---

## 3. CKAN MCP Server
**Type:** MCP server — open data portals  
**What it does:** Connect to any CKAN-powered open data portal (government, research, public datasets) and query datasets via MCP tools.  
**Install:**
```bash
npm install -g @aborruso/ckan-mcp-server
```

---

## 4. BitNet (Microsoft)
**Type:** 1-bit LLM inference engine  
**Stars:** 42K  
**What it does:** Run 1-bit quantised language models locally at a fraction of the memory cost. Ideal for edge/offline inference.  
**Install:**
```bash
git clone https://github.com/microsoft/BitNet
cd BitNet && pip install -r requirements.txt
```

---

## 5. Fireworks AI + Nexus CLI
**Type:** Hosted model API + Claude Code integration  
**What it does:** Access Fireworks AI's model roster (including Nanbeige 4.3, Qwen 3.5 3D Coder, DeepSeek, etc.) from Claude Code via the Nexus CLI integration.  
**Install:**
```bash
# Sign up at fireworks.ai, then:
npm install -g fireworks-nexus-cli
nexus auth login
```

---

## 6. SubQ
**Type:** Claude Code community skill — codebase analysis  
**What it does:** Semantic codebase analysis skill; asks sub-questions about a codebase and synthesises a structured answer.  
**Install:**
```bash
npx skills add community/subq
```

---

## 7. Nanbeige 4.3
**Type:** Reasoning and coding model  
**What it does:** Strong reasoning + coding model, available via Fireworks AI. Competitive on code generation and multi-step reasoning tasks.  
**Install:** Available via Fireworks AI — see entry 5. Model ID: `accounts/fireworks/models/nanbeige-4-3`.

---

## 8. Marketing Skills
**Type:** Claude Code skill — AI marketing workflow  
**What it does:** End-to-end AI marketing workflow skill: brief → copy → imagery → schedule.  
**Install:**
```bash
npx skills add anthropic-skills:marketing
```

---

## 9. Qwen 3.5 3D Coder
**Type:** 3D coding AI model  
**What it does:** Specialised model for 3D code generation (Three.js, WebGL, shader code). Available via Fireworks AI.  
**Install:** Available via Fireworks AI — see entry 5. Model ID: `accounts/fireworks/models/qwen-3-5-3d-coder`.

---

## 10. MiniMax H3 Image
**Type:** Image generation AI  
**What it does:** High-quality image generation model from MiniMax. Competitive with leading image generators; API available.  
**Install:**
```bash
# API access via minimax.io
# Or via ElevenLabs creative connector (creative_generate_image)
```

---

*Last updated: 2026-11-23*
