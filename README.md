# Hi, I'm Shubham Sarvankar,

I build stuff. 

## Projects

These are some selected projects that I've worked on recently.

- **[Litmus](https://github.com/ShubhamSarvankar/litmus):** S3-compatible object store built for correctness. AWS CLI and boto3 work unmodified. A two-tier chaos suite proves durability invariants hold across SIGKILL and injected OSErrors. 115/325 ceph/s3-tests pass; every failure documented.
- **[ITCH 5.0 Parser](https://github.com/ShubhamSarvankar/itch-parser):** C++ limit order book reconstruction for NASDAQ TotalView-ITCH 5.0. Lock-free snapshot handoff via `atomic<shared_ptr>`, fixed-point price arithmetic throughout, 57M msg/s parse throughput. Validated against a real 7.7 GB production capture.
- **[Botnet C2 Detection](https://github.com/ShubhamSarvankar/botnet-graph-analysis)**: graph topology classifier over CTU-13 (13 captures, 7 botnet families). Leave-one-family-out cross-validation with pre-registered thresholds. Donbot achieves 0.872 PR-AUC on an unseen family; the `cc_dst_only` collapse to 0.001 is itself a documented finding.
- **[Storm](https://github.com/ShubhamSarvankar/storm)**: real-time messaging platform in TypeScript. AES-256-GCM encryption, single-use JWT refresh tokens with replay detection, 112 tests against real MongoDB and Redis.
- **[Streaming Observability Platform](https://github.com/ShubhamSarvankar/streaming-observability-platform):** End-to-end log analytics pipeline: NASA HTTP logs (1.9M lines) replay through Kafka → Spark Structured Streaming → Cassandra, served by a layered Spring Boot API. A LangGraph agent answers questions in plain English but never writes a query — it selects from five typed tools, so the LLM can't reach the database directly. Swappable provider behind one interface, validated on both claude-haiku-4-5 and local qwen2.5:7b (GPU).
- **[MedGuard](https://github.com/ShubhamSarvankar/medguard):** Cross-platform medical records system with end-to-end encryption and HIPAA-aware audit logging. Mandatory PHI de-identification runs as a Firestore trigger (not optional middleware) using a two-stage Claude pipeline: entity extraction → deterministic placeholder substitution. Per-record AES-256-GCM keys wrapped via envelope encryption; Android local storage requires biometric auth. 355 tests across Cloud Functions, React web, and Android (Kotlin + Compose).
- **[PA Legal Case Search](https://github.com/ShubhamSarvankar/PALawSearch):** Multi-method retrieval system over 200k+ Pennsylvania legal cases. BM25 baseline, Legal-BERT dual-encoder semantic search, and cross-encoder reranking (BAAI/bge-reranker-large, 560M params). RAG Q&A layer fuses BM25 and dense results via Reciprocal Rank Fusion, then streams answers through Qwen3:8b with case citations. Dense+rerank drops from ~3s first query to ~10ms cached.
- **[Flagged Unfairly](https://github.com/ShubhamSarvankar/flagged-unfairly):** Fairness audit of Detoxify's `unbiased` toxicity classifier on the Civil Comments dataset (21,293 identity-annotated comments). Black-identity comments are false-positived at 3.02× the baseline rate; counterfactual term-swapping confirms the model reacts to the identity term itself, not surrounding content. Intersectional analysis finds black × jewish FPR at 5.88×. Per-group threshold optimization cuts maximum FPR disparity from 3.07× to 1.20× at a cost of −1.1% F1.
- **[Join Society](https://github.com/ShubhamSarvankar/JoinSociety):** Full-stack e-commerce platform on the MERN stack. Stripe checkout with coupon support, Cloudinary image uploads, Redis caching, JWT auth via HTTP-only cookies, and an admin dashboard with live analytics (Recharts). Covers the complete user journey from browsing to order history.

---

## Let’s Connect

- 📩 [Email](mailto:shubham.sarvankar@pitt.edu)
- 💼 [LinkedIn](https://www.linkedin.com/in/shubhamsarvankar/)
