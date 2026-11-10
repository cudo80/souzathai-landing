# SouzaThai Massoterapia — Landing Page

Landing page de **Leandro Souza (SouzaThai)**: massoterapia, cuidador de idosos, crianças e PcD, cursos e palestras — atendimento a domicílio na Grande Florianópolis (Florianópolis, São José, Palhoça e Biguaçu).

**Contato:** WhatsApp (48) 99604-1664 · [Instagram @erechimsouza](https://www.instagram.com/erechimsouza/) · terapeutasc@hotmail.com

## 🌐 Site no ar
Após ativar o GitHub Pages, a página fica em:
**https://cudo80.github.io/souzathai-landing/**

> A URL canônica está definida nesse endereço. Se migrar para Netlify ou domínio próprio (ex.: `souzathai.com.br`), atualize a canonical, os metadados OG, o `robots.txt` e o `sitemap.xml` no `index.html`.

## 📄 Estrutura
- `index.html` — página completa (HTML + CSS + JS embutidos, sem build)
- `robots.txt` / `sitemap.xml` — indexação no Google
- `og-image.png` — imagem de prévia ao compartilhar o link

## 🔧 Como editar (sem ferramentas)
Abra o `index.html` em qualquer editor de texto e procure por:

| O que trocar | Onde procurar |
|---|---|
| Fotos por imagens reais | comentários `<!-- PLACEHOLDER: ... -->` |
| Avaliações de clientes | seção `#depoimentos`; transcrição em `assets/data/avaliacoes.json` |
| Textos dos serviços | seções dos 3 pilares |

## 🚀 Publicar no Netlify (alternativa)
Acesse [app.netlify.com/drop](https://app.netlify.com/drop) e arraste a pasta inteira. Pronto.

## 📈 SEO pós-lançamento (recomendado)
1. Cadastrar em [Google Search Console](https://search.google.com/search-console) e enviar o sitemap
2. Criar **Google Meu Negócio** (perfil de serviço móvel — por área de atendimento)
3. Adicionar o link do site na **bio do Instagram**

## Avaliações de clientes

A seção **Recomendações de clientes** contém 36 avaliações únicas transcritas das 17 capturas da Cronoshare anexadas pelo usuário, substituindo os três depoimentos de exemplo. Os cards são HTML estático e não dependem de JavaScript para aparecer.

- Transcrição e rastreabilidade: `assets/data/avaliacoes.json`, com nome, data, nota original de 0 a 10, comentário e imagens de origem.
- A grafia dos comentários foi preservada, normalizando apenas quebras de linha. Aparições repetidas foram reunidas.
- Myriam e Dione não apresentam comentário nas capturas; os cards indicam isso sem inventar relatos.
- Valdecir Roberto tem nota **9/10** (4,5 estrelas) e Sonia Mara Da Silva **5/10** (2,5 estrelas); as demais notas são **10/10**.
- O link Cronoshare de cada card abre o site oficial https://www.cronoshare.com.br/ em nova aba. As capturas de origem ficam registradas em `assets/data/avaliacoes.json`; os arquivos originais não foram alterados.
- O cabeçalho da plataforma mostra média 9,8 e 36 avaliações. Esses valores não foram usados como média calculada dos comentários transcritos nem adicionados ao JSON-LD.

Ao corrigir uma transcrição, atualize o JSON e o card correspondente no `index.html`, conferindo a imagem de origem. Referências de marcação: [HTML Standard: blockquote](https://html.spec.whatwg.org/multipage/grouping-content.html#the-blockquote-element) e [time](https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-time-element).

## Responsividade

A foto respeita a largura disponível e mantém o recorte circular; a coluna da seção Sobre pode encolher em telas estreitas. Em 10/11/2026, a página foi testada localmente com Playwright e Chrome headless nas larguras de 320, 360, 390, 768, 820, 821, 920, 921, 1024, 1280 e 1440 px: sem transbordamento horizontal ou erros JavaScript. O menu mobile abriu, fechou com Escape e devolveu o foco ao botão. Capturas de celular, tablet e desktop também foram inspecionadas. Isso não representa teste em aparelhos físicos ou em outros navegadores.

Referência para a largura mínima de verificação: [W3C — Reflow, 320 CSS px](https://www.w3.org/WAI/WCAG22/Understanding/reflow.html).
