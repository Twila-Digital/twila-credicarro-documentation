<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="logo/dark.svg"></source>
    <source media="(prefers-color-scheme: light)" srcset="logo/light.svg"></source>
    <img alt="Credicarro Logo" src="logo/light.svg" width="300"></img>
  </picture>
</p>

# Credicarro Documentation

## 🚀 Quick Start

This documentation is built with [Mintlify](https://mintlify.com)

1. **Preview locally**
```bash
# Install Mintlify CLI
npm i -g mintlify

# Start development server
mintlify dev
```

2. **Visit `http://localhost:3000` to see your documentation**

## 📚 Documentation Structure

```
.
├── images/         # Store all documentation images and screenshots
├── logo/           # Brand logos for light and dark themes
├── pages/          # Main documentation content
├── docs.json       # Mintlify configuration file for documentation settings
├── favicon.ico     # Website favicon
├── openapi.yaml    # OpenAPI/Swagger specification file
└── README.md       # Project overview and setup instructions
```

## 🔧 Local Development

1. **Install dependencies**
```bash
mintlify install
```

2. **Start development server**
```bash
mintlify dev
```

### OR

1. Run using docker
```bash
make start
```

### Troubleshooting

- If Mintlify dev isn't running, try `mintlify install` to reinstall dependencies
- For 404 errors, ensure you're in a directory with `mint.json`

## 🚀 Deployment

Changes are automatically deployed when merged to the `production` branch, through the Mintlify GitHub integration.

See [Mintlify GitHub App Documentation](https://mintlify.com/docs/settings/github) for more information.
