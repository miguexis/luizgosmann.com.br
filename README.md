# luizgosmann.com.br

Site de **Luiz Miguel Gosmann** — consultoria para pizzarias. HTML estático, sem build, servido via
GitHub Pages em **https://luizgosmann.com.br**. Os domínios **luizmiguelgosmann.com.br** e
**miguelgosmann.com.br** vão redirecionar pro principal (redirect 301 na Cloudflare, configuração prevista pra S1).

Contato: contato@luizgosmann.com.br

## Estado

Atualizado em dom 25/10/2026.

- **S1 (26–30/10/2026) — esqueleto, que é o que está neste repo.** O `index.html` é um placeholder
  temporário com `<meta name="robots" content="noindex,nofollow">`: nada aqui é pra ser indexado antes
  da v1. Sem `robots.txt` nem `sitemap.xml` ainda — os dois entram no mesmo commit da v1.
- **S3 (09–13/11/2026) — v1 no ar:** 4 páginas (Início, Raio-X, Como funciona, Contato) e a lista
  técnica abaixo, no mesmo commit; o `noindex` sai.
- **S4–S6 (16/11–04/12/2026):** Serviços, Sobre e FAQ (S4) e o Guia, uma página por pergunta,
  publicado em três lotes (páginas 1–3 na S4, 4–8 na S5, 9–12 na S6).

## Lista técnica da v1 (§8.2 da encomenda)

- `robots.txt` com `User-agent: *` liberado e linhas explícitas pra Googlebot, Bingbot, OAI-SearchBot,
  ChatGPT-User, GPTBot, Claude-SearchBot, Claude-User, ClaudeBot, PerplexityBot e Google-Extended
- `sitemap.xml`
- JSON-LD: Person (com `alternateName` "Miguexis"), ProfessionalService, Service e FAQPage
- `canonical` e Open Graph em toda página
- IndexNow (chave publicada no site + ping a cada publish)
- política de privacidade e consentimento no formulário de contato
- Cloudflare Web Analytics (sem cookie)
- HTTPS forçado no GitHub Pages e domínio verificado no GitHub
- sem vídeo na v1

## Regras deste repositório — ele é PÚBLICO

- **Nunca entra aqui:** segredo ou credencial, dado de cliente, número real das casas do Luiz, margem
  ou estrutura de custo.
- **Casos entram anonimizados**, nas regras da §0 da encomenda — inclusive a de qual casa do Luiz
  nunca é nomeada em case. O nome não está neste README de propósito: o repo é público.
- **Entidade clara em toda página:** "Luiz Miguel Gosmann" por extenso. "Miguexis" é apelido
  (`alternateName` no schema.org), nunca marca.
- **Fonte oficial da frente:** o repo privado `consultoria-ops`, arquivo `docs/ENCOMENDA-2026-10-25.md`.
  O que não estiver lá não se inventa aqui.

## Rodar local

Não há build: abrir `index.html` no navegador.
