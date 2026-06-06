# Contribution #1: Add Wan2.2-Fun-A14B-InP Model Support to vLLM-omni

**Contribution Number:** 1  
**Student:** jindaxz (Jinda Zhang)  
**Issue:** [vLLM-omni #1809](https://github.com/vllm-project/vllm-omni/issues/1809)  
**Status:** Phase I - In Progress

---

## Why I Chose This Issue

I'm interested in contributing to vLLM-omni to understand how modern LLM inference engines support different model architectures. This is my first open-source contribution as part of the CodePath AI301 program, and I chose this issue because:

1. **Good First Issue:** Labeled as beginner-friendly with clear scope
2. **Learning Goal:** I want to understand how vLLM integrates new models and how model-specific configurations are handled
3. **Practical Impact:** Adding support for new models is valuable for the community and will help me learn about model architecture variations (the Wan2.2-Fun model is an Alibaba model with specific architectural features)

---

## Understanding the Issue

### Problem Description

vLLM-omni currently doesn't support the Wan2.2-Fun-A14B-InP model from Alibaba. Users who want to use this model architecture with vLLM-omni can't because there's no model configuration or integration for it.

### Expected Behavior

Users should be able to load and run the Wan2.2-Fun-A14B-InP model using vLLM-omni, with proper architecture detection and configuration for the model's specific attention mechanisms and layer structure.

### Current Behavior

Attempting to use the Wan2.2-Fun-A14B-InP model with vLLM-omni fails because:
- The model is not registered in the supported models list
- Model-specific configurations aren't defined
- Architecture parameters aren't configured

### Affected Components

- Model registry/configuration system in vLLM-omni
- Model architecture detection code
- Model-specific attention and layer implementations (if needed)

---

## Reproduction Process

### Environment Setup

**Phase 1 Goal:** Clone vLLM-omni, set up development environment, and explore codebase structure.

- [ ] Clone vLLM-omni repository
- [ ] Review model registry structure
- [ ] Identify where model configurations are stored
- [ ] Understand the architecture detection mechanism

### Steps to Reproduce

1. Clone the vLLM-omni repository
2. Attempt to load the Wan2.2-Fun-A14B-InP model 
3. Observe error that model is not supported

### Reproduction Evidence

- **Status:** Phase 1 - Setting up local environment this week
- **Model Link:** https://huggingface.co/alibaba-pai/Wan2.2-Fun-A14B-InP
- **My findings:** (To be updated as I explore the codebase)

---

## Solution Approach

### Analysis

**Phase 1 Focus:** Understanding the codebase structure and how model support is implemented.

The issue requires adding the Wan2.2-Fun-A14B-InP model to vLLM-omni. This involves:
1. Identifying how models are registered in the system
2. Understanding model configuration requirements
3. Determining if Wan2.2-Fun needs custom architecture implementations or if it can use existing components

### Proposed Solution

**Phase 1 Deliverable:** A detailed plan for adding model support, including:
1. Locating the model registry and configuration system
2. Analyzing existing similar model implementations
3. Identifying required changes to support Wan2.2-Fun
4. Creating implementation roadmap for Phase 2

### Implementation Plan

Using SPARC framework (Specification → Architecture → Refinement → Completion):

**Understand:** Add Wan2.2-Fun-A14B-InP model support to vLLM-omni so users can load and run this model.

**Match:** Analyze how existing models are integrated (find similar Alibaba/transformer models)

**Plan (Phase 1):**
1. Clone repo and explore model registry structure
2. Find and analyze existing model implementations
3. Study the Wan2.2-Fun model architecture
4. Document where changes are needed

**Implement:** (Phase 2) Will be implemented based on Phase 1 findings

**Review:** (Phase 2) Follow vLLM contribution guidelines

**Evaluate:** (Phase 2) Test with actual Wan2.2-Fun model

---

## Testing Strategy

### Phase 1 Checklist

- [ ] Model loads without errors
- [ ] Model initialization works correctly
- [ ] Basic inference passes

### Phase 2 Testing (Planned)

- [ ] Unit tests for model configuration
- [ ] Integration tests with vLLM inference pipeline
- [ ] Performance benchmarks
- [ ] Compatibility tests with different batch sizes

---

## Implementation Notes

### Phase 1 Progress (Week of June 5, 2026)

**Objective:** Understand vLLM-omni codebase and create implementation plan

**Tasks:**
- [ ] Clone vLLM-omni repository and explore structure
- [ ] Locate model registry and configuration files
- [ ] Review similar model implementations (e.g., other Alibaba models)
- [ ] Study Wan2.2-Fun-A14B-InP architecture from HuggingFace
- [ ] Document findings and create detailed implementation plan for Phase 2

**Challenges:** (To be updated as discovered)

**Decisions:** (To be updated as work progresses)

### Code Changes

- **Status:** Phase 1 - Analysis phase, no code changes yet
- **Repository:** [vLLM-omni](https://github.com/vllm-project/vllm-omni)
- **Branch:** (To be created in Phase 2)

---

## Pull Request

**Status:** Phase 1 - Not yet submitted

**Timeline:**
- Phase 1 (Week 1): Research & Planning
- Phase 2 (Weeks 2-3): Implementation
- Phase 3 (Week 4): Testing & Iteration
- Phase 4 (Week 5): PR Submission & Review

**PR Link:** (To be created in Phase 3)

**PR Description:** (To be drafted in Phase 2)

---

## Learnings & Reflections

### Phase 1 Learnings (To be updated)

**Technical Skills:**
- (In progress) Understanding how LLM inference engines manage model support
- (In progress) Exploring model registry patterns

**Process Learnings:**
- (To be documented after Phase 1)

### Challenges & Solutions

- (To be documented as they arise)

---

## Resources Used

- [Wan2.2-Fun Model on HuggingFace](https://huggingface.co/alibaba-pai/Wan2.2-Fun-A14B-InP)
- [vLLM-omni Repository](https://github.com/vllm-project/vllm-omni)
- [vLLM Documentation](https://docs.vllm.ai/)
- [vLLM Contributing Guide](https://github.com/vllm-project/vllm/blob/main/CONTRIBUTING.md)
- CodePath AI301 Program Resources
