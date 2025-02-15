# @elizaos/plugin-perplexity

A plugin for Perplexity AI integration, providing automated text generation and research capabilities.

## Overview

This plugin provides functionality to:

- Generate text using Perplexity's Sonar models
- Customize prompts for context-aware content generation
- Access real-time web search results in responses
- Get structured outputs in JSON or regex formats

## Installation

```bash
npm install @elizaos/plugin-perplexity
```

## Configuration

The plugin requires the following environment variable:

```env
PERPLEXITY_API_KEY=your_perplexity_api_key
```

## Usage

Import and register the plugin in your Eliza configuration:

```typescript
import { perplexityPlugin } from "@elizaos/plugin-perplexity";

export default {
    plugins: [perplexityPlugin],
    // ... other configuration
};
```

### Generating Text

```typescript
const result = await generateTextAction.handler(runtime, message, state);
console.log(result.text); // Output generated by Perplexity
```

## Development

### Building

```bash
npm run build
```

### Testing

```bash
npm run test
```

## License

This plugin is part of the Eliza project. See the main project repository for license information.
