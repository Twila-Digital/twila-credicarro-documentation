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
├── images/              # Imagens e capturas de tela
├── logo/                # Logos para os temas claro e escuro
├── pages/
│   ├── introduction.mdx # Página inicial (lojista x desenvolvedor)
│   ├── concepts/        # Para lojistas: produto, jornada, documentos, custos
│   ├── guides/          # Guias (lojista e desenvolvedor)
│   ├── reference/       # Convenções da API
│   ├── customer/        # Endpoints de cliente (v1, compartilhados)
│   ├── simulation/      # Endpoints de simulação v1 e consultas
│   ├── proposal/        # Endpoints de proposta v1 e listagem
│   ├── webhook/         # Endpoints de webhook (compartilhados)
│   ├── webhooks/        # Segurança dos webhooks
│   ├── v1/              # Páginas exclusivas da versão v1
│   └── v2/              # Fluxo, etapas, webhook e endpoints v2
├── docs.json            # Navegação (versões v2 e v1) e configuração do Mintlify
├── favicon.ico
├── openapi.yaml         # Especificação OpenAPI usada nas páginas de endpoint
└── README.md
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
