# TreeTangler

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/dkbiocode/TreeTangler)

**Published in PLOS Pathogens (2021)** | Interactive D3.js Phylogenetic Visualization Tool

> 🔬 **Note**: This is a research tool originally developed in 2017-2021. It contains some deprecated dependencies but remains functional for demonstration and educational purposes. A modernized version is planned.

## 🚀 Try It Now - No Installation Required!

Click the Codespaces badge above to launch an interactive demo in your browser:

1. Wait ~30 seconds for the environment to build
2. Once ready, the terminal will show: `Server running on port 8000`
3. Click "Open in Browser" when prompted
4. Explore phylogenetic trees interactively!

## What is TreeTangler?

TreeTangler is an interactive web-based tool for visualizing and comparing phylogenetic trees (cophylogenies). It was developed to simplify the analysis of host-parasite evolutionary relationships.

**Key Features:**
- Interactive D3.js-based visualization
- Real-time tree manipulation
- Custom binary tree algorithms
- Drag-and-drop interface for tree comparison
- Published research tool with peer-reviewed applications

## Local Installation

For local development or deployment:
```bash
git clone https://github.com/dkbiocode/TreeTangler.git
cd TreeTangler
npm install
npm start
# Navigate to http://localhost:8000
```

## Technology Stack

- **Frontend**: D3.js (v5), JavaScript ES6+
- **Backend**: Node.js, Express
- **Build System**: Grunt, Browserify
- **Module System**: Custom tree manipulation library (cophy-treetools)

## Usage

1. Load your Newick format phylogenetic trees
2. Visualize tree structures side-by-side
3. Explore relationships through interactive manipulation
4. Export visualizations for publications

## Citation

If you use TreeTangler in your research, please cite:

Kapuscinski ML, et al. (2021). Genomic characterization of 99 viruses from the bunyavirus families. *PLOS Pathogens*, 17(3):e1009315. [DOI: 10.1371/journal.ppat.1009315](https://doi.org/10.1371/journal.ppat.1009315)

## Development

### Building from Source
```bash
npm install        # Install dependencies
npm run build      # Build bundles
npm start          # Start server
```

### Project Structure
```
TreeTangler/
├── app.js              # Main server file
├── lib/                # Core library code
├── public/             # Static assets and bundles
├── assets/             # Example data files
└── test/               # Test suite
```

## Known Issues & Limitations

⚠️ **Security Notice**: This project uses older dependencies with known vulnerabilities. These are primarily in development dependencies (documentation generation) and do not affect the core visualization functionality. Use in production environments is not recommended without dependency updates.

The main vulnerabilities are:
- d3@5.8.2 (ReDoS in d3-color)
- esdoc and related documentation tools
- Various deprecated npm packages

**For portfolio demonstration purposes**, the tool remains functional and secure when used as intended (local visualization tool).

## Future Plans

- [ ] Update to D3.js v7+
- [ ] Replace Grunt with modern build tools (Vite/Webpack)
- [ ] Add TypeScript support
- [ ] Comprehensive test coverage
- [ ] Update all dependencies to current versions

## About

Developed by David King at Colorado State University as part of collaborative research on viral phylogenomics. This tool was created to address specific needs in cophylogenetic analysis and has been used in peer-reviewed publications.

**Original Repository**: [meekrob/TreeTangler](https://github.com/meekrob/TreeTangler)  
**Portfolio Version**: Adapted for demonstration and educational purposes

## License

MIT License - See [LICENSE](LICENSE) for details

## Related Projects

- [cophy-treetools](https://github.com/meekrob/cophy-treetools) - Command-line phylogenetic utilities
- [More bioinformatics tools](https://github.com/dkbiocode) - Additional visualization and analysis tools

---

**Questions or Issues?** Please open an issue or contact david.king@colostate.edu