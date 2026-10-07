# LVMH: A Meta-Optimization Harness for Long-Video Agent Memory

[Read the preprint (PDF)](LVMH_preprint.pdf) · September 15, 2026

## Abstract

Long-video agents must map hours or days of multimodal evidence into a bounded context while respecting token and latency budgets, making memory design a context-management challenge.
Existing memory systems largely rely on hand-designed policies, leaving open how to jointly optimize memory design for performance and efficiency.
We propose Long Video Meta-memory Harness (LVMH), an automated multi-agent framework that formulates memory-policy development as multi-objective code search around a fixed answer model.
To guard against self-certification and development-set overfitting, LVMH separates implementation from independent review and enforces protected observation boundaries.
Persistent meta-memory records past proposals, traces, costs, and failures to guide subsequent policy revisions.
Through this harness, we discover Self-Evolving Evidence Memory (SEEM), a “text-first, vision-second” policy that answers from compact structured event memory and evidence specialists, consulting localized frames through a selective visual gate.
The policy evolved on EgoLifeQA generalizes to unseen benchmarks, outperforming Meta-Harness on both Ego-R1 Bench and Video-MME (L) with GPT-5 mini.
Across the three benchmarks, SEEM with GPT-5 achieves 65.7% average accuracy, surpassing the previous state of the art by 7.7 percentage points with approximately 32× lower average evaluation token use and 91× shorter average response time.
