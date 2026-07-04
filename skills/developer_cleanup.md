# Developer Cleanup Guidelines

When asked to free up space for developers, prioritize these common caches and artifacts:

* **Python Cleanup**
  * `.venv` and `venv` environments (ask first if active)
  * pip cache 
  * conda cache (`conda clean --all`)
  * `__pycache__`

* **Node.js Cleanup**
  * `node_modules` (in older or archived projects)
  * pnpm store
  * npm cache (`npm cache clean --force`)
  * yarn cache

* **AI Storage**
  * Hugging Face cache (`.cache/huggingface`)
  * Ollama models
  * LM Studio models
  * Stable Diffusion checkpoints

* **Docker Cleanup**
  * Dangling Images (`docker image prune`)
  * Unused Volumes (`docker volume prune`)
  * Build cache (`docker builder prune`)

* **WSL Cleanup**
  * VHDX files (Virtual Hard Disks)
  * Old abandoned distributions
  * Package cache
