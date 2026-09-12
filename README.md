# 旅行汉语 · Chinês para Viagem

Flashcards de chinês mandarim para usar em viagem, direto no navegador do celular.

**Estudar agora:** https://abouhid2.github.io/chines-viagem/

## O que tem

- **450 palavras e frases**, todas com pinyin, tradução e explicação caractere por caractere.
- **Cobertura completa de HSK 1 e HSK 2**, o núcleo de vocabulário de um iniciante (157 + 157 palavras), somado a 136 frases práticas de viagem que não aparecem nas listas oficiais.
- **Teste de nível A1 e A2**: 15 perguntas de múltipla escolha que alternam entre hanzi para português e português para hanzi. No fim mostra o percentual e um veredito, e o que você errou entra automaticamente na fila de revisão, com botão para treinar só esses erros.
- **27 áreas temáticas** (saudações, restaurante, transporte, hotel, compras, emergência, aeroporto, conversa, verbos, pronomes, gramática, adjetivos, números, tempo e outras), cada uma com contagem e barra de progresso.
- Áudio em mandarim via Web Speech API (toque no botão ♪).
- Swipe estilo baralho: direita para "sei", esquerda para "revisar".
- Progresso salvo no próprio aparelho (localStorage).

## Como usar

- **Toque no card** ou tecla `espaço`: vira o card.
- **Swipe direita / seta →**: marca como "sei".
- **Swipe esquerda / seta ←**: manda para "revisar".
- **Botão de menu** (canto superior direito): abre a grelha de áreas. Toque numa área para ver a lista completa dela, ou nas duas cartas vermelhas para fazer o teste de nível. O botão "Treinar esta lista" inicia uma sessão só com o que está filtrado.

No iPhone, use Safari e adicione à tela de início (Compartilhar > Adicionar à Tela de Início) para abrir como app. O áudio depende das vozes instaladas; em Ajustes > Acessibilidade > Conteúdo Falado > Vozes é possível baixar a voz chinesa.

Se a página aparecer cortada ou muito pequena, verifique se o navegador está em "modo desktop" e abra https://abouhid2.github.io/chines-viagem/diag.html, que mostra a largura lógica, o zoom aplicado e se a página está transbordando.

## Sobre os níveis A1 e A2

Não existe tabela de equivalência oficial entre HSK e CEFR endossada pelos dois organismos, e as fontes divergem. O critério adotado aqui é o mais prático para quem está começando:

- **A1** = as 157 palavras de HSK 1
- **A2** = as 157 palavras novas de HSK 2
- **Viagem** = frases de sobrevivência que não constam do HSK

Isso também conversa com a faixa de 500 a 700 vocábulos que a literatura do CEFR costuma associar ao A1.

## Adicionar palavras

Todo o conteúdo fica no array `deck`, dentro de `index.html`:

```js
{ hanzi: "你好", pinyin: "nǐ hǎo", pt: "olá", cat: "Saudação", lvl: "A1",
  etym: "<span class=\"han\">你</span> (você) + <span class=\"han\">好</span> (bom)" }
```

`lvl` aceita `A1`, `A2` ou `Viagem` e define de qual teste a palavra participa. Uma categoria nova em `cat` aparece sozinha como área na grelha.

## Estrutura

Página estática única, sem build e sem dependências além das fontes do Google Fonts. Publicada por GitHub Pages a partir da branch `main`.
