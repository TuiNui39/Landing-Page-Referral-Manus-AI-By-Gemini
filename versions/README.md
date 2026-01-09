# Language Versions

This directory contains different language versions of the Manus AI Referral Landing Page.

## Available Languages

### 🇹🇭 Thai (ไทย)
- **Path:** `versions/th/index.html`
- **Status:** ✅ Backed up
- **Last Updated:** 2026-01-09

### 🇺🇸 English (อังกฤษ)
- **Path:** `versions/en/index.html`
- **Status:** ✅ Active (Deployed to manus-flow.com)
- **Last Updated:** 2026-01-09

## Usage

### To switch language versions:

1. **Deploy Thai version:**
   ```bash
   cp versions/th/index.html index.html
   wrangler pages deploy . --project-name=manus-flow-landing
   ```

2. **Deploy English version:**
   ```bash
   cp versions/en/index.html index.html
   wrangler pages deploy . --project-name=manus-flow-landing
   ```

## Adding New Languages

To add a new language version:

1. Create a new directory: `versions/{language_code}/`
2. Copy and translate `index.html`
3. Update this README
4. Deploy when needed

## Language Codes

- `th` - Thai (ไทย)
- `en` - English (อังกฤษ)
- `zh` - Chinese (中文)
- `ja` - Japanese (日本語)
- `ko` - Korean (한국어)
- etc.
