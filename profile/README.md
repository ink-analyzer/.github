# 🦑 ink! Analyzer

A collection of modular and reusable libraries and tools for semantic analysis of [ink!](https://use.ink/) smart contract code.

ink! analyzer aims to improve [ink!](https://use.ink/) language support in [integrated development environments (IDEs)](https://en.wikipedia.org/wiki/Integrated_development_environment), [source code editors](https://en.wikipedia.org/wiki/Source-code_editor) and other development tools by providing modular and reusable building blocks for implementing features like diagnostic errors, code completion suggestions, code/intent actions and hover content for the [ink! programming language](https://use.ink/) which is used for writing smart contracts for blockchains built on [Substrate](https://substrate.io/).

## Components

### 1. 🔬 [Semantic Analyzer](https://github.com/ink-analyzer/ink-analyzer)

A modular domain-specific semantic analysis library for ink!.
It's responsible for parsing the smart contract code, analyzing it based on ink!'s semantic rules for smart contracts and returning semantic information for other components to consume.

### 2. 🗣 Language Server (coming soon - June/2023)

A [Language Server Protocol (LSP)](https://microsoft.github.io/language-server-protocol/) implementation built on top of the semantic analyzer.
It acts as a backend that provides language support features to IDEs, code editors and other development tools.
It can be reused by multiple IDEs, code editors and other development tools that support LSP servers including [Visual Studio Code, Visual Studio, Vim / Neovim, Emacs, Atom, Sublime Text, Acme, Lapce, Eclipse and many more](https://microsoft.github.io/language-server-protocol/implementors/tools/).

### 3. 👩‍💻 Extensions/plugins/integrations for IDEs and code editors (coming soon - Q2/2023)

Extensions/plugins/integrations add ink! language support to IDEs, code editors and other development tools. 
They communicate with the language server running as a separate process using the [Language Server Protocol](https://microsoft.github.io/language-server-protocol/) via [JSON-RPC](https://www.jsonrpc.org/).

Planned extensions/plugins/integrations:
- Visual Studio Code Extension (Q2/2023)
- IntelliJ Plugin (Q2/2023)


**NOTE:** ink! Analyzer is still in early stages of development, check back over the next few weeks for regular updates.

💬 Twitter: [@davidsemakula](https://twitter.com/davidsemakula).

🌱 Funded by: the [Web3 Foundation](https://web3.foundation/).