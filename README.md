# SignDocs Brasil

**Assinatura eletrônica e digital com validade jurídica no Brasil.** API REST, SDKs oficiais em seis
linguagens e integrações prontas — com ICP-Brasil (A1/A3), biometria facial, OTP e trilha de
evidências assinada.

*Brazilian e-signature platform: REST API, official SDKs and ready-made integrations, with
ICP-Brasil certificates, facial biometrics, OTP and a signed evidence trail.*

[Site](https://www.signdocs.com.br) · [Documentação da API](https://docs.signdocs.com.br) · [Guia de início rápido](https://docs.signdocs.com.br/guias/inicio-rapido.html)

---

## SDKs oficiais

| Linguagem | Pacote | Instalação |
| --- | --- | --- |
| TypeScript / Node.js | [`@signdocs-brasil/api`](https://www.npmjs.com/package/@signdocs-brasil/api) | `npm i @signdocs-brasil/api` |
| Python | [`signdocs-brasil`](https://pypi.org/project/signdocs-brasil/) | `pip install signdocs-brasil` |
| PHP | [`signdocs-brasil/signdocs-brasil-php`](https://packagist.org/packages/signdocs-brasil/signdocs-brasil-php) | `composer require signdocs-brasil/signdocs-brasil-php` |
| Java | [`io.github.signdocsbrasil:signdocsbrasil-api`](https://central.sonatype.com/artifact/io.github.signdocsbrasil/signdocsbrasil-api) | Maven Central |
| .NET | [`SignDocsBrasil.Api`](https://www.nuget.org/packages/SignDocsBrasil.Api) | `dotnet add package SignDocsBrasil.Api` |
| Go | [`signdocsbrasil-go`](https://pkg.go.dev/github.com/signdocsbrasil/signdocsbrasil-go/v2) | `go get github.com/signdocsbrasil/signdocsbrasil-go/v2` |

Todos autenticam por OAuth2 (`client_secret` ou `private_key_jwt` com ES256) e trazem retry,
paginação automática e verificação de assinatura de webhook.

## Integrações

| | |
| --- | --- |
| [MCP Server](https://github.com/signdocsbrasil/signdocs-mcp-server) | Assine por linguagem natural em qualquer cliente MCP — Claude, Cursor, Claude Code |
| [Plugin Claude](https://github.com/signdocsbrasil/signdocs-mcp-plugin) | Plugin do Claude Code e extensão do Claude Desktop |
| [n8n](https://github.com/signdocsbrasil/n8n-nodes-signdocs-brasil) | Nó community para automações |
| [Zapier](https://github.com/signdocsbrasil/signdocs-zapier-app) | Integração para o Zapier |
| [WordPress](https://github.com/signdocsbrasil/signdocs-brasil-wordpress) | Plugin oficial, com suporte a WooCommerce |
| [Nextcloud](https://github.com/signdocsbrasil/signdocs-nextcloud) | Assine direto do app Arquivos |
| [LibreOffice](https://github.com/signdocsbrasil/signdocs-libreoffice) | Envie o documento aberto sem sair do Writer, Calc, Impress ou Draw |
| [Lovable](https://github.com/signdocsbrasil/signdocs-lovable-starter) | Starter remixável via Supabase Edge Functions |
| [Assinador A3](https://github.com/signdocsbrasil/signdocsbrasil-assinador) | Ponte PKCS#11 para token e cartão em hardware |

## Níveis de assinatura

Conforme a **Lei 14.063/2020** e a **MP 2.200-2/2001**:

- **Simples** — aceite eletrônico com registro de IP, geolocalização e horário
- **Avançada** — OTP por e-mail ou SMS, biometria facial com prova de vida, documento de identidade
- **Qualificada** — certificado digital ICP-Brasil A1 (via API) ou A3 (token/cartão, pelo assinador)

Cada envelope concluído gera um **pacote de evidências** em PKCS#7/CMS, assinado e verificável de
forma independente.

## Sandbox

O ambiente de homologação é gratuito para testar a integração de ponta a ponta antes de ir para
produção. Comece pelo [guia de início rápido](https://docs.signdocs.com.br/guias/inicio-rapido.html).
