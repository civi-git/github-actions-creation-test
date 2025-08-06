# Formal Definition and Implementation of Reproducibility Tenets for Computational Workflows

**Citation:** Pritchard, N., et al. (2024). Formal Definition and Implementation of Reproducibility Tenets for Computational Workflows. arXiv:2406.01146.

**URL:** https://arxiv.org/abs/2406.01146

## CS197 Analysis Structure

### 1. Problem
**What problem does it solve? Why does it matter?**

The reproducibility crisis in scientific computing stems from:
- Lack of formal definitions for what constitutes reproducible computational workflows
- Inability to automatically verify scientific quality in workflow executions
- Difficulty in comparing workflow executions to identify discrepancies
- Challenge of providing formal guarantees about workflow reproducibility

This matters because reproducibility is fundamental to scientific validity, and large-scale projects like the Square Kilometre Array (SKA) require massive collaboration with guaranteed reproducibility.

### 2. Prior Assumptions
**What assumption did earlier work assume? Why was it inadequate?**

Prior approaches assumed:
- Informal definitions of reproducibility were sufficient
- Manual verification of workflow reproducibility was feasible
- Provenance tracking alone could ensure reproducibility
- Reproducibility could be achieved without formal mathematical frameworks

These assumptions were inadequate because:
- They provided no systematic way to verify reproducibility
- They couldn't scale to large collaborative scientific projects
- They offered no formal guarantees about workflow quality
- They couldn't automatically detect subtle but important workflow differences

### 3. Insight
**What's the novel contribution?**

The key insight is to create a **formal mathematical framework** that:
- Extends five well-known reproducibility concepts into **seven well-defined tenets**
- Provides a **scale and system-agnostic** computational workflow model
- Uses **cryptographic primitives** to generate workflow execution signatures in amortized constant time
- Enables **automatic formal verification** of scientific quality

### 4. Technical Approach
**How is it implemented?**

The framework consists of:
1. **Formal workflow model** - mathematical definitions of computational workflows
2. **Seven reproducibility tenets** - formal extensions of existing concepts
3. **Cryptographic workflow signatures** - using hash functions and merkle trees for efficient signature generation
4. **Provenance integration** - embedding specific provenance information into signatures
5. **Implementation in DALiuGE** - concrete realization in the SKA workflow management system

Technical details:
- Amortized constant time signature generation using cryptographic primitives
- Formal UML specification for workflow models
- Integration with existing workflow management systems

### 5. Evaluation
**How was it validated?**

Validation through:
- **Astronomical processing example** - filtering noisy signals with lowpass filters
- **CPU vs GPU comparison** - testing identical workflows on different hardware
- **Concrete implementation** in DALiuGE workflow management system
- **Formal verification** of reproducibility tenets in practice

The example demonstrates the framework can:
- Detect discrepancies between principally identical executions
- Automatically verify scientific quality
- Scale to real astronomical data processing tasks

### 6. Impact
**What are the implications? How will it change the field?**

This work enables:
- **Automated reproducibility verification** rather than manual checking
- **Formal guarantees** about workflow quality and reproducibility
- **Scalable reproducibility** for large collaborative scientific projects
- **Standardized definitions** that can be applied across different domains
- **Real-time quality assurance** during workflow execution

## Key Assumptions Challenged

**Literature-level bit flip:** The assumption that reproducibility is an informal concept that can only be verified manually. Instead, reproducibility can be formally defined and automatically verified using mathematical frameworks.

## Connection to GitHub Actions

This work provides the formal foundation for implementing reproducibility checks in GitHub Actions workflows, enabling automatic verification of scientific quality in CI/CD pipelines.