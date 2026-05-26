# Shuo - Professional Local Voice Input Method

**[中文文档](./README.zh-CN.md)**

A professional, local-first voice input method for macOS and Windows. No vendor lock-in, core capabilities run locally. Privacy-friendly.

## Features

- **Local Voice Recognition** - Voice data never leaves your device
- **Custom AI Providers** - Supports 10+ AI providers, freely configurable
- **Auto-structuring** - Automatic text formatting and paragraph organization
- **Colloquial Filtering** - Smart filtering of filler words and repetitions
- **Privacy First** - Zero cloud data collection, API keys stored locally
- **Professionally Crafted** - Community-driven, auditable code

## Tech Stack

- **Core**: Rust
- **ASR Engine**: Sherpa ONNX
- **Frontend**: Astro, Tailwind CSS, Alpine.js

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build
```

## Project Structure

```
/
├── public/           # Static assets
├── src/
│   ├── components/   # Astro components
│   ├── i18n/         # Translations (EN/ZH)
│   ├── layouts/      # Page layouts
│   ├── pages/        # Route pages
│   └── styles/       # Global styles
└── package.json
```

## Related Links

- Website: [shuo.us](https://shuo.us)
- GitHub: [shuo-us/shuo-website](https://github.com/shuo-us/shuo-website)

## License

Apache 2.0
