# ![icon](/images/iconx32.png "icon") ink! Analyzer

A collection of modular and reusable libraries and tools for semantic analysis of [ink!](https://use.ink/) smart contracts.

ink! analyzer aims to improve [ink!](https://use.ink/) language support in [integrated development environments (IDEs)](https://en.wikipedia.org/wiki/Integrated_development_environment), [source code editors](https://en.wikipedia.org/wiki/Source-code_editor) and other development tools by providing modular and reusable building blocks for implementing features like diagnostic errors, code completion suggestions, code/intent actions and hover content for the [ink! programming language](https://use.ink/) which is used for writing smart contracts for blockchains built with [Substrate](https://substrate.io/).

- [Introductory blog post](https://analyze.ink/blog/introducing-ink-analyzer).

## Components

### 1. 🔬 [Semantic Analyzer](https://github.com/ink-analyzer/ink-analyzer/tree/master/crates/analyzer)

A modular domain-specific semantic analysis library for ink! built on a resilient and lossless parser.
It's responsible for parsing the smart contract code, analyzing it based on ink!'s semantic rules for smart contracts and returning semantic information for other components to consume.

### 2. 🗣 [Language Server](https://github.com/ink-analyzer/ink-analyzer/tree/master/crates/lsp-server)

A [Language Server Protocol (LSP)](https://microsoft.github.io/language-server-protocol/) implementation built on top of the semantic analyzer.
It acts as a backend that provides language support features to IDEs, code editors and other development tools.
It can be reused by multiple IDEs, code editors and other development tools that support LSP servers including [Visual Studio Code, Visual Studio, Vim / Neovim, Emacs, Atom, Sublime Text, Acme, Lapce, Eclipse and many more](https://microsoft.github.io/language-server-protocol/implementors/tools/).

### 3. 👩‍💻 Extensions/plugins/integrations for IDEs, code editors and other development tools

Extensions/plugins/integrations add ink! language support to IDEs, code editors and other development tools. 
They communicate with the language server running as a separate process using the [Language Server Protocol](https://microsoft.github.io/language-server-protocol/) via [JSON-RPC](https://www.jsonrpc.org/).

Planned extensions/plugins/integrations:
- [Visual Studio Code Extension](https://github.com/ink-analyzer/ink-vscode) ([Install from Marketplace](https://marketplace.visualstudio.com/items?itemName=ink-analyzer.ink-analyzer))
- IntelliJ Plugin (TBD)

🌱 Funded by: the [Web3 Foundation](https://web3.foundation/) and [Polkadot Treasury](https://polkadot.network/ecosystem/treasury/).