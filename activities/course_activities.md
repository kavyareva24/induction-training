---
title: "Generative AI — Balanced Theory + Applied LLM Systems Track"
semester: "6"
status: "draft — revised syllabus + lesson plan (v4, + Hugging Face)"
---

# Course File Draft — Generative AI (Balanced Track)
## Generative model foundations (theory) + Transformers → Hugging Face → LangChain → RAG → LangGraph (applied), taught hands-on with Ollama

> **Why this shape:** Unit 1 gives students the actual "generative AI" landscape
> (AE/VAE, GANs, diffusion) as taxonomy/theory so the course earns its title,
> not just an "LLM app-building" elective. Units 2–4 then go deep on the
> Transformer/LLM branch of that landscape — since that's what's practically
> buildable in a semester. **Hugging Face** (Hub, model cards, `transformers`
> library) is introduced as the standard place models/datasets are found and
> loaded from directly, positioned right before **Ollama**, the free local
> no-API-key runtime used for every hands-on lab from that point on.

---

## Course Content (Units)

| Unit | Syllabus | Weightage |
|---|---|---|
| 1 | Foundations of Generative AI: probabilistic/latent-variable models, AE/VAE, GANs, Diffusion (theory + demos) | 25 Marks |
| 2 | Transformers & Attention (theory) + Hugging Face Hub/`transformers` + practical LLM usage via Ollama | 25 Marks |
| 3 | LangChain & RAG — orchestration, embeddings, vector databases, LLM/RAG evaluation (theory + labs) | 25 Marks |
| 4 | LangGraph agentic workflows + Multimodal generation & Responsible AI (theory + labs) | 25 Marks |

**CO mapping**
- **CO1** — Explain the landscape of generative model families: AE/VAE, GANs, and diffusion models *(Awareness)*
- **CO2** — Explain the Transformer/attention architecture and use pretrained models practically via Hugging Face and a local model runtime *(Both)*
- **CO3** — Build LLM applications using LangChain (chains, memory, tools) *(Both)*
- **CO4** — Design and tune RAG pipelines using embeddings and vector databases *(Advanced)*
- **CO5** — Evaluate LLM/RAG system outputs using quantitative evaluation methods *(Advanced)*
- **CO6** — Design agentic workflows with LangGraph and assess multimodal-generation and responsible-AI considerations *(Advanced)*

**Legend — Merrill's First Principles phase:** Act = Activation · Dem = Demonstration · App = Application · Int = Integration

---

## 11. Lesson Plan

