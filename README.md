# REPERTÓRIO.

Site estático de estudos para comunicação, argumentação, publicidade, mídia, marketing de influência e repertório cultural. Desenvolvido com HTML, CSS e JavaScript, sem build, login ou backend.

## Como testar

O `index.html` usa `fetch()` para carregar `data/content.json`; por isso, não abra o arquivo diretamente com duplo clique (`file://`). Rode um servidor estático local, por exemplo:

```bash
python -m http.server 8000
```

Depois abra `http://localhost:8000` na pasta do projeto.

## Publicar no GitHub Pages

1. Extraia o ZIP no computador.
2. Crie um repositório no GitHub.
3. Envie o conteúdo da pasta `repertorio-site` para a raiz do repositório. A raiz deve conter `index.html`, `assets/` e `data/` — não deixe tudo escondido dentro de uma segunda pasta.
4. No repositório, abra **Settings → Pages**.
5. Em **Build and deployment**, escolha **Deploy from a branch**, selecione `main` e `/ (root)`, e salve.
6. Aguarde a publicação e abra a URL indicada pelo GitHub Pages.

Os caminhos dos arquivos são relativos, para funcionar em páginas de projeto. Se editar o conteúdo, mantenha IDs estáveis em `data/content.json`.

## Funcionalidades incluídas

- Página Hoje com rotina diária de quatro atividades.
- Seis trilhas e currículo de módulos.
- Biblioteca com busca e filtros por trilha/status.
- 12 aulas introdutórias com explicações, exemplos, prática, reflexão e quizzes.
- Laboratório de fala e desafios de argumentação.
- Glossário inicial com 36 termos.
- Dois casos para análise e simulador de campanha hipotética.
- Caderno pessoal, favoritos, conclusão de aulas, histórico e revisões simples.
- Progresso por trilha e exportação/importação de backup JSON.
- Armazenamento local no navegador.

## Limitações conhecidas

- Não há login nem sincronização entre dispositivos.
- Dados podem ser perdidos se os dados do navegador forem apagados; exporte backups.
- Não grava nem envia áudio; o laboratório de fala funciona sem microfone.
- Os estudos de caso incluem orientações de pesquisa, mas os resultados quantitativos não são inventados nem apresentados como comprovados. Verifique fontes primárias antes de usar alegações específicas.
- O conteúdo é uma base inicial de estudo e pode ser ampliado e aprofundado. Nem todas as aulas do currículo mestre estão escritas nesta primeira versão.

## Arquivos

- `index.html`: entrada do site.
- `assets/css/styles.css`: identidade visual e responsividade.
- `assets/js/app.js`: navegação e funcionalidades.
- `data/content.json`: trilhas, aulas, glossário e casos.
