# Instruções para agentes neste projeto

## Sobre este projeto

- Documentação da API de integração da Credicarro (financiamento e refinanciamento de veículos), construída em [Mintlify](https://mintlify.com)
- Páginas são arquivos MDX com front-matter YAML
- Configuração de navegação em `docs.json`
- Páginas de referência de endpoints usam `openapi:` no front-matter e puxam descrição/parâmetros de `openapi.yaml` — não duplique essa informação manualmente na página
- Rode `mint dev` para pré-visualizar localmente e `mint broken-links` para checar links
- Siga o mesmo padrão da documentação do Parcele+ (`twila-parcelemais-documentation`) e da AbacatePay

## Terminologia

- "Credicarro" em texto visível para o leitor — "CrediCarro" aparece apenas em identificadores técnicos (ex.: header `X-CrediCarro-Signature`)
- "proposta", não "pedido" ou "contrato"
- "parceiro" ou "integrador" para quem consome a API — "cliente" é reservado para o comprador (`Customer`)
- "v2" é o fluxo recomendado; endpoints de simulação e proposta v1 são "legado"
- "lojista" para o leitor da aba Para lojistas; "loja" para o participante da proposta (`loja`, `cnpjLoja`)
- Códigos de erro (`tipo`) seguem o backend em `IntegrationErrorCodes` — confira antes de documentar um novo
- Todo o conteúdo das páginas é em português do Brasil

## Estilo

- Use voz ativa e segunda pessoa ("você")
- Frases curtas — uma ideia por frase
- Sentence case em títulos ("Criar proposta", não "Criar Proposta")
- Nomes de arquivo, comandos, caminhos e identificadores de código em `code formatting`
- Campos JSON de listas paginadas usam `itens` e `pagina` — reflete o nome do campo na API real

## Navegação

- Estrutura inspirada na documentação da [AbacatePay](https://github.com/AbacatePay/documentation): seletor de versão em `navigation.versions`
- **v2** (tag "Atual"): Comece aqui, Para lojistas, Para desenvolvedores, Autenticação, Proposta, Webhooks
- **v1** (tag "Legado"): Comece aqui, Para lojistas e Para desenvolvedores (iguais à v2, sem os guias v2), Autenticação, Proposta (com o fluxo v1), Webhooks
- **Para lojistas** (`pages/concepts/`, `pages/guides/first-proposal`, `pages/faq`, `pages/glossary`) é escrito para quem não programa: sem nomes de campos, códigos ou JSON — links para a parte técnica quando necessário
- **Para desenvolvedores** reúne integração, fluxo v2 e guias ponta a ponta (`pages/guides/*-integration`, `pages/guides/document-upload`)
- Endpoints ficam na barra lateral das abas de domínio (Autenticação, Proposta, Webhooks), como na documentação do Parcele+: cada grupo começa com uma visão geral (`reference.mdx`) e segue com as páginas de endpoint (`openapi:` no front-matter)
- Páginas compartilhadas entre versões (autenticação, cliente, webhooks) aparecem nas duas navegações
- Não renomeie caminhos de páginas já publicados; se for inevitável, adicione um `redirect` em `docs.json`

## Limites de conteúdo

- Documenta apenas a API de integração pública, voltada a parceiros — não documenta endpoints internos de backoffice/admin
