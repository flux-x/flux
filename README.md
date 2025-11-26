<p align="center">
  <picture>
      <source media="(prefers-color-scheme: dark)" srcset="docs/flux-banner-dark.png">
      <source media="(prefers-color-scheme: light)" srcset="docs/flux-banner-light.png">
      <img height="120" alt="Flux" src="docs/flux-banner-light.png">
  </picture>
</p>

<p align="center">
    <b>Distributed Job Runner for Modern AI & Data Workloads</b>
</p>

<p align="center">
    <a href="https://github.com/NoemiAI/flux/actions/workflows/rust.yml">
      <img src="https://img.shields.io/github/actions/workflow/status/NoemiAI/flux/rust.yml?style=flat-square" alt="Rust CI">
    </a>
    <a href="https://img.shields.io/badge/docs-coming_soon-blue?style=flat-square">
      <img src="https://img.shields.io/badge/Docs-Coming_Soon-blue?style=flat-square" alt="Docs">
    </a>
    <a href="https://github.com/NoemiAI/flux/blob/main/LICENSE">
      <img src="https://img.shields.io/github/license/NoemiAI/flux?style=flat-square" alt="License">
    </a>
    <a href="https://discord.gg/your-link">
      <img src="https://img.shields.io/badge/Discord-Join-blue?logo=Discord&style=flat-square" alt="Discord">
    </a>
    <a href="ROADMAP.md">
      <img src="https://img.shields.io/badge/Roadmap-2025-orange.svg?style=flat-square" alt="Roadmap 2025">
    </a>
</p>

**Flux** is a high-performance, distributed job runner built in Rust 🦀.  

It provides a simple and reliable way to execute tasks across multiple workers, with first-class Python support, predictable scheduling, retries, resource-aware routing, and cloud-friendly scalability.

Flux focuses on **AI, ML, and data processing pipelines**, making it a modern alternative to Celery—faster, safer, and easier to operate.

Flux is written in Rust, giving it strong guarantees around performance, reliability, and concurrency.

<p align="center">
<strong>
<a href="#getting-started">Quick Start</a> • 
<a href="#rust-worker">Rust Worker</a> • 
<a href="ROADMAP.md">Roadmap</a> • 
<a href="#contributing">Contributing</a>
</strong>
</p>

---

## 🚀 Features

- ⚡ **High-performance async worker runtime** (Rust + Tokio)  
- 🐍 **Python SDK** with a simple `@task` decorator  
- 🔁 **Retries with exponential backoff**  
- ⏰ **Scheduled & delayed jobs**  
- 🧵 **Concurrent workers** with configurable queue bindings  
- 🧠 **Resource-aware scheduling** (CPU/GPU, memory classes)  
- 🔌 **Pluggable brokers** (Redis first, more coming)  
- 🌐 **HTTP API & monitoring UI** (coming soon)  
- ☁️ Works locally, on VMs, containers, or Kubernetes  

---

## Getting Started

### Python SDK

Install:

```bash
pip install flux-py