| S.No | Unit / Topic | Merrill phase | Activity | Level | CO |
|---|---|---|---|---|---|
| 01 | **Unit 1** — What is Generative AI? Generative vs. discriminative modeling; taxonomy of model families | Act | Think–pair–share: sort familiar AI tools (ChatGPT, image generators, spam filters) into generative/discriminative buckets | A | CO1 |
| 02 | Probability & statistics refresher: distributions, likelihood, Bayes' rule for generative modeling | Dem | Instructor walkthrough of MLE on a toy dataset; students verify by hand on a second dataset | A | CO1 |
| 03 | Latent variable models & the concept of latent space | Dem | Visualization exercise: plot and interpret a 2D latent space of a small image dataset | A | CO1 |
| 04 | Autoencoders (AE): architecture, encoder–decoder, reconstruction loss | Dem/App | Short guided demo: run a pretrained AE on sample images, inspect reconstructions at different bottleneck sizes | A | CO1 |
| 05 | Variational Autoencoders (VAE): ELBO, reparameterization trick | Dem | Instructor derives ELBO on the board; students annotate each term with its intuitive meaning | Adv | CO1 |
| 06 | GANs: adversarial framework, generator vs. discriminator, training dynamics (mode collapse) | Dem | Role-play: "forger vs. detective" rounds, followed by demo of a pretrained GAN's outputs | Adv | CO1 |
| 07 | Diffusion models: forward & reverse diffusion process, DDPM core idea | Dem | Visual analogy activity: relate diffusion to progressively "un-blurring" noise, step by step | Adv | CO1 |
| 08 | Comparing generative model families: AE/VAE vs. GAN vs. Diffusion vs. Transformer-based LLMs — strengths, weaknesses, use-cases | Int | Structured debate: teams argue which model family is best suited to a given real-world scenario | Both | CO1 |
| 09 | **Unit 1 wrap-up** — explore outputs from pretrained VAE/GAN/Diffusion demos and classify strengths/weaknesses | App/Int | Lab: use free hosted demos (Hugging Face Spaces) to generate samples from each model family; write a short comparison report | Both | CO1 |
| 10 | **Unit 2** — Why RNNs/LSTMs struggle: long-range dependency problem | Act | Demo an LSTM failing on a long-dependency sentence; class discusses why | A | CO2 |
| 11 | Attention mechanism: intuition and math formulation | Dem | Manual attention-weight calculation on a short sentence, by hand | A | CO2 |
| 12 | Self-attention & multi-head attention | Dem/App | Lab: visualize attention heatmaps from a pretrained model on sample text | Adv | CO2 |
| 13 | "Attention Is All You Need" — full encoder–decoder Transformer walkthrough | Dem | Instructor builds architecture diagram block-by-block on board with Q&A at each block | A | CO2 |
| 14 | Positional encoding — why Transformers need it | Dem | Worked example: compute positional encodings for a short sequence, compare with/without | A | CO2 |
| 15 | Pretraining paradigms: autoregressive vs. masked; tokenization | Dem/App | Hands-on: tokenize sample text with BPE, inspect resulting tokens/subwords | A | CO2 |
| 16 | Hugging Face Hub: model cards, datasets, Spaces, licensing — where pretrained models actually come from | Dem | Guided tour: students browse the Hub, find and compare model cards for two similar models (size, license, intended use) | A | CO2 |
| 17 | Hands-on: load & run a pretrained model directly using the Hugging Face `transformers` library (pipeline API) | App | Lab: run a text-generation/classification pipeline in a notebook using a small HF model; inspect config, tokenizer, and outputs | Both | CO2 |
| 18 | Practical LLM usage: installing & running Ollama; Ollama vs. Hugging Face `transformers` — when to use which | App | Lab: install Ollama, pull a small model (e.g., llama3.2 / phi3), run first prompt from terminal; discuss trade-offs (ease-of-use vs. flexibility/control) vs. session 17 | Both | CO2 |
| 19 | Prompting basics: zero-shot, few-shot, system prompts | App | Lab: same task attempted with zero-shot vs. few-shot vs. system-prompt variants on Ollama; compare outputs | Both | CO2 |
| 20 | **Unit 2 wrap-up** — hands-on prompting lab | App/Int | Team lab: design a small prompt-engineering "playbook" for a chosen task, tested on Ollama | Both | CO2 |
| 21 | **Unit 3** — Why orchestration frameworks? Introduction to LangChain | Act | Discussion: what breaks when you try to build a multi-step LLM app with raw API calls only | A | CO3 |
| 22 | LangChain core abstractions: LLM wrappers, prompt templates; chains (simple & sequential) | Dem/App | Lab: build a 2-step sequential chain (e.g., summarize → translate) using LangChain + Ollama | Adv | CO3 |
| 23 | Memory in LangChain: conversation buffer & summary memory | Dem/App | Lab: add conversation memory to a chatbot; compare behavior with/without memory | Adv | CO3 |
| 24 | Embeddings: theory — how text becomes vectors, similarity metrics (cosine, dot product) | Dem | Instructor demo: generate embeddings using a Hugging Face `sentence-transformers` model, compute and interpret similarity scores | A | CO4 |
| 25 | Vector databases: indexing & similarity-search theory + hands-on setup | Dem/App | Lab: store document embeddings in Chroma/FAISS, run nearest-neighbor queries, inspect results | Adv | CO4 |
| 26 | Building a RAG pipeline: retriever + generator, via LangChain + Ollama | App | Lab: connect vector store retriever to Ollama LLM in LangChain; ask questions grounded in custom docs | Adv | CO4 |
| 27 | Chunking strategies & retrieval quality tuning | App | Lab: compare answer quality across different chunk sizes/overlaps on the same document set | Adv | CO4 |
| 28 | LLM/RAG evaluation theory: faithfulness, relevance, hallucination detection metrics | Dem | Instructor demo: run a RAG-eval framework (e.g., RAGAS) on sample Q&A pairs; interpret metrics | Adv | CO5 |
| 29 | **Unit 3 wrap-up** — build & evaluate a full RAG system | App/Int | Team lab: build a RAG assistant over a custom document set (local, via Ollama + HF embeddings) and report its eval scores | Adv | CO4–CO5 |
| 30 | **Unit 4** — From chains to graphs: why state, branching, and loops are needed | Act | Discussion: identify a task a simple chain can't handle (e.g., "retry until answer passes a check") | A | CO6 |
| 31 | LangGraph core concepts: nodes, edges, state | Dem | Instructor demo: build a minimal 3-node LangGraph workflow, trace state as it flows through | A | CO6 |
| 32 | Building a stateful workflow + conditional branching in LangGraph | App | Lab: implement a draft → self-critique → revise loop with a conditional branch | Adv | CO6 |
| 33 | Agents & tool-calling: the ReAct pattern | Dem | Instructor demo: ReAct-style agent reasoning trace (thought → action → observation) on a sample task | Adv | CO6 |
| 34 | Hands-on: build an agent with LangGraph + Ollama + a custom tool | App | Lab: build an agent that calls a custom tool (e.g., calculator, file lookup) within a LangGraph flow | Adv | CO6 |
| 35 | Combining RAG + LangGraph: an agentic RAG assistant | App | Lab: extend Unit 3's RAG pipeline into a LangGraph agent that decides when to retrieve vs. answer directly | Adv | CO4–CO6 |
| 36 | Multimodal generative AI: text-to-image, text-to-audio, text-to-video (diffusion-based tools, many hosted on Hugging Face Spaces) | Dem | Live demo comparison of outputs from text-to-image tools with prompt-variation exercise; link back to Unit 1's diffusion theory and Unit 2's Hugging Face Hub session | A | CO1, CO2, CO6 |
| 37 | Responsible AI: bias, hallucination, deepfakes, copyright, misuse, cost/latency trade-offs | Int | Case discussion + role-play: stakeholders (developer, end-user, regulator) debate deploying a generative/agentic system | A | CO6 |
| 38 | **Capstone** — build & present a complete Gen AI application | App/Int | Final team presentation: end-to-end local app — Hugging Face model + Ollama runtime + LangChain + RAG + LangGraph, with eval results and a short note on responsible-use considerations | Both | CO1–CO6 |

