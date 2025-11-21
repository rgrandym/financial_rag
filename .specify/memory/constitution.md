<!--
Sync Impact Report:
- Version change: Template → 1.0.0
- Added principles: Modular Code Architecture, Environment Management, Manual Testing Approach, Branch-Based Development, Scientific Report Generation
- Templates requiring updates: ✅ plan-template.md / ⚠ spec-template.md / ⚠ tasks-template.md / ⚠ command files
- Follow-up TODOs: None
-->

# Report Writing Agent Constitution

## Core Principles

### I. Modular Code Architecture

All code MUST be organized into small, focused modules with clear single responsibilities.
Classes and functions MUST NOT exceed 50 lines. Each module MUST perform one specific task with clear inputs and outputs. Complex operations MUST be decomposed into smaller, composable units.

**Rationale**: Maintains code readability, testability, and facilitates easier debugging and maintenance of the system components.

### II. Environment Management

Development MUST use the conda environment indicated on the plan.md file for the project. If new dependencies are not avaialable in conda,  use pip as fallback. All dependencies MUST be clearly documented.

**Rationale**: Ensures reproducible development environments for machine learning workflows while providing flexibility for different development setups.

### III. Manual Testing Approach

Code testing MUST be performed manually rather than writing automated test suites. Focus MUST be on functionality verification and manual validation of system behavior. Tests will be conducted through direct interaction with the system components.

**Rationale**: Prioritizes rapid development and functional verification over test automation, suitable for research and analysis workflows.

### IV. Branch-Based Development

All development work MUST be performed on feature branches. Merging to main branch requires explicit approval and request. No direct commits to main branch are permitted during development phases.

**Rationale**: Maintains main branch stability and enables controlled integration of features in the financial analysis system.

### V. Scientific Report Generation

Report writing MUST use Quarto for document generation. Reports MUST follow the structured format: Introduction (500 words), Goals and Objectives (100-200 words), Methods (300-500 words), Results (100-200 words per figure), Discussion (200 words), Conclusion (200 words), References. All claims MUST be properly referenced with placeholders for unavailable sources.

If requested, use visual capabilities for analysis and interpretation of charts and tables. After completion of first draft, carry out a critical review of the document. Make sure anlysis and conclusions are gounded. Confirm that references are real. If references are not available, use a place holder to indicate that a reference is needed in place. DO NOT invent results or references.

**Rationale**: Ensures professional, reproducible scientific documentation for financial analysis results and maintains academic standards.

## Technology Stack Requirements

**Environment**: Conda environment `rag-transformers` (primary), pip fallback
**Document Generation**: Quarto for all reports and documentation
**Development**: Python-based RAG system with transformer models
**Version Control**: Git with mandatory branch-based workflow
**Analysis**: Visual capabilities for chart and image interpretation from notebooks

## Development Workflow

**Branch Management**: All work on feature branches, merge to main only upon explicit request
**Code Organization**: Modular architecture with <50 line functions/classes
**Testing**: Manual verification and functional validation
**Documentation**: Concise summaries unless extensive detail is specifically requested
**Report Generation**: Structured scientific format with proper referencing
**Analysis**: Integration of visual interpretation capabilities for data analysis

## Governance

This constitution supersedes all other development practices. All code reviews and pull requests MUST verify compliance with modular architecture principles. Complexity that violates the 50-line limit MUST be justified and decomposed. Visual analysis capabilities MUST be leveraged for interpreting charts, graphs, and images in reports and notebooks.

**Version**: 1.0.0 | **Ratified**: 2025-11-16 | **Last Amended**: 2025-11-16
