# AI Agent Benchmark Compendium

This post provides a high-level overview to over 50 of modern benchmarks, grouped into four key categories Function Calling and Tool Use, General Assistant and Reasoning, Coding and Software Engineering and Computer Interactions.

Would love to keep this up to date and extend when need benchmarks are coming up. Please Open PRs or Issues. 

## Function Calling & Tool Use

### BFCL (Berkeley Function Calling Leaderboard)

BFCL is a comprehensive benchmark designed to evaluate the function calling (also known as tool use) capabilities of Large Language Models (LLMs) in a wide range of real-world settings. It assesses models across various scenarios, including serial (simple), parallel, and multi-turn interactions, and evaluates agentic capabilities such as reasoning in stateful multi-step environments, memory, web search, and format sensitivity.

Links: [Paper](https://openreview.net/pdf?id=2GmDdhBdDk) | [GitHub](https://github.com/ShishirPatil/gorilla/tree/main/berkeley-function-call-leaderboard) | [Leaderboard](https://gorilla.cs.berkeley.edu/leaderboard.html) | [Dataset](https://huggingface.co/datasets/gorilla-llm/Berkeley-Function-Calling-Leaderboard)

### ToolBench

A massive-scale benchmark designed for evaluating and facilitating large language models in mastering over 16,000 real-world RESTful APIs. It functions as an instruction-tuning dataset for tool use, which was automatically generated using ChatGPT to enhance the general tool-use capabilities of large language models.

Links: [Paper](https://arxiv.org/abs/2307.16789) | [GitHub](https://github.com/OpenBMB/ToolBench) | [Leaderboard](https://huggingface.co/spaces/qiantong-xu/toolbench-leaderboard) | [Dataset](https://huggingface.co/datasets/Maurus/ToolBench)

### ComplexFuncBench

A benchmark specifically designed for the evaluation of complex function calling in LLMs. It addresses challenging scenarios across five key aspects: multi-step function calls within a single turn, function calls involving user-provided constraints, parameter value reasoning, calls with long parameter values, and calls requiring a 128k long-context length.

Links: [Paper](https://arxiv.org/abs/2501.10132) | [GitHub](https://github.com/THUDM/ComplexFuncBench) | [Dataset](https://huggingface.co/datasets/zai-org/ComplexFuncBench)

### τ-Bench/Tau-Bench

A conversational benchmark designed to test AI agents in dynamic, open-ended real-world scenarios. It specifically evaluates an agent's ability to interact with simulated human users and programmatic APIs while strictly adhering to domain-specific policies and maintaining consistent behavior, with domains in e-commerce and airline reservations.

Links: [Paper](https://arxiv.org/abs/2406.12045) | [GitHub](https://github.com/sierra-research/tau-bench) | [Leaderboard](https://github.com/sierra-research/tau-bench#leaderboard)

### Composio Function Calling Benchmark

Tests the ability of LLMs to correctly call functions based on given prompts. It comprises 50 function calling problems, each designed to be solved using one of eight provided function schemas inspired by real-world API structures from ClickUp's integration endpoints.

Links: [GitHub](https://github.com/ComposioHQ/Composio-Function-Calling-Benchmark)

### API-Bank: A Comprehensive Benchmark for Tool-Augmented LLMs

Evaluates an agent's ability to plan step-by-step API calls, retrieve relevant APIs, and correctly execute API calls to meet human needs based on understanding real-world API documentation. It features over 2,200 dialogues utilizing thousands of APIs.

Links: [Paper](https://arxiv.org/pdf/2304.08244.pdf) | [GitHub](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/api-bank)

### HammerBench: Fine-Grained Function-Calling Evaluation in Real Mobile Device Scenarios

A novel benchmark designed to evaluate the function-calling capabilities of LLMs in realistic, multi-turn human-agent interactions, particularly simulating mobile assistant use cases. It tests models under challenging circumstances like imperfect instructions and shifts in user intent.

Links: [Paper](https://arxiv.org/abs/2412.16516) | [GitHub](https://github.com/MadeAgents/HammerBench) | [Dataset](https://huggingface.co/datasets/MadeAgents/HammerBench)

### DPAB-α

The Dria Pythonic Agent Benchmark is a comprehensive benchmark designed to evaluate the function calling capabilities of LLMs. It specifically compares the performance of models using Pythonic function calling versus traditional JSON-based methods across 100 problems.

Links: [Blog](https://huggingface.co/blog/andthattoo/dpab-a)

### NFCL (Nexus Function Calling Leaderboard)

A benchmark designed to evaluate the proficiency of LLMs in single-turn function calling tasks. It assesses various complexities, including simple, parallel, and nested function calls, where the output of one function serves as an input for another.

Links: [GitHub](https://github.com/nexusflowai/NexusRaven-V2) | [Leaderboard](https://huggingface.co/spaces/Nexusflow/Nexus_Function_Calling_Leaderboard)

### xLAM: A Family of Large Action Models for Function Calling and AI Agent Systems

A series of large action models (LLMs) developed by Salesforce AI Research, specifically optimized for function calling and AI agent tasks. These models are designed to enhance the generalizability and performance of AI agents across diverse environments.

Links: [Paper](https://arxiv.org/abs/2409.03215) | [GitHub](https://github.com/SalesforceAIResearch/xLAM)

### ToolACE: A Framework for Generating High-Quality Tool-Learning Data for LLMs

An automatic agentic pipeline meticulously designed to generate accurate, complex, and diverse tool-learning data, specifically tailored to enhance the function-calling capabilities of LLMs.

Links: [Paper](https://arxiv.org/abs/2409.00920)

### MCPMark

An evaluation suite for agentic models in real MCP tool environments (Notion / GitHub / Filesystem / Postgres / Playwright). MCPMark provides a reproducible, extensible benchmark for researchers and engineers with one-command tasks, isolated sandboxes, auto-resume for failures, unified metrics, and aggregated reports.

Links: [Paper](https://arxiv.org/abs/2509.24002) | [HuggingFace Daily Paper](https://huggingface.co/papers/2509.24002) | [GitHub](https://github.com/eval-sys/mcpmark) | [Website](https://mcpmark.ai) | [Dataset](https://huggingface.co/datasets/Jakumetsu/mcpmark-trajectory-log)

### LiveMCPBench

A comprehensive benchmark designed to evaluate the ability of LLM agents to navigate and effectively utilize a large-scale Model Context Protocol (MCP) toolset in real-world scenarios, overcoming limitations of single-server environments.

Links: [Paper](https://arxiv.org/abs/2508.01780) | [GitHub](https://icip-cas.github.io/LiveMCPBench) | [Leaderboard](https://docs.google.com/spreadsheets/d/1EXpgXq1VKw5A7l7-N2E9xt3w0eLJ2YPVPT-VrRxKZBw/edit?gid=0#gid=0) | [Dataset](https://huggingface.co/datasets/ICIP/LiveMCPBench)

### MCP-Universe

A comprehensive framework and benchmark for developing, testing, and evaluating AI agents and LLMs through direct interaction with real-world Model Context Protocol (MCP) servers, rather than relying on simulations, covering domains like financial analysis and browser automation.

Links: [Paper](https://arxiv.org/pdf/2508.14704.pdf) | [GitHub](https://github.com/SalesforceAIResearch/MCP-Universe) | [Leaderboard](https://mcp-universe.github.io/)

---

## General Assistant & Reasoning

### GAIA (General AI Assistants)

A landmark benchmark designed to evaluate General AI Assistants, posing real-world questions that are conceptually simple for humans but significantly challenging for most advanced AI systems. It requires AI models to demonstrate a combination of fundamental abilities, including reasoning, multi-modality handling, web browsing, and proficient tool use.

Links: [Paper](https://arxiv.org/abs/2311.12983) | [Leaderboard](https://huggingface.co/spaces/gaia-benchmark/leaderboard) | [Dataset](https://huggingface.co/datasets/gaia-benchmark/GAIA)

### AgentBench: A Comprehensive Benchmark for Evaluating LLMs as Agents

A multi-dimensional, evolving benchmark designed to thoroughly assess the reasoning and decision-making capabilities of LLMs when functioning as autonomous agents. It encompasses eight distinct environments, including Operating System, Database, and Web Shopping.

Links: [Paper](https://arxiv.org/abs/2308.03688) | [GitHub](https://github.com/THUDM/AgentBench) | [Leaderboard](https://github.com/THUDM/AgentBench?tab=readme-ov-file#leaderboard) | [Dataset](https://github.com/THUDM/AgentBench#dataset-summary)

### AssistantBench

A challenging benchmark designed to evaluate the ability of web agents to automatically solve realistic and time-consuming tasks. It comprises 214 tasks that require navigating the open web, spanning multiple domains, and interacting with over 525 pages from 258 different websites.

Links: [Paper](https://arxiv.org/abs/2407.15711) | [GitHub](https://github.com/oriyor/assistantbench) | [Leaderboard](https://huggingface.co/spaces/AssistantBench/leaderboard) | [Dataset](https://huggingface.co/datasets/AssistantBench/AssistantBench)

### LiveBench: A Challenging, Contamination-Free Benchmark for LLMs

A challenging, contamination-free benchmark for LLMs that regularly releases new questions from recent information sources to ensure models are tested on novel problems rather than memorized answers.

Links: [Paper](https://arxiv.org/abs/2406.19314) | [GitHub](https://github.com/livebench/livebench) | [Leaderboard](https://livebench.ai/) | [Dataset](https://huggingface.co/datasets/livebench)

### Humanity's Last Exam (HLE)

A highly challenging, multi-modal benchmark with 2,500 expert-level academic questions across a broad range of disciplines, designed to test models at the absolute frontier of human knowledge and require genuine reasoning capabilities rather than simple factual recall.

Links: [Paper](https://arxiv.org/abs/2501.14249) | [GitHub](https://github.com/centerforaisafety/hle) | [Leaderboard](https://lastexam.ai/) | [Dataset](https://huggingface.co/datasets/cais/hle)

### FORTRESS: Frontier Risk Evaluation for National Security and Public Safety

A benchmark designed to evaluate the robustness of LLM safeguards against potential misuse relevant to national security and public safety, using expert-crafted adversarial prompts across domains like CBRNE and political violence.

Links: [Paper](https://arxiv.org/abs/2506.14922) | [Leaderboard](https://scale.com/leaderboard/fortress)

### The MASK Benchmark: Disentangling Honesty from Accuracy in AI Systems

Aims to evaluate the honesty of LLMs by disentangling it from factual accuracy. The benchmark measures whether models will knowingly contradict their established beliefs when subjected to pressure to lie.

Links: [Paper](https://arxiv.org/abs/2503.03750) | [GitHub](https://github.com/centerforaisafety/mask) | [Leaderboard](https://scale.com/leaderboard/mask)

### SimpleQA

A factuality benchmark designed to evaluate the ability of LLMs to answer short, fact-seeking questions. It aims to measure how well models "know what they know" and to identify "hallucinations" or factually incorrect outputs with single, indisputable answers.

Links: [Paper](https://cdn.openai.com/papers/simpleqa.pdf) | [GitHub](https://github.com/openai/simple-evals) | [Dataset](https://huggingface.co/datasets/basicv8vc/SimpleQA)

### SimpleQA Verified

A 1,000-prompt benchmark designed for evaluating the short-form factuality of LLMs, developed to address limitations in the original SimpleQA benchmark, such as noisy labels and topical biases, through a rigorous filtering process.

Links: [Paper](https://arxiv.org/abs/2509.07968) | [Leaderboard](https://www.kaggle.com/benchmarks/deepmind/simpleqa-verified) | [Dataset](https://www.kaggle.com/benchmarks/deepmind/simpleqa-verified)

### FACTS Grounding

Evaluates LLMs' ability to generate long-form responses that are factually accurate and strictly "grounded" in provided context documents, thereby mitigating hallucination. Tasks require models to generate responses based exclusively on documents up to 32,000 tokens long.

Links: [Paper](https://deepmind.google/discover/blog/facts-grounding-a-new-benchmark-for-evaluating-the-factuality-of-large-language-models/) | [GitHub](https://github.com/google-deepmind/long-form-factuality) | [Leaderboard](https://www.kaggle.com/facts-leaderboard) | [Dataset](https://www.kaggle.com/facts-leaderboard)

### Galileo Agent Leaderboard v2

Provides comprehensive performance metrics for LLM agents across business domains.

Links: [Paper](https://galileo.ai/blog/agent-leaderboard) | [GitHub](https://github.com/rungalileo/agent-leaderboard) 

---

## Coding & Software Engineering

### SWE-bench: Evaluating AI in Real-World Software Engineering

A benchmark for evaluating LLMs and AI agents on their ability to resolve real-world software engineering issues. It comprises 2,294 problems sourced from GitHub issues across 12 popular Python repositories. The task is to generate a patch that resolves the issue.

Links: [Paper](https://arxiv.org/abs/2310.06770) | [GitHub](https://github.com/SWE-bench/SWE-bench) | [Leaderboard](https://swebench.com/) | [Dataset](https://www.swebench.com/SWE-bench/guides/datasets/)

### SWE-bench Verified

SWE-bench Verified is a human-validated subset of the original SWE-bench dataset, containing 500 samples that assess the capability of AI models to resolve real-world software engineering issues. To improve the reliability of evaluation, SWE-bench Verified was created in collaboration with OpenAI and involved professional software developers who screened each sample to ensure well-specified issue descriptions and appropriate unit tests. 

Links: [Blog](https://openai.com/index/introducing-swe-bench-verified/) | [Leaderboard](https://www.swebench.com/)

### SWE-Bench Pro:

A benchmark for evaluating LLMs and AI agents on their ability to resolve real-world software engineering issues. It comprises 1,865 problems sourced from 41 diverse professional repositories. The task is to generate a patch that resolves the issue. Hidden Test set with 276 additional private tasks.

Links: [Paper](https://t.co/5ArWF1bKmS)  | [GitHub](https://github.com/scaleapi/SWE-bench_Pro-os/tree/main?tab=readme-ov-file) | [Leaderboard](https://scale.com/leaderboard/swe_bench_pro_public) | [Dataset](https://huggingface.co/datasets/ScaleAI/SWE-bench_Pro)

### LiveCodeBench

A holistic and contamination-free benchmark for evaluating LLMs for code-related tasks. It continuously collects new problems from competitive programming platforms and assesses capabilities like self-repair, code execution, and test output prediction.

Links: [Paper](https://arxiv.org/abs/2403.07974) | [GitHub](https://github.com/LiveCodeBench/LiveCodeBench) | [Leaderboard](https://www.kaggle.com/benchmarks/open-benchmarks/livecodebench)

### SWE-PolyBench: A Multi-Language Benchmark for AI Coding Agents

A multi-language benchmark designed to evaluate AI coding agents across diverse programming tasks and languages. It contains over 2,000 curated issues from 21 real-world repositories, covering Java, JavaScript, TypeScript, and Python.

Links: [Paper](https://arxiv.org/pdf/2504.08703) | [GitHub](https://github.com/amazon-science/SWE-PolyBench) | [Leaderboard](https://amazon-science.github.io/SWE-PolyBench/)

### Aider's "AI-Assisted Code" Benchmarks

A set of practical evaluations designed to measure how effectively LLMs can edit, refactor, and contribute to an existing codebase. These benchmarks include a code editing benchmark, a challenging refactoring benchmark, and a polyglot benchmark.

Links: [GitHub](https://github.com/Aider-AI/aider) | [Leaderboard](https://aider.chat/docs/leaderboards/)

### Aider Polyglot Benchmark

Evaluates coding and self-correction abilities of LLMs by testing them on 225 challenging Exercism coding exercises across multiple languages, including C++, Go, Java, JavaScript, Python, and Rust.

Links: [GitHub](https://github.com/Aider-AI/polyglot-benchmark) | [Leaderboard](https://aider.chat/docs/leaderboards/)

---

## Computer Interaction (GUI & Web)

### WebArena: A Realistic Web Environment for Building Autonomous Agents

A standalone, self-hostable web environment for building autonomous agents. WebArena creates websites from four popular categories with functionality and data mimicking their real-world equivalents and introduces a benchmark on interpreting high-level commands.

Links: [Paper](https://arxiv.org/pdf/2307.13854.pdf) | [GitHub](https://github.com/web-arena-x/webarena)

### VisualWebArena

A benchmark designed to assess the performance of multimodal agents on realistic, visually grounded web tasks. It extends WebArena with 910 new, diverse, and complex tasks that require agents to accurately process image-text inputs and execute actions on websites.

Links: [Paper](https://aclanthology.org/2024.acl-long.50/) | [GitHub](https://github.com/web-arena-x/visualwebarena)

### Web Bench: A Benchmark for AI Browser Agents

A benchmark designed to evaluate the performance of AI browser agents. It differentiates agent capabilities on information retrieval (READ) tasks from state-changing (WRITE) tasks across 452 live websites, encompassing 5,750 tasks.

Links: [Paper](https://halluminate.ai/blog/benchmark) | [GitHub](https://github.com/Halluminate/WebBench) | [Dataset](https://huggingface.co/datasets/Halluminate/WebBench)

### WebVoyager

A foundational benchmark designed for evaluating Large Multimodal Models (LMMs) and web agents on end-to-end, real-world navigation tasks across a diverse set of popular, live websites, integrating both textual (HTML) and visual (screenshots) information.

Links: [Paper](https://arxiv.org/abs/2401.13919) | [GitHub](https://github.com/MinorJerry/WebVoyager) | [Leaderboard](https://leaderboard.steel.dev/)

### BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents

A simple yet challenging benchmark to measure the ability of agents to browse the web. It consists of 1,266 questions that demand persistent navigation of the internet to find hard-to-find, entangled information.

Links: [Paper](https://arxiv.org/abs/2504.12516) | [GitHub](https://github.com/openai/simple-evals/tree/main)

### Mind2Web

A comprehensive benchmark for developing and evaluating generalist web agents. The original dataset includes over 2,000 open-ended tasks collected from 137 real-world websites, with variants for evaluating performance on live websites.

Links: [Paper](https://arxiv.org/abs/2306.06070) | [GitHub](https://github.com/osu-nlp-group/Mind2Web) | [Leaderboard](https://huggingface.co/spaces/osunlp/Online_Mind2Web_Leaderboard) | [Dataset](https://huggingface.co/datasets/osunlp/Mind2Web)

### WebGames Benchmark

A comprehensive benchmark suite to evaluate general-purpose web-browsing AI agents, featuring over 50 interactive challenges crafted to be straightforward for humans but challenging for AI. It operates in a self-contained, hermetic testing environment.

Links: [Paper](https://arxiv.org/abs/2502.18356) | [GitHub](https://github.com/convergence-ai/webgames) | [Leaderboard](https://webgames.convergence.ai/) | [Dataset](https://huggingface.co/datasets/convergence-ai/webgames)

### ST-WebAgentBench

A benchmarking platform specifically designed to evaluate the safety and trustworthiness of autonomous web agents in realistic enterprise contexts, where policy compliance and safety are paramount.

Links: [Paper](https://arxiv.org/abs/2410.06703) | [GitHub](https://github.com/segev-shlomov/ST-WebAgentBench)

### OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments

A first-of-its-kind scalable, real computer environment for benchmarking multimodal agents on open-ended tasks within genuine operating systems, including Windows, macOS, and Ubuntu, featuring 369 real-world tasks.

Links: [Paper](https://arxiv.org/abs/2404.07972) | [GitHub](https://os-world.github.io/)

### OSUniverse

A benchmark for evaluating advanced GUI-navigation AI agents on complex, multimodal, desktop-oriented tasks. It features 160 tasks across five levels of complexity and nine categories, designed to be easy for humans but challenging for AI.

Links: [Paper](https://arxiv.org/abs/2505.03570) | [GitHub](https://github.com/agentsea/osuniverse)

### ScreenSuite Benchmark

A comprehensive suite of 13 benchmarks for evaluating Graphical User Interface (GUI) agents, focusing on the Vision Language Models (VLMs) that power them. It uses a vision-only evaluation stack without relying on accessibility trees or DOM information.

Links: [GitHub](https://github.com/huggingface/screensuite)

### WorkArena++ Benchmark: Enhanced Evaluation for AI in Enterprise Workflows

A novel benchmark to rigorously evaluate AI agents in performing complex, realistic enterprise workflows. It expands upon the original WorkArena benchmark with 682 tasks that mimic the intricate operations of knowledge workers on the ServiceNow platform.

Links: [Paper](https://arxiv.org/abs/2407.05291)

### AndroidWorld Benchmark

A dynamic benchmarking environment for autonomous agents that control mobile devices. It operates on a live Android emulator and features 116 hand-crafted tasks across 20 real-world Android applications, with millions of unique task variations.

Links: [Paper](https://arxiv.org/abs/2405.14573) | [GitHub](https://github.com/google-research/android_world)

### WorldGUI

A comprehensive Graphical User Interface (GUI) benchmark designed to evaluate AI agents across ten widely used desktop and web applications (e.g., PowerPoint, VSCode). It features 315 tasks with diverse initial states to simulate authentic human-computer interactions.

Links: [Paper](https://arxiv.org/abs/2502.08047) | [GitHub](https://github.com/showlab/WorldGUI)

### macOSWorld

The first comprehensive, multilingual, and interactive benchmark to evaluate GUI agents operating within the macOS environment. It features 202 multilingual tasks across 30 applications, with instructions and interfaces in five languages.

Links: [Paper](https://arxiv.org/abs/2506.04135) | [GitHub](https://github.com/showlab/macosworld)

### OfficeBench: Benchmarking Language Agents across Multiple Applications for Office Automation

A pioneering benchmark to evaluate an LLM agent's ability to automate complex office workflows across multiple applications, such as Word, Excel, and email. It assesses long-horizon planning and proficiency in switching between applications.

Links: [Paper](https://arxiv.org/abs/2407.19056) | [GitHub](https://github.com/zlwang-cs/OfficeBench)

### EEBD (Emergence Enterprise Benchmark Dataset)

Evaluates AI agents in realistic enterprise scenarios that require them to go beyond simple browser interaction, intelligently selecting tools like APIs and combining web UI interaction with API calls.

Links: [Paper](https://github.com/EmergenceAI/emergence-benchmarks/blob/main/papers/e-web/e-web-v0.pdf) | [GitHub](https://github.com/EmergenceAI/emergence-benchmarks) | [Dataset](https://github.com/EmergenceAI/emergence-benchmarks/blob/main/benchmarks/e-web/e-web_benchmark_lite.csv)

### ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks

A benchmark for learning a mapping from natural language instructions and egocentric vision to sequences of actions for household tasks. It features long, compositional tasks in a simulated 3D environment.

Links: [Paper](https://arxiv.org/abs/1912.01734) | [GitHub](https://github.com/askforalfred/alfred) | [Leaderboard](https://askforalfred.com/leaderboard/leaderboard.html)

### EmbodiedBench

A comprehensive benchmark designed to evaluate Multi-modal Large Language Models (MLLMs) as embodied agents. It spans diverse tasks in navigation, manipulation, and high-level planning across four simulated environments.

Links: [Paper](https://arxiv.org/abs/2502.09560) | [GitHub](https://github.com/EmbodiedBench/EmbodiedBench)
