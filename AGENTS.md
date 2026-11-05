# Documentação do PostClean: instruções

- Site Mintlify: páginas MDX com frontmatter YAML; navegação e `openapi` ficam no `docs.json`.
- Idioma único: português do Brasil. Rótulos de tela em negrito, exatamente como em `lang/pt-BR/*.php` do app.
- O código do app (fonte da verdade) é o repositório do PostClean (`chatclean post`). Toda afirmação sobre comportamento precisa bater com o código.
- O PostClean é só SaaS: não há self-hosting nem comparação "Cloud vs self-hosted".

## URLs

| Serviço | URL |
| --- | --- |
| App | `https://post.chatclean.com.br` |
| API REST | `https://post.chatclean.com.br/api` |
| Servidor MCP | `https://post.chatclean.com.br/mcp/trypost` (o caminho é esse mesmo) |
| Suporte | `contato@chatclean.com.br` |

Nos guias de clientes de IA, o nome do servidor MCP é `postclean`.

## URLs congeladas (o app linka para elas)

- `/`, `/ai/introduction`
- `/platforms/<slug>`: instagram, facebook, threads, x-twitter, linkedin, tiktok, youtube, pinterest, bluesky, mastodon, discord, telegram, google-business
- `/knowledge-base/media` com as âncoras `#instagram #facebook #threads #x-twitter #linkedin #tiktok #youtube #pinterest #bluesky #mastodon #discord #telegram #google-business-profile`. Os títulos das redes nessa página não podem ser traduzidos.
- `/knowledge-base/automations/external-agent` (destino de `AUTOMATIONS_AGENT_DOCS_URL`)

Se alguma precisar mudar, adicione um `redirects` no `docs.json`.

## API

`openapi.json` gera as páginas de endpoint. As descrições dos endpoints ainda estão em inglês e alguns schemas de posts descrevem uma versão mais nova do TryPost; quando divergirem, vale o guia `api-reference/guides/posting.mdx`.
