# Spotify History — Timeline

Visualizador de histórico do Spotify em formato de timeline. Carregue os arquivos JSON do seu pacote de dados do Spotify e explore suas reproduções por ano e mês, com estatísticas, filtros e busca.

🔗 **Online:** https://timeline.computeiros.com/

## Funcionalidades

- Upload de vários arquivos JSON por arrastar e soltar ou seleção, com possibilidade de adicionar mais arquivos depois
- Timeline agrupada por mês, com carregamento paginado (200 itens por vez)
- Estatísticas gerais: reproduções, artistas, horas ouvidas e anos
- Gráfico de reproduções por ano
- Top 8 artistas e músicas, por ano ou geral
- Busca por música, artista ou álbum
- Filtros: puladas, offline e shuffle
- Ordenação por data, duração ou artista
- Detalhes de cada faixa: plataforma, país, motivo de início e fim, timestamp, modo incógnito e link para abrir no Spotify
- Remoção automática de duplicados (por `ts` + URI da faixa)

## Privacidade

Tudo roda **100% no navegador**. Os arquivos JSON são lidos localmente com a File API e **nunca são enviados a nenhum servidor**. Não há backend, cookies nem rastreamento. Os únicos recursos externos são as fontes do Google Fonts.

## Como obter seus dados

1. Acesse [spotify.com/account/privacy](https://www.spotify.com/account/privacy/).
2. Solicite o **"Extended streaming history"** (histórico estendido) ou os dados da conta.
3. Aguarde o e-mail do Spotify e baixe o pacote.
4. Use os arquivos JSON, por exemplo `Streaming_History_Audio_2023.json` ou `StreamingHistory_music_0.json`.

> Apenas faixas de música são exibidas. Podcasts e audiolivros são ignorados.

## Como usar

Abra a página, arraste os arquivos `.json` para a área de upload e navegue pela timeline.

Para rodar localmente, basta abrir o `index.html` no navegador. Não há build nem dependências.

## Estrutura

| Arquivo | Descrição |
|---|---|
| `index.html` | Aplicação completa (HTML, CSS e JavaScript) |
| `robots.txt` | Regras para indexação |
| `sitemap.xml` | Sitemap para buscadores |
| `CNAME` | Domínio customizado do GitHub Pages |

## Hospedagem (GitHub Pages)

1. Publique os arquivos na raiz do repositório, com o arquivo principal como `index.html`.
2. Crie um arquivo `CNAME` com `timeline.computeiros.com`.
3. No DNS, crie um registro `CNAME` de `timeline` para `SEU-USUARIO.github.io`.
4. Em *Settings → Pages*, selecione a branch e ative **Enforce HTTPS**.

> ⚠️ **Não envie ao repositório os JSONs do seu histórico.** Eles contêm dados pessoais.

## Tecnologias

HTML, CSS e JavaScript puro, sem frameworks. Fontes: Syne, DM Mono e DM Sans.

## Aviso

Projeto independente, sem afiliação com o Spotify. Spotify é marca registrada de seus respectivos proprietários.
