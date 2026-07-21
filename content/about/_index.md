+++
date = "2016-11-05T21:05:33+05:30"
title = "About"
+++

I am interested in building LLM inference platform and runtime at production scale. In my spare time, I like to build softwares for my hobbies: Music, Movie, and Board Games.


## Technical Focus

- LLM serving with vLLM, PyTorch, VLM inference, continuous batching, chunked prefill, prefix caching, KV-cache management, tensor parallelism, and data parallelism
- Serving infrastructure with Kubernetes, multi-cluster orchestration, topology-aware node scheduling, self-healing automation, capacity planning, and auto-scaling
- Accelerator performance with AWS Trainium, Neuron, NKI kernel development, Neuron Profiler, and performance profiling
- Programming in Python, C/C++, Java, SQL, Ruby, and TypeScript

## Professional Experience

### Software Development Engineer II, Trainium Multimodal Serving

*AWS Annapurna Labs, Seattle, WA - Mar 2026 - Present*

- Extended the vLLM Neuron plugin from text-only serving to vision-language model serving on Trainium, including ViT encoder execution and vision-embedding injection into the text prefill graph.
- Built a vision-embedding cache to avoid repeated image encoder computation in workloads where KV prefix caching cannot cover repeated images.
- Designed hybrid model parallelism for VLM serving, using data parallelism across vision encoder executions and tensor parallelism for the text decoder.
- Profiled and optimized an NKI MLP kernel for Qwen3-VL on Trainium, fusing operations to reduce per-layer forward-pass latency.

### Software Development Engineer I -> II, Claude Serving Platform

*AWS Bedrock, Seattle, WA - Oct 2024 - Mar 2026*

- Onboarded Trn2 UltraServers for low-latency multi-node decoding, automating node provisioning from EC2 Capacity Blocks into shared warm pools across Kubernetes clusters.
- Led the design and delivery of a self-healing system with per-fault-type tolerance policies for large-scale inference fleets across GPUs and Trainium.
- Designed a centralized node-allocation service that assigns physically co-located nodes to inference StatefulSets across multiple Kubernetes clusters.
- Enabled topology- and accelerator-aware prefill/decode routing for disaggregated Claude serving by surfacing node topology and accelerator metadata through Kubernetes pod metadata.

### Software Development Engineer I, Elastic Load Balancing

*AWS Elastic Load Balancing, Seattle, WA - Sep 2023 - Oct 2024*

- Expanded ELB fleet capacity by enabling scale-up to larger EC2 instance types with priority-based scaling logic.
- Automated end-to-end benchmarking for ELB instance-type onboarding, reducing validation effort and accelerating rollout across commercial regions.

## Education

- M.S. Computer Science, University of Southern California, Los Angeles, CA
- B.S. Computer Science & Mathematics, Macalester College, St. Paul, MN

## Contact

- Email: [vanadiumzhang@gmail.com](mailto:vanadiumzhang@gmail.com)
- LinkedIn: [linkedin.com/in/fanzhangg](https://linkedin.com/in/fanzhangg)
- GitHub: [github.com/fanzhangg](https://github.com/fanzhangg)
