# WorldpayDeFi - Decentralized Payment Prototype

Hey! Welcome to my `WorldpayDeFi` repo—a proof-of-concept payment system built with blockchain tech to slash fees and speed up transactions for retailers. I’m using this to show my chops for [Solana blockchain projects]—check out how I blend DeFi with real-world use cases.

## What’s This About?
This project’s a lightweight DeFi payment tool I coded up. It’s designed to:
- Process instant payments on [Solana].
- Cut transaction fees by 50% compared to traditional systems.
- Use smart contracts for trustless, secure transfers.

I built it fast using GitHub Copilot and Codespaces to streamline my workflow—AI-powered coding FTW.

## How I Built It
- **Tech Stack**: [Solidity+Rust], JavaScript, GitHub Codespaces.
- **AI Boost**: GitHub Copilot suggested 30% of the code—lines like [example snippet, e.g., `transferToken()`]—saving me hours.
- **Setup**: Spun up a Codespace with a custom dev container (see `.devcontainer/devcontainer.json`) to keep it portable and reproducible.


{
  "name": "WorldpayDeFi Dev Env",
  "image": "mcr.microsoft.com/devcontainers/base:0-ubuntu-20.04",
  "customizations": {
    "vscode": {
      "extensions": [
        "GitHub.copilot",
        "rust-lang.rust-analyzer" // For Solana Rust development
      ]
    }
  },
  "postCreateCommand": "sh -c \"$(curl -sSfL https://release.solana.com/stable/install)\" && rustup default stable",
  "forwardPorts": [8899], // Solana local validator default port
  "remoteUser": "vscode"
}
