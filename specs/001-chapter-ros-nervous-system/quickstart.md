# Quickstart: Contributing to the Chapter

This guide provides instructions for setting up the environment and contributing to the textbook chapter.

## Prerequisites

-   Node.js (LTS version)
-   Yarn
-   A local clone of the repository.

## Setup

1.  **Install Dependencies**: From the root of the repository, run:
    ```bash
    yarn install
    ```

2.  **Start the Development Server**: To preview the Docusaurus site locally, run:
    ```bash
    yarn start
    ```
    The site will be available at `http://localhost:3000`.

## Content Workflow

1.  **Find the Files**: The content for this chapter is located in `docs/01-robotic-nervous-system/`.
2.  **Make Changes**: Edit the `.md` files according to the `data-model.md` structure.
3.  **Add Images**: Place new images in `static/img/01-ros-nervous-system/`.
4.  **Add Code Examples**: Add new code to `src/code-examples/01-ros-nervous-system/`.
5.  **Submit for Review**: Create a pull request with your changes.
