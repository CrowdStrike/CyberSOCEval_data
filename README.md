# CyberSOCEval Benchmark Data

This repository contains data sources used for creating and evaluating the CyberSOCEval benchmark in the cybersecurity domain, a joint project between CrowdStrike and Meta.

## Overview

CyberSOCEval is a benchmark designed to evaluate large language models on cybersecurity knowledge and capabilities, with a focus on Security Operations Center (SOC) tasks. This repository houses the data sources used in the benchmark, provided with appropriate licensing and attribution to enable collaborative research and evaluation.

## Paper

The benchmark will be explained in the upcoming paper, "CyberSOCEval: Benchmarking LLMs Capabilities for Malware Analysis and Threat Intelligence Reasoning" by Lauren Deason*†, Adam Bali†, Ciprian Bejean‡, Diana Bolocan*‡, James Crnkovich*†, Ioana Croitoru*‡, Krishna Durai†, Chase Midler‡, Calin Miron‡, David Molnar*†, Brad Moon‡, Bruno Ostarcevic‡, Alberto Peltea‡, Matt Rosenberg‡, Catalin Sandu‡, Arthur Saputkin†, Sagar Shah*†, Daniel Stan‡, Ernest Szocs‡, Shengye Wan†, Spencer Whitman†, Sven Krasser‡, and Joshua Saxe*†.

\* Core Contributors\
† Meta\
‡ CrowdStrike

### Abstract

Today’s cyber defenders are overwhelmed by a deluge of security alerts, threat intelligence signals, and shifting business context, creating an urgent need for AI systems that can enhance operational security work. Despite the potential of Large Language Models (LLMs) to automate and scale Security Operations Center (SOC) operations, existing evaluations are incomplete in assessing the scenarios that matter most to real-world cyber defenders. This lack of informed evaluation has significant implications for both AI developers and those seeking to apply LLMs to SOC automation. Without a clear understanding of how LLMs perform in real-world security scenarios, AI system developers lack a north star to guide their development efforts, and users are left without a reliable way to select the most effective models. Furthermore, malicious actors have begun using AI to scale cyber attacks, emphasizing the need for open source benchmarks to drive adoption and community-driven improvement among defenders and AI model developers. 

To address this gap, we introduce CyberSOCEval, a new suite of open source benchmarks that are part of CyberSecEval 4. CyberSOCEval consists of benchmarks tailored to evaluate LLMs in two tasks: Malware Analysis and Threat Intelligence Reasoning, core defensive domains that have inadequate coverage in current security benchmarks.  Our evaluations reveal that larger, more modern LLMs tend to perform better, confirming the training scaling laws paradigm. We also find that reasoning models leveraging test time scaling do not achieve the boost they do in areas like coding and math, suggesting that these models have not been trained to reason about cybersecurity analysis, and pointing to a key opportunity for improvement.  Finally, we find that current LLMs are far from saturating our evaluations, demonstrating that CyberSOCEval presents a significant hill to climb for AI developers to improve AI cyber defense capabilities.

## Disclaimer

This dataset (e.g. scenarios) contains fictional business descriptions created for benchmarking purposes. Any similarities to real businesses, organizations, or individuals are purely coincidental and unintentional. The CyberSOCEval benchmark is designed to test cybersecurity knowledge and capabilities in a controlled environment and does not intend to represent, implicate, or make claims about any specific real-world entities or events.

## Repository Structure

```markdown
CyberSOCEval_data/
├── data/ # Raw data sources
│ ├── crowdstrike-reports/         # CrowdStrike reports (PDFs)
│ └── hybrid-analysis/             # Hybrid Analysis data (JSONs)
├── LICENSE-DATA.md                # Licensing information for all data sources
├── CITATION.md                    # Citation information
└── README.md                      # Main repository documentation
```
Each directory contains its own README.md and LICENSE.md with more detailed information.

## Licensing

This repository contains data from multiple sources, each with different licensing requirements. Please refer to the LICENSE.md files in the various subdirectories.

## Using the Benchmark

To use the CyberSOCEval benchmark:

1. **Data**: This repository provides the data sources used in the CyberSOCEval benchmark
2. **Code**: The implementation of the CyberSOCEval benchmark is part of the [Purple Llama repository](https://github.com/meta-llama/PurpleLlama)
3. **Documentation**: Refer to both repositories' documentation for complete usage instructions

## Citation

If you use code or data from this benchmark in your research, please cite as described in [CITATION.md](CITATION.md).
