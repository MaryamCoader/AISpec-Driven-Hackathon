# Data Model: Chapter 1 Topic File

## Entity: Chapter1TopicFile

### Description
Represents an individual topic file (`.md`) within the `01-intro` directory in a Docusaurus project.

### Fields
-   **filename** (string): The name of the markdown file (e.g., `what-is-physical-ai.md`). Should be descriptive, lowercase, and URL-friendly.
-   **title** (string): The primary title of the topic within the file (e.g., "What is Physical AI?").
-   **content** (markdown): The complete, detailed, page-level content of the topic, adhering to the 800-1200 word count, including headings, text, code blocks, examples, explanations, and professional formatting.
-   **chapter_directory** (string): The fixed path to the parent chapter's directory (`ai-native-book/docs/01-intro/`).
-   **sidebar_label** (string, optional): The label that will appear in the Docusaurus sidebar navigation for this topic.

### Relationships
-   The `ai-native-book/docs/01-intro/` directory contains many **Chapter1TopicFiles**.
-   **Chapter1TopicFiles** are linked and ordered within the Docusaurus `sidebars.ts` configuration (likely via autogeneration).
