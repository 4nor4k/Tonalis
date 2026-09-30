# Tonalis

Painel de consulta rápida de teoria musical, pensado para quem está compondo ou produzindo beats e precisa de resposta na hora — sem enrolação, sem precisar decorar teoria.

## O que o Tonalis faz

- **Roda de tonalidades** — escolha qualquer nota (em cifra: C, D, E, F#...) e veja, na hora, a escala maior, a escala menor relativa e as tonalidades vizinhas.
- **Acordes** — tríades (maior, menor, diminuto), acordes com sétima (maj7, m7, dominante7, m7b5, dim7) e com nona (maj9, m9, dominante9), todos calculados automaticamente a partir da tônica escolhida.
- **Teclado visual** — cada acorde aparece desenhado num teclado de piano, com as notas marcadas, pra você tocar de ouvido ou conferir no seu teclado MIDI.
- **Progressões prontas por estilo** — mais de 15 progressões de acordes comuns em pop, trap, lo-fi, R&B/neo-soul, blues, house, rock, jazz, reggaeton, afrobeats, boom bap, synthwave, funk e trilha cinematográfica, já transpostas pra tonalidade selecionada. Cada uma pode ser tocada (áudio sintetizado simples) direto na página.
- **Regras de formação de acordes** — um painel de referência mostrando a fórmula de semitons de cada tipo de acorde (ex: acorde maior = 4 + 3 semitons).

Não é um app que ensina teoria musical do zero — é uma referência rápida pra consultar enquanto você compõe.

## Instalar como app (PWA)

O Tonalis é um PWA (Progressive Web App): funciona direto no navegador e também pode ser instalado na tela inicial do celular, abrindo como um app normal, com ícone próprio e sem a barra de endereço do navegador.

### Android (Chrome)

1. Abra o link do Tonalis no Chrome.
2. Toque no menu de três pontinhos, no canto superior direito.
3. Toque em **"Instalar app"** (ou **"Adicionar à tela inicial"**, dependendo da versão do Chrome).
4. Confirme. O ícone do Tonalis aparece na tela inicial, junto com os outros apps.

### iPhone / iPad (Safari)

1. Abra o link do Tonalis no Safari (precisa ser no Safari — outros navegadores no iOS não suportam instalar PWA).
2. Toque no ícone de **Compartilhar** (o quadrado com uma seta pra cima), na barra inferior.
3. Role as opções e toque em **"Adicionar à Tela de Início"**.
4. Confirme o nome e toque em **"Adicionar"**. O ícone do Tonalis aparece na tela inicial.

Depois de instalado, o app funciona offline (o essencial da página fica salvo no aparelho) e abre igual a qualquer outro app do celular.

## Publicar / atualizar este repositório

Este repositório é servido como site estático via **GitHub Pages**:

1. Em **Settings → Pages**, escolha a branch `main` e a pasta `/ (root)`.
2. O link gerado (algo como `https://usuario.github.io/repositorio/`) é o que se usa nos passos de instalação acima.

Para atualizar o app depois de alguma mudança nos arquivos, basta subir os arquivos novos substituindo os antigos (mesmos nomes) e aguardar o GitHub Pages reprocessar — geralmente leva menos de um minuto. Como o app tem cache offline (`sw.js`), pode ser necessário limpar o cache do navegador/app no celular para ver a versão mais recente.

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | A aplicação inteira (HTML, CSS e JavaScript em um único arquivo) |
| `manifest.json` | Metadados do PWA (nome, ícones, cores) |
| `sw.js` | Service worker — permite o app funcionar offline |
| `icon-*.png`, `favicon*.png`, `apple-touch-icon.png`, `favicon.ico` | Ícones do app em diferentes tamanhos |
