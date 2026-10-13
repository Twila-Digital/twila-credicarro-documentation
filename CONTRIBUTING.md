# Contribuindo com a documentação

## Como contribuir

### Opção 1: editar direto no GitHub

1. Navegue até a página que quer editar
2. Clique no ícone de lápis ("Edit this file")
3. Faça as alterações e abra um pull request

### Opção 2: desenvolvimento local

1. Clone este repositório e crie uma branch
2. Instale a CLI da Mintlify: `npm i -g mint`
3. Rode `mint dev` na raiz do repositório (ou `make start` com Docker) e pré-visualize localmente
4. Rode `mint broken-links` antes de abrir o PR
5. Abra um pull request para `production`

## Diretrizes de escrita

- Use voz ativa e se dirija ao leitor na segunda pessoa ("você")
- Frases curtas — uma ideia por frase
- Comece pelo objetivo do leitor, não pela implementação
- Use sempre o mesmo termo para o mesmo conceito (veja [AGENTS.md](AGENTS.md#terminologia))
- Prefira exemplos de código a apenas descrever o comportamento
- Páginas de referência de endpoint (`openapi: "..."` no front-matter) não devem duplicar descrição/parâmetros — isso vem de `openapi.yaml`
