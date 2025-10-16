# Markdown to HTML Converter

## Summary

This static web application converts Markdown input from a file named `input.md` into HTML using the `marked` library. It then renders this content in a designated HTML element with syntax highlighting for code blocks provided by `highlight.js`.

## Setup

Follow these steps to deploy the application on GitHub Pages:

1. **Fork the Repository**: Start by forking the repository to your GitHub account.
2. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/repository-name.git
   ```
3. **Navigate to the Project Directory**:
   ```bash
   cd repository-name
   ```
4. **Add `input.md`**: Place your `input.md` file in the root directory of the project.
5. **Commit and Push**:
   ```bash
   git add input.md
   git commit -m "Add input.md"
   git push origin main
   ```
6. **Enable GitHub Pages**:
   - Go to your repository on GitHub.
   - Navigate to Settings > Pages.
   - Under "Source", select `main` branch and `/root` directory.
   - Click "Save".

## Usage

- **Accessing the Page**: Visit the GitHub Pages URL provided in the repository's settings.
- **Configuration Options**: This application does not require any additional configuration or query parameters.
- **Key Features**:
  - Automatic Markdown conversion to HTML.
  - Real-time syntax highlighting for code blocks within Markdown content.

## Code Explanation

- **HTML/JS Implementation**: The application uses a simple HTML file with embedded JavaScript to fetch `input.md` and convert it to HTML. The main logic loads the Markdown from the file, uses `marked` for parsing, and injects the converted HTML into the `#markdown-output` div.
- **Key Libraries Used**:
  - `marked`: A low-level Markdown compiler to parse and convert Markdown to HTML.
  - `highlight.js`: A library for syntax highlighting of code blocks.
- **Important Logic**:
  - Fetching of `input.md` and handling file reading is done with `fetch` API.
  - Once fetched, the Markdown string is processed by `marked` and inserted into the page.
  - All `<code>` elements within the converted HTML are highlighted using `highlight.js`.

## License

This project is licensed under the MIT License.