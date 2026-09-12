# 旅行汉语 · Chinês para Viagem

Flashcards de chinês mandarim para usar em viagem, direto no navegador do celular.

**Estudar agora:** https://abouhid2.github.io/chines-viagem/

## O que tem

- Vocabulário e frases de conversação organizados por categoria (saudações, restaurante, transporte, hotel, compras, emergência, aeroporto, conversa, números, tempo).
- Áudio em mandarim via Web Speech API (toque no botão ♪).
- Pinyin na frente do card e tradução no verso.
- Etimologia dos caracteres, para memorizar pelo sentido e não pela força bruta.
- Swipe estilo baralho: direita = "sei", esquerda = "revisar".
- Progresso salvo no próprio aparelho (localStorage), com painel de vocabulário filtrável por categoria e sessão só com as palavras marcadas para revisar.

## Como usar

- **Toque no card** ou tecla `espaço`: vira o card.
- **Swipe direita / seta →**: marca como "sei".
- **Swipe esquerda / seta ←**: manda para "revisar".
- **Botão de menu** (canto superior direito): abre a lista completa, com filtro por categoria e por status. O botão "Treinar esta lista" inicia uma sessão só com o que está filtrado.

No iPhone, use **Safari** e adicione à tela de início (Compartilhar > Adicionar à Tela de Início) para abrir como app. O áudio em mandarim depende das vozes instaladas no aparelho; em Ajustes > Acessibilidade > Conteúdo Falado > Vozes é possível baixar a voz chinesa.

## Adicionar palavras

Todo o conteúdo fica no array `deck`, dentro de `index.html`. Cada entrada tem o formato:

```js
{ hanzi: "你好", pinyin: "nǐ hǎo", pt: "olá", cat: "Saudação",
  etym: "<span class=\"han\">你</span> (você) + <span class=\"han\">好</span> (bom)" }
```

`etym` é opcional. Uma categoria nova aparece automaticamente como filtro no painel.

## Estrutura

Página estática única, sem build e sem dependências além das fontes do Google Fonts. Publicada por GitHub Pages a partir da branch `main`.
