# A Framework for Supporting the Reproducibility of Computational Experiments

**Citation:** Costa, L., Barbosa, S., & Cunha, J. (2020). A Framework for Supporting the Reproducibility of Computational Experiments. arXiv:2503.07080.

**URL:** https://arxiv.org/html/2503.07080v2

## CS197 Analysis Structure

### 1. Problem
**What problem does it solve? Why does it matter?**

Computational reproducibility faces fundamental challenges:
- Variety of computational environments makes recreation difficult
- Challenging to recreate exact frameworks, code, dependencies, and configurations
- Researchers struggle to reproduce computational experiments across different systems
- Lack of systematic approach to package experiments for reproducibility

This matters because computational work is integral to most scientific domains, and irreproducible computational results undermine scientific validity across disciplines.

### 2. Prior Assumptions
**What assumption did earlier work assume? Why was it inadequate?**

Prior approaches assumed:
- Providing source code and data is sufficient for reproducibility
- Computational environments can be easily recreated manually
- Documentation of dependencies and configurations is complete and accurate
- Researchers have the expertise to recreate computational environments

These assumptions were inadequate because:
- They underestimated the complexity of computational environment recreation
- They ignored the diversity of computational platforms and configurations
- They assumed perfect documentation, which rarely exists in practice
- They placed too much burden on reproducing researchers

### 3. Insight
**What's the novel contribution?**

The key insight is to create a **comprehensive framework (SciRep)** that:
- **Systematically packages everything** necessary for experiment reproduction
- **Defines complete experimental configurations** including code, data, languages, dependencies, databases, and execution commands
- **Creates reproducibility capsules** that are completely self-contained
- **Works across multiple scientific domains** from medicine to computer science

### 4. Technical Approach
**How is it implemented?**

**SciRep framework** provides:
- **Configuration system** - defines all aspects of computational experiments
- **Execution environment** - ensures consistent execution across systems
- **Packaging system** - creates complete reproducibility packages
- **Cross-domain support** - works for multiple scientific fields
- **Automated execution** - runs experiments consistently producing identical results

Technical features:
- Complete environment specification
- Dependency management
- Database configuration support
- Command execution automation
- Platform-agnostic packaging

### 5. Evaluation
**How was it validated?**

Comprehensive evaluation:
- **Comparison with 3 state-of-the-art tools**
- **18 experiments from published scientific articles**
- **Success rate measurement**: SciRep achieved 89% (16/18) success vs competitors' 61%
- **Result verification**: 100% of executed experiments produced original results
- **Cross-domain validation**: experiments from medicine to computer science

### 6. Impact
**What are the implications? How will it change the field?**

This framework enables:
- **Systematic reproducibility** across scientific domains
- **Higher success rates** in reproduction attempts
- **Complete experimental packaging** reducing reproduction barriers
- **Cross-platform compatibility** enabling broader reproduction
- **Standardized reproducibility practices** across scientific fields

## Key Assumptions Challenged

**Literature-level bit flip:** The assumption that reproducibility requires domain-specific solutions. Instead, a general framework can systematically support reproducibility across diverse scientific domains by focusing on complete experimental packaging.

## Connection to GitHub Actions

SciRep provides a model for how GitHub Actions workflows can systematically package and execute reproducible computational experiments by ensuring complete environment and dependency specification.