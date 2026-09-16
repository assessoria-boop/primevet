# Prime Vet — Clínica Veterinária 24h (Landing Page)

Página única e estática (`index.html`), recriada a partir das pranchetas "Desktop V1" e "Mobile V1" do template premium do Paper.
Não usa bibliotecas: as fontes (Manrope e Montserrat) ficam em `fonts/` e todo o CSS/JS está no próprio HTML.

## Seções (na ordem)
Hero → cards de destaque (3) → Avaliações (carrossel) → O que fazemos (3 cards) →
Serviços (lista com foto que abre + notificações flutuando) → Cards Cães/Gatos →
Etapas (carrossel) → CTA final com mapa → Rodapé. Botão flutuante do WhatsApp.

## Paleta
Preto e prata da logo, com o vermelho da Prime Vet na linha "Veterinária 24h". Hero claro, com texto em preto.

| Uso | Cor |
|---|---|
| Preto da marca (ícones, barra dos carrosséis, card do CTA) | `#111111` |
| Grafite (destaques de texto, botão ativo, "serviços") | `#3F3F46` |
| Prata (link "Como chegar") | `#D4D4D8` |
| Vermelho da linha "Veterinária 24h" do hero | `#E53935` |
| Fundo da seção Serviços | `#F4F4F5` |
| Rodapé | `#0B0B0C` |
| Hero (degradê claro, mais escuro do lado do cão) | `#F4F4F5 → #ECECEE → #CFCFD4 → #A1A1AA` |
| CTAs | verde do WhatsApp `#25D366` |

## Imagens (`img/`)

| Arquivo | O que é | Origem |
|---|---|---|
| `primevet-logo-96.webp`, `primevet-logo-192.png` | Ícone da logo (cabeçalho, rodapé e favicon) | recortado da logo do cliente |
| `logo.webp` | Logo completa | do cliente |
| `avaliacao-1.webp` … `avaliacao-5.webp` | Prints reais do Google | do cliente (os mesmos 1–5.webp da página anterior) |
| `etapa-01.webp` … `etapa-04.webp` | Fotos da seção **Etapas** (recortadas em 740×440) | do cliente ✅ |
| `destaque-cirurgia/exames/consultas.webp` | Cards de "O que fazemos" e fotos da lista de serviços (600×800) | do cliente ✅ |
| `laboratorio.webp` | Foto da linha "Laboratório" na lista de serviços (600×612) | do cliente ✅ |
| `hero-cao-1100/1600.webp` | Cão do hero (mobile/desktop) | foto do template |
| `card-caes/gatos.webp`, `servico-emergencia.webp` | Cards Cães/Gatos e foto da linha "Emergência 24h" | fotos do template |

Para trocar uma foto, mantenha o mesmo nome. As etapas usam 740×440 px (WebP, qualidade ~80).
Os originais da marca ficam em `C:\Users\Gaabs\brand-assets\prime-vet` (as fotos de 16/09 ficam em `fotos-originais-16-09`).

## Integrações
- **WhatsApp**: `wa.me/5561998324760`, com a mensagem "Olá encontrei vocês pelo Google, gostaria de atendimento." (a mesma da página anterior).
- **Google Tag Manager**: `GTM-WGTJFJVS` (o mesmo da página anterior).
- **Microsoft Clarity**: `yjavigcci0`.
- **Mapa**: o mesmo embed da página anterior, carregado só quando a seção de contato se aproxima da tela.

GTM e Clarity carregam na primeira interação (toque, rolagem, mouse ou tecla), fora do caminho do carregamento.

## CTAs
Todos os botões verdes levam ao mesmo WhatsApp. Os principais (hero e CTA final) dizem "ATENDIMENTO IMEDIATO" e mudam para "ABRINDO O WHATSAPP" ao clicar.

## Medições (16/09/2026, servidor local)
- Altura no desktop: 5.841 px (prancheta: 5.840 px).
- Lighthouse desktop: 100 desempenho / 93 acessibilidade / 100 boas práticas / 100 SEO.
- Lighthouse mobile: 92–95 / 93 / 100 / 100 (LCP 2,3 s, CLS 0).
- Acessibilidade fica em 93 por causa do `user-scalable=no` do viewport, que vem do template.
