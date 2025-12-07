# Research: Chapter Content Generation

**Purpose**: To resolve open questions from the technical context and define the tools and processes for creating the textbook chapter.

## 1. Diagram Generation Tools

-   **Decision**: Use Mermaid.js for architectural diagrams and flowcharts. For more complex illustrations or screenshots, use static PNG/SVG files created with an external tool (e.g., Excalidraw, Inkscape).
-   **Rationale**: Mermaid.js is supported by Docusaurus and allows diagrams to be managed as code, making them easy to version and update. Static images provide flexibility for complex visuals that are difficult to represent in code. This hybrid approach offers the best of both worlds.
-   **Alternatives considered**:
    -   **Static images only**: Harder to maintain and update consistently.
    -   **Exclusively code-based diagrams**: Can be limiting for highly detailed or custom illustrations.

## 2. Code Sample Integration

-   **Decision**: Code samples will be maintained as complete, runnable projects in the `src/code-examples/` directory. Snippets of these files will be embedded into the Markdown files using the Docusaurus `code-block` component with line highlighting.
-   **Rationale**: This ensures that all code presented to the learner is verifiable and tested. Embedding snippets from source files avoids code duplication and ensures the documentation is always in sync with the working examples.
-   **Alternatives considered**:
    -   **Inline code blocks only**: Prone to typos and becoming outdated. Not easily testable.

## 3. Content Generation Workflow

-   **Decision**: The content will be generated in phases:
    1.  **Outline**: Create the file structure and headings for each section.
    2.  **Drafting**: Write the prose for each section, focusing on clarity and technical accuracy.
    3.  **Code Integration**: Write and test the code examples, then embed them.
    4.  **Diagram Creation**: Create and embed the diagrams.
    5.  **Review & Refinement**: Peer review for quality, clarity, and technical accuracy.
-   **Rationale**: A phased approach ensures a structured and methodical process, improving the quality of the final output.
-   **Alternatives considered**:
    -   **Ad-hoc writing**: Lacks structure and can lead to inconsistent quality.
