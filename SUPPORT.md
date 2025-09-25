# Supporting Guide to Linera Documentation Repository

Welcome to this supporting guide for the [linera-io/linera-documentation](https://github.com/linera-io/linera-documentation) repository. This repository contains the source files for the Linera developer documentation, hosted at [linera.dev](https://linera.dev). The docs are built using mdBook, with Markdown files organized primarily under the `src/` directory. Navigating the raw files can be challenging due to nested folders, so this guide provides a logical, educational sequence to explore the content.

This guide is designed for both technical developers (who may dive into code examples and SDK details) and non-technical users (who can focus on high-level concepts and overviews). We'll start with foundational knowledge and build progressively, helping you assimilate information step by step. Each section includes:

- **Overview**: A brief explanation of what the section covers and why it's important.
- **Key Files**: Relative paths to relevant Markdown files in the repo (e.g., `src/section/subsection.md`). You can view them directly on GitHub by appending `/blob/main/` to the repo URL (e.g., https://github.com/linera-io/linera-documentation/blob/main/src/protocol/overview.md).
- **Learning Path**: Suggested reading order, with tips on how to connect concepts.
- **Transitions**: Guidance on moving to the next section for smooth knowledge building.

The structure mirrors the three main parts of the Linera Manual (High-Level Overview, Developers, Operators), plus appendices. Start at the beginning for a complete understanding, or jump to sections based on your needs.

## 1. High-Level Overview (Protocol Fundamentals)
This part introduces the Linera protocol at a conceptual level. It's ideal for beginners or non-developers to grasp what Linera is, its use cases, and future direction without technical deep dives. Developers can use this as a foundation before coding.

### Key Concepts Covered
- Core ideas behind Linera's scalable, low-latency design for Web3 apps.
- Real-world applications and benefits.
- Upcoming developments.

### Key Files
- `src/protocol/overview.md` : Main introduction to the protocol.
- `src/protocol/use_cases.md` : Examples of practical implementations.
- `src/protocol/roadmap.md` : Future plans and milestones.

### Learning Path
1. Begin with `src/protocol/overview.md` to understand Linera's unique architecture (e.g., multi-chain approach for unlimited users).<grok:render card_id="ad180f" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">32</argument>
</grok:render>
2. Move to `src/protocol/use_cases.md` to see how it solves real problems like user scalability without compromising security.<grok:render card_id="e672b6" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">33</argument>
</grok:render>
3. End with `src/protocol/roadmap.md` to contextualize current features with future enhancements.<grok:render card_id="562911" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">31</argument>
</grok:render>

**Tips**: Non-devs, focus on diagrams and summaries. Devs, note how the protocol enables app development. This builds curiosity for hands-on sections.

**Transition**: Once you understand the "why" of Linera, proceed to the Developers section to learn the "how" of building on it.

## 2. Developers Guide (Building Applications)
This is the core for developers, covering installation, SDK usage, and advanced topics. Non-devs can skim for insights into how apps work on Linera. The content is sequenced from setup to complex features, allowing gradual skill-building.

### 2.1 Getting Started
Start here to set up your environment and run your first app.

#### Key Files
- `src/developers/getting_started.md` : Overview of toolchain.
- `src/developers/getting_started/installation.md` : Step-by-step setup.
- `src/developers/getting_started/hello_linera.md` : Simple example app.

#### Learning Path
1. Read `src/developers/getting_started.md` for an intro to tools.<grok:render card_id="b7831b" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">37</argument>
</grok:render>
2. Follow `src/developers/getting_started/installation.md` to install from crates.io or source.<grok:render card_id="bfdb31" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">71</argument>
</grok:render>
3. Build and deploy in `src/developers/getting_started/hello_linera.md` using testnet or local net.<grok:render card_id="1a6b6c" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">70</argument>
</grok:render>

**Tips**: Practice commands in a terminal for retention. Non-devs, read for high-level flow.

### 2.2 Core Concepts
Deepen understanding of key protocol elements.

#### Key Files
- `src/developers/core_concepts.md` : Detailed explanations.

#### Learning Path
- Read the entire file to connect concepts like chains and executions.<grok:render card_id="48cdb3" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">36</argument>
</grok:render>

**Transition**: With basics in place, move to backend/frontend for app creation.

### 2.3 Writing Backends
Focus on Rust-based smart contracts and services.

#### Key Files
- `src/developers/backend.md` : Introduction.
- `src/developers/backend/creating_a_project.md` : Project setup.
- `src/developers/backend/abi.md` : Defining interfaces.
- `src/developers/backend/contract.md` : Contract logic.
- `src/developers/backend/service.md` : GraphQL services.
- `src/developers/backend/composition.md` : Cross-app calls.
- `src/developers/backend/messages.md` : Cross-chain communication.
- `src/developers/backend/testing.md` : Unit/integration tests.
- `src/developers/backend/logging.md` : Debugging logs.

#### Learning Path
1. Start with `src/developers/backend.md` and `src/developers/backend/creating_a_project.md` to scaffold a project.<grok:render card_id="a233d6" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">51</argument>
</grok:render><grok:render card_id="b2c7dc" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">59</argument>
</grok:render>
2. Define ABI in `src/developers/backend/abi.md`.<grok:render card_id="38f8ca" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">55</argument>
</grok:render>
3. Implement contract and service in the respective files.<grok:render card_id="dc340c" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">52</argument>
</grok:render><grok:render card_id="5d6d6e" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">53</argument>
</grok:render>
4. Add advanced features like composition and messages.<grok:render card_id="7896d1" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">54</argument>
</grok:render><grok:render card_id="5da81e" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">57</argument>
</grok:render>
5. Test and log as per the last files.<grok:render card_id="0f7c1d" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">56</argument>
</grok:render><grok:render card_id="cae712" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">58</argument>
</grok:render>

**Tips**: Build a sample app incrementally, testing at each step.

### 2.4 Writing Frontends
Connect UIs to backends using JS/WebAssembly.

#### Key Files
- `src/developers/frontend.md` : Intro.
- `src/developers/frontend/overview.md` : Architecture.
- `src/developers/frontend/setup.md` : HTML scaffolding.
- `src/developers/frontend/interactivity.md` : JS integration.

#### Learning Path
1. Overview and setup first.<grok:render card_id="b7a31d" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">60</argument>
</grok:render><grok:render card_id="6bbd62" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">63</argument>
</grok:render><grok:render card_id="598608" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">61</argument>
</grok:render>
2. Add interactivity.<grok:render card_id="e0af2f" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">62</argument>
</grok:render>

**Tips**: Non-devs, focus on how frontends interact with blockchain.

### 2.5 Experimental Features
Explore cutting-edge integrations.

#### Key Files
- `src/developers/experimental.md` : Overview.
- `src/developers/experimental/ml.md` : Machine learning.
- `src/developers/experimental/ethereum.md` : EVM compatibility.

#### Learning Path
- Read in order for emerging capabilities.<grok:render card_id="ce491d" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">77</argument>
</grok:render><grok:render card_id="725220" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">78</argument>
</grok:render><grok:render card_id="7caea5" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">79</argument>
</grok:render>

### 2.6 Advanced Topics
For deeper protocol insights.

#### Key Files
- `src/developers/advanced_topics.md` : Intro.
- `src/developers/advanced_topics/block_creation.md` : Block mechanics.
- `src/developers/advanced_topics/validators.md` : Node operations.
- `src/developers/advanced_topics/contract_finalize.md` : Execution finalization.
- `src/developers/advanced_topics/assets.md` : Asset management.

#### Learning Path
- Tackle one topic at a time, referencing core concepts.<grok:render card_id="9e4143" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">64</argument>
</grok:render><grok:render card_id="c658de" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">65</argument>
</grok:render><grok:render card_id="2a3217" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">66</argument>
</grok:render><grok:render card_id="077d38" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">67</argument>
</grok:render><grok:render card_id="855c51" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">68</argument>
</grok:render>

**Transition**: With app-building knowledge, learn operations for deployment.

## 3. Operators Guide (Running Infrastructure)
For those running nodes or networks. Devs can use this for local testing; non-devs for understanding infrastructure.

### 3.1 Devnets
Local development networks.

#### Key Files
- `src/operators/devnets.md` : Overview.
- `src/operators/devnets/kind.md` : Kubernetes setup.
- `src/operators/devnets/compose.md` : Docker Compose.

#### Learning Path
1. Start with overview.<grok:render card_id="436537" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">72</argument>
</grok:render>
2. Choose tool: Kind or Compose.<grok:render card_id="ff9011" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">73</argument>
</grok:render><grok:render card_id="365728" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">74</argument>
</grok:render>

### 3.2 Testnets
Public test environments.

#### Key Files
- `src/operators/testnets.md` : Overview.
- `src/operators/testnets/manual-installation.md` : Setup guide.

#### Learning Path
- Read overview, then install.<grok:render card_id="6c588a" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">75</argument>
</grok:render><grok:render card_id="2b674a" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">76</argument>
</grok:render>

**Tips**: Practice on devnets before testnets.

**Transition**: Wrap up with appendices for references.

## 4. Appendix (Additional Resources)
Supplementary materials.

### Key Files
- `src/appendix/glossary.md` : Terms definitions.
- `src/appendix/videos.md` : Video tutorials.

### Learning Path
- Use glossary for quick lookups.<grok:render card_id="e41a17" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">44</argument>
</grok:render>
- Watch videos for visual explanations.<grok:render card_id="cd51c8" card_type="citation_card" type="render_inline_citation">
<argument name="citation_id">45</argument>
</grok:render>

## Additional Repo Navigation Tips
- **Root Files**: Check `README.md` for build instructions, `book.toml` for mdBook config, and `src/SUMMARY.md` for the raw table of contents.
- **Building Locally**: Follow root README to run mdBook and view docs locally.
- **Contributing**: See issue #205 for ideas like chatbots; contribute by editing md files and PRs.
- **Search Tip**: Use GitHub search in the repo for keywords across files.

This guide sequences content to build knowledge progressively: concepts → building → operating → references. Revisit sections as needed for reinforcement. For updates, check the repo commits.
