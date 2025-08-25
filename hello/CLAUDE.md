# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Simple Node.js project that demonstrates OpenAI API integration, specifically configured for Moonshot AI's Kimi model. The project uses the official OpenAI client library but connects to Moonshot AI's API endpoint.

## Architecture

- **Entry Point**: `main.js` - Single file application that demonstrates OpenAI API usage
- **Dependencies**: Uses `openai` npm package v5.15.0
- **Configuration**: API key loaded from `OPENAI_API_KEY` environment variable
- **API Endpoint**: Configured for Moonshot AI at `https://api.moonshot.cn/v1`
- **Model**: Uses `kimi-k2-0711-preview` model

## Development Commands

### Setup
```bash
# Install dependencies
npm install

# Set API key
export OPENAI_API_KEY=your_key_here
```

### Run
```bash
# Execute the application
node main.js
```

### Files
- `main.js:3-6` - OpenAI client configuration
- `main.js:8-22` - Main async function with API call
- `main.js:10` - Model configuration
- `main.js:15` - System prompt (Chinese language)

## Key Configuration Notes

- **Environment Variable**: Must set `OPENAI_API_KEY` before running
- **API Base URL**: Uses Moonshot AI instead of OpenAI's default endpoint
- **Model**: `kimi-k2-0711-preview` is a Chinese-optimized model
- **System Prompt**: Pre-configured in Chinese for general assistance

## Testing

No test framework configured. Basic verification can be done by running `node main.js` with a valid API key.