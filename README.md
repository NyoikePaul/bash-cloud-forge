# 🔥 Bash Cloud Forge

**Pure Bash toolkit for lightning-fast cloud server provisioning, hardening, monitoring & API deployments.**

Perfect for **DigitalOcean + AWS + Telegram** alerts. Built for Kenyan freelancers, DevOps engineers & full-stack agencies.

![Bash](https://img.shields.io/badge/Bash-4.4+-black?style=flat&logo=gnubash)
![License](https://img.shields.io/github/license/NyoikePaul/bash-cloud-forge)
[![CI](https://github.com/NyoikePaul/bash-cloud-forge/actions/workflows/bash-ci.yml/badge.svg)](https://github.com/NyoikePaul/bash-cloud-forge/actions)
![Stars](https://img.shields.io/github/stars/NyoikePaul/bash-cloud-forge)
![Last Commit](https://img.shields.io/github/last-commit/NyoikePaul/bash-cloud-forge)

---

## ✨ Features

- ⚡ **Zero dependencies** — Pure Bash (works on almost any Linux server)
- 🔒 **Strict Mode** + Enterprise safety (`set -euo pipefail`)
- 🌩️ DigitalOcean droplet provisioning & hardening
- 📡 AWS support (EC2, security groups, etc.)
- 📲 Telegram notifications & monitoring
- 📦 One-command deploy for APIs & web apps
- 🔄 Automated backups with retention policy
- 🧪 Built-in testing & CI with ShellCheck + shfmt

---

## 🚀 Quick Start

### 1. Clone & Setup
``bash
git clone https://github.com/NyoikePaul/bash-cloud-forge.git
cd bash-cloud-forge
cp .env.example .env
# Edit .env with your DO_TOKEN, TELEGRAM_BOT_TOKEN, etc.
chmod +x forge.sh

2. Basic Commandsbash

# Provision a new hardened server
./forge.sh provision web-server --region nairobi

# Deploy your application
./forge.sh deploy production

# Run full system backup
./forge.sh backup /var/www/myapp

# Test Telegram alerts
./forge.sh test

# Show help
./forge.sh help

 Project Structure

bash-cloud-forge/
├── forge.sh          # Main CLI entrypoint
├── lib/              # Core reusable functions
├── scripts/          # Atomic task scripts
├── examples/         # Usage examples
├── .github/workflows # CI: ShellCheck + shfmt
└── .env.example

 Pro VersionFree = Personal & learning use
Pro (KSh 1,099/mo) = Commercial license + premium templates + priority supportGet Pro → DevelopmentRun linting locally:bash

# ShellCheck + formatting check
find . -type f -name "*.sh" -exec shellcheck {} +

Made with  for Kenyan developers & hustlersStar the repo if it helps you ship faster! 

