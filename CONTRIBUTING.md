# Contributing to Workflow Engines Explorer

Thank you for your interest in contributing to the Workflow Engines Explorer! Community collaboration is essential to keep this project up to date and comprehensive.

## Ways to Contribute

### 🐛 Reporting Issues

Found something wrong? We'd love to hear about it!

- **[Create an issue](https://github.com/iocanel/workflow-engines/issues)** to report:
  - Missing workflow engines
  - Incorrect categorizations or descriptions
  - Broken links or outdated information
  - UI/UX improvements
  - New category suggestions

### 🚀 Adding New Workflow Engines

To add a new workflow engine:

1. **Fork the repository**
2. **Edit the `workflow-engines.json` file**
3. **Add your engine** following this structure:

```javascript
{
  "name": "Engine Name",
  "url": "https://engine-website.com",
  "icon": "icons/engine.png",
  "description": "Brief description highlighting key characteristics and use cases.",
  "tags": ["Category1", "Category2", "Category3", "Additional", "Traits"]
}
```

4. **Choose appropriate tags** from existing categories:
   - **Ontological**: Event, Process, Data, Integration, Automation
   - **Architectural**: Log, State-machine, DAG, Code flows
   - **Teleological**: Microservice orchestration, Business process automation, Data Pipelines, Integration, CI/CD, Machine Learning
   - **Structural**: Code-as-workflow, DSL, Graph (DAG), YAML, JSON, Visual
   - **Licensing**: Free, OpenSource, Source-Available, Proprietary
   - **Operational**: Managed Service, Self Hosted, Library
   - **Other**: Persistent, Replayable, Ephemeral, Event-driven, Cloud-native, Kubernetes-native, Container, Serverless

5. **Add an icon** (optional):
   - Place a 24x24px icon in the `icons/` directory
   - Use PNG format with transparent background
   - Name it consistently (e.g., `engine-name.png`)

6. **Submit a pull request** with a clear description

### 🏷️ Updating Existing Engines

To update existing engines:

1. **Fork the repository**
2. **Locate the engine** in the `workflow-engines.json` file
3. **Update the relevant fields**:
   - Fix incorrect descriptions
   - Add missing tags
   - Update URLs or icons
   - Correct categorizations
4. **Submit a pull request** explaining the changes

### 📂 Adding New Categories

To propose new category dimensions:

1. **Open an issue** first to discuss the new category
2. **Provide rationale** for why it's needed
3. **Suggest category values** and how existing engines would be classified
4. **If approved**, update:
   - The `categorizations` object
   - The `facetConfig` array
   - Engine tags as needed

## Guidelines

### Categorization Principles

- **Ontological**: What kind of thing is the engine fundamentally managing?
- **Architectural**: What are the core technical/architectural elements?
- **Teleological**: What is the primary purpose and business goal?
- **Structural**: How are workflows defined and represented?
- **Operational**: How is the engine deployed, run, and maintained?
- **Licensing**: What are the legal/commercial terms?

### Quality Standards

- **Accurate descriptions**: Focus on key differentiators and use cases
- **Consistent categorization**: Use existing tags when possible
- **Current information**: Ensure URLs and details are up to date
- **Neutral tone**: Avoid marketing language or bias
- **Proper formatting**: Follow the existing code style

### Tag Selection

- **Be precise**: Choose tags that accurately reflect the engine's nature
- **Be consistent**: Use existing tags rather than creating synonyms
- **Be complete**: Include all relevant dimensions
- **Avoid redundancy**: Don't duplicate information across tags

## Technical Details

### File Structure

```
workflow-engines/
├── index.html              # Main application file
├── workflow-engines.json   # Workflow engine data (preferred for editing)
├── icons/                 # Engine icons (24x24px PNG)
├── README.md              # Project documentation
├── CONTRIBUTING.md        # This file
└── CLAUDE.md             # Development guidelines
```

### Data Location

**Single source of truth**: All workflow engine data is stored in `workflow-engines.json`
**Categories**: Defined in the `categorizations` object within `index.html`
**HTTP Server Required**: The application loads data from the JSON file and requires an HTTP server to run

### Testing Changes

1. **Run locally**: Use `python3 -m http.server 8000`
2. **Test filtering**: Verify your engine appears in correct categories
3. **Check search**: Ensure the engine is searchable by name
4. **Validate links**: Confirm URLs work and open correctly
5. **Review mobile**: Test on mobile devices for responsiveness

## Pull Request Process

1. **Fork** the repository
2. **Create a feature branch**: `git checkout -b add-engine-name`
3. **Make your changes** and test them locally
4. **Commit with clear messages**: `git commit -m "Add [Engine Name] workflow engine"`
5. **Push to your fork**: `git push origin add-engine-name`
6. **Create a pull request** with:
   - Clear title describing the change
   - Description of what was added/changed
   - Why the change is valuable
   - Screenshots if UI changes are involved

## Code of Conduct

- **Be respectful**: Treat all contributors with respect
- **Be constructive**: Provide helpful feedback and suggestions
- **Be collaborative**: Work together to improve the project
- **Be patient**: Allow time for review and discussion

## Questions?

- **Open an issue** for questions about contributing
- **Check existing issues** before creating new ones
- **Be specific** in your questions and requests

## Recognition

All contributors will be recognized in the project. Significant contributions may be highlighted in release notes.

Thank you for helping make workflow engine discovery better for everyone! 🙏