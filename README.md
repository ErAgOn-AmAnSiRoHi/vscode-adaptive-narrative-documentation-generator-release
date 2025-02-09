# vscode-adaptive-narrative-documentation-generator-release
VSCode extension to generate narrative documentation for codebases. This is the public version of my private repository to share the extension release publicly.

---

# Adaptive Narrative Documentation Generator

## Description

The Adaptive Narrative Documentation Generator is a Visual Studio Code extension that dynamically generates narrative documentation for any codebase opened in VSCode. It analyzes code in real-time, extracts structural information, and produces story-like documentation that explains the codebase's architecture, evolution, and design decisions.

## Features

- **Narrative Summary:** Generates a clear, natural language summary of the codebase.
- **Interactive Diagrams:** Visualizes module dependencies and relationships using interactive diagrams (D3.js).
- **Timeline View:** Illustrates code evolution with a timeline or history view.
- **Embedded Explanations:** Provides explanations for key components, comments on code smells, and refactoring recommendations.
- **Real-time Updates:** Automatically updates documentation in a VSCode side panel as you edit files.
- **OpenRouter API Integration:** Leverages DeepSeek: R1 Distill Llama 70B via OpenRouter for natural language generation tasks.
- **Configurable Settings:** Allows customization of update frequency, diagram styles, and API key via VSCode settings.

## Installation

1.  **Prerequisites:**

    - [Visual Studio Code](https://code.visualstudio.com/) (version ^1.85.0 or higher)
    - [Node.js](https://nodejs.org/) and npm (for building and packaging the extension)
    - An API key from [OpenRouter](https://openrouter.ai/) (for LLM features)

2.  **Install from VSCode Marketplace (Coming Soon):**

    - Once published, you will be able to install directly from the VSCode Marketplace.

3.  **Manual Installation (for development):**
    - Clone this repository to your local machine.
    - Open VSCode and go to the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X`).
    - Click on the "..." menu in the Extensions view and select "Install from VSIX...".
    - Choose the `adaptive-narrative-documentation-generator-x.x.x.vsix` file from the packaged extension (after running `vsce package`).

## Usage

1.  **Open a Project:** Open any codebase in VSCode.
2.  **Generate Documentation:**
    - Open the Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`).
    - Type and select `Generate Narrative Documentation`.
    - Alternatively, the Narrative Documentation panel should activate automatically upon opening a workspace.
3.  **View Documentation:** The Narrative Documentation panel will appear in the VSCode sidebar, displaying the generated documentation.
4.  **Real-time Updates:** As you edit files in your workspace, the documentation will update automatically (based on the configured update frequency).

## Configuration

You can configure the extension settings in VSCode:

1.  Go to `File` > `Preferences` > `Settings` (or `Code` > `Settings` on macOS).
2.  Search for "Adaptive Narrative Documentation Generator" in the settings panel.
3.  Configure the following settings:
    - **OpenRouter API Key:** Enter your API key from OpenRouter.
    - **Update Frequency:** Set the frequency (in milliseconds) for automatic documentation updates.
    - **Diagram Style:** Choose the style for the diagrams (default, dark, or light).


## License

[MIT License](https://github.com/ErAgOn-AmAnSiRoHi/vscode-adaptive-narrative-documentation-generator/blob/main/LICENSE)

## Repository

[https://github.com/ErAgOn-AmAnSiRoHi/vscode-adaptive-narrative-documentation-generator](https://github.com/ErAgOn-AmAnSiRoHi/vscode-adaptive-narrative-documentation-generator)

---