---

### Notes
- **Unit 1 is intentionally demo-based, not lab-heavy** — the goal is conceptual fluency across the generative-model landscape (so the course earns its title), while the deep hands-on time is concentrated in Units 2–4 where a full working stack can actually be built in a semester.
- **Hugging Face's role (sessions 16–17):** positioned deliberately before Ollama — students first see *where* models/datasets actually come from and how to load one directly via `transformers`, then see Ollama as the easy local-runtime shortcut built on the same underlying model ecosystem. This also sets up `sentence-transformers` (from HF) as the natural embedding-model choice in Unit 3.
- **Session count is now 38** (up from 36) to fit Hugging Face in properly rather than cramming it into an existing slot — adjust unit weightage/contact hours accordingly if your scheme of instruction is fixed at 36 sessions; sessions 16 and 17 could be merged into one combined Hub-tour-plus-lab session if time is tight.
- **Embeddings (session 24):** Hugging Face `sentence-transformers` is suggested as the default; substitute only if lab hardware can't run it.
- **RAG evaluation (session 28):** RAGAS is one option; any faithfulness/relevance-style eval tool works — the key learning goal is that RAG outputs must be measured, not just eyeballed.
- **Session 36 deliberately loops back** to Unit 1's diffusion-model theory and Unit 2's Hugging Face session, so multimodal generation and the Hub aren't introduced as throwaway demos.
- **Capstone (session 38):** forces integration of theory (model landscape, architecture) and practice (build + evaluate) — a natural point for the CGPA-calibration "advanced ceiling" task if using the dual-level (floor/ceiling) evaluation scheme.