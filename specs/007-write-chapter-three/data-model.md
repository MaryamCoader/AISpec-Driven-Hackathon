# Data Model: Chapter 3 Topic File

## Entity: Chapter3TopicFile

### Description
Represents an individual topic file (`.md`) within the `03-chapter-three` directory in a Docusaurus project.

### Fields
-   **filename** (string): The name of the markdown file (e.g., `rl-for-robot-behaviors.md`). Should be descriptive, lowercase, and URL-friendly.
-   **title** (string): The primary title of the topic within the file (e.g., "Reinforcement Learning for Complex Robot Behaviors").
-   **content** (markdown): The complete, detailed, page-level content of the topic, adhering to the 800-1200 word count, including headings, text, code blocks, examples, explanations, and professional formatting.
-   **chapter_directory** (string): The fixed path to the parent chapter's directory (`ai-native-book/docs/03-chapter-three/`).
-   **sidebar_label** (string, optional): The label that will appear in the Docusaurus sidebar navigation for this topic.

### Relationships
-   The `ai-native-book/docs/03-chapter-three/` directory contains many **Chapter3TopicFiles**.
-   **Chapter3TopicFiles** are linked and ordered within the Docusaurus `sidebars.ts` configuration (likely via autogeneration).
