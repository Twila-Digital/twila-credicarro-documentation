# Instruções para agentes neste projeto

## Sobre este projeto

- Documentação da API de integração da Credicarro (financiamento e refinanciamento de veículos), construída em [Mintlify](https://mintlify.com)
- Páginas são arquivos MDX com front-matter YAML
- Configuração de navegação em `docs.json`
- Páginas de referência de endpoints usam `openapi:` no front-matter e puxam descrição/parâmetros de `openapi.yaml` — não duplique essa informação manualmente na página
- Rode `mint dev` para pré-visualizar localmente e `mint broken-links` para checar links
- Siga o mesmo padrão da documentação do Parcele+ (`twila-parcelemais-documentation`)

## Terminologia

- "Credicarro" em texto visível para o leitor — "CrediCarro" aparece apenas em identificadores técnicos (ex.: header `X-CrediCarro-Signature`)
- "proposta", não "pedido" ou "contrato"
- "parceiro" ou "integrador" para quem consome a API — "cliente" é reservado para o comprador (`Customer`)
- "v2" é o fluxo recomendado; endpoints de simulação e proposta v1 são "legado"
- Todo o conteúdo das páginas é em português do Brasil

## Estilo

- Use voz ativa e segunda pessoa ("você")
- Frases curtas — uma ideia por frase
- Sentence case em títulos ("Criar proposta", não "Criar Proposta")
- Nomes de arquivo, comandos, caminhos e identificadores de código em `code formatting`
- Campos JSON de listas paginadas usam `itens` e `pagina` — reflete o nome do campo na API real

## Navegação

- Abas por domínio: Comece aqui, Para Desenvolvedores, Autenticação, Proposta, Webhooks
- Cada aba começa com um grupo de visão geral/fluxo e depois os grupos de endpoints
- Não renomeie caminhos de páginas já publicados; se for inevitável, adicione um `redirect` em `docs.json`

## Limites de conteúdo

- Documenta apenas a API de integração pública, voltada a parceiros — não documenta endpoints internos de backoffice/admin
