# Generative AI — Activities List

## Unit 1 — Foundations of Generative AI
1. Sort familiar AI tools (ChatGPT, image generators, spam filters) into generative/discriminative buckets
2. MLE walkthrough on a toy dataset; students verify by hand on a second dataset
3. Plot and interpret a 2D latent space of a small image dataset
4. Run a pretrained AE on sample images, inspect reconstructions at different bottleneck sizes
5. Instructor derives ELBO on the board; students annotate each term's meaning
6. "Forger vs. detective" role-play, followed by a demo of a pretrained GAN's outputs
7. Visual analogy activity: relate diffusion to progressively "un-blurring" noise, step by step
8. Structured debate: teams argue which model family best suits a given real-world scenario
9. Use free Hugging Face Spaces demos to generate samples from each model family; write a comparison report

## Unit 2 — Transformers, Hugging Face & Ollama
10. Demo an LSTM failing on a long-dependency sentence; discuss why
11. Manual attention-weight calculation on a short sentence, by hand
12. Visualize attention heatmaps from a pretrained model on sample text
13. Instructor builds the Transformer architecture diagram block-by-block, with Q&A
14. Compute positional encodings for a short sequence, compare with/without
15. Tokenize sample text with BPE, inspect resulting tokens/subwords
16. Guided tour of the Hugging Face Hub: find and compare model cards for two similar models
17. Run a text-generation/classification pipeline using a small HF model; inspect config, tokenizer, outputs
18. Install Ollama, pull a small model, run first prompt; discuss trade-offs vs. Hugging Face `transformers`
19. Same task attempted zero-shot vs. few-shot vs. system-prompt on Ollama; compare outputs
20. Team lab: design a prompt-engineering "playbook" for a chosen task, tested on Ollama

## Unit 3 — LangChain & RAG
21. Discussion: what breaks when building a multi-step LLM app with raw API calls only
22. Build a 2-step sequential chain (e.g., summarize → translate) using LangChain + Ollama
23. Add conversation memory to a chatbot; compare behavior with/without memory
24. Generate embeddings using a Hugging Face `sentence-transformers` model; compute/interpret similarity scores
25. Store document embeddings in Chroma/FAISS, run nearest-neighbor queries, inspect results
26. Connect a vector-store retriever to Ollama via LangChain; ask questions grounded in custom docs
27. Compare answer quality across different chunk sizes/overlaps on the same document set
28. Run a RAG-eval framework (e.g., RAGAS) on sample Q&A pairs; interpret metrics
29. Team lab: build a RAG assistant over a custom document set and report its eval scores

## Unit 4 — LangGraph, Multimodal & Responsible AI
30. Discussion: identify a task a simple chain can't handle (e.g., "retry until answer passes a check")
31. Build a minimal 3-node LangGraph workflow, trace state as it flows through
32. Implement a draft → self-critique → revise loop with a conditional branch
33. Trace a ReAct-style agent's reasoning (thought → action → observation) on a sample task
34. Build an agent that calls a custom tool (e.g., calculator, file lookup) within a LangGraph flow
35. Extend the Unit 3 RAG pipeline into a LangGraph agent that decides when to retrieve vs. answer directly
36. Live demo comparison of text-to-image tool outputs with prompt-variation exercise
37. Case discussion + role-play: stakeholders debate deploying a generative/agentic system
38. Final team presentation: end-to-end app (HF model + Ollama + LangChain + RAG + LangGraph) with eval results