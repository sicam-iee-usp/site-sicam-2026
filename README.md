# Site do SICAM 🌎

Este repositório contém o código do **site do SICAM** (Simpósio Interdisciplinar de Ciência Ambiental), evento organizado por discentes do PROCAM-IEE-USP.

🔗 **Site no ar:** <https://sicam.com.br/>

> 💡 **Você não precisa saber programar para ajudar!** Abaixo explicamos, passo a passo, duas formas de contribuir — da mais simples para a mais avançada. Escolha a que for mais confortável para você.

---

## 🙋 Opção 1 — Pedir uma mudança (o jeito mais fácil)

Não precisa de nada técnico. É só **descrever o que você quer mudar** e alguém da equipe faz por você.

1. Acesse a aba de **[Issues](https://github.com/sicam-iee-usp/site-sicam-2026/issues)** (é a nossa "lista de tarefas / pedidos").
2. Veja se **já existe** um pedido parecido na lista. Se existir, você pode comentar nele.
3. Se não existir, clique no botão verde **"New issue"**.
4. Escreva um **título curto** e, na descrição, conte com o máximo de detalhes:
   - **Qual página** deve mudar (ex.: "Equipe", "Submissão");
   - **O que** deve ser alterado (texto novo, corrigir uma data, trocar uma imagem, etc.).
5. Clique em **"Submit new issue"**. Pronto! 🎉

> ✉️ Quando alguém responder ou marcar você numa issue, você recebe um **e-mail**. Pode **responder direto pelo e-mail** que a sua mensagem vira um comentário automaticamente.

---

## ✏️ Opção 2 — Editar uma página você mesma(o) pelo site do GitHub

Também **não precisa instalar nada nem saber programar** — dá para editar tudo pelo navegador.

> 🔑 **Pré-requisito:** ter acesso de contribuidor ao repositório. Se você ainda não tem, peça para a [Beatriz Milz](https://github.com/beatrizmilz).

**Passo a passo:**

1. Abra o arquivo da página que você quer mudar (use o **mapa de páginas** mais abaixo para saber qual é).
2. Clique no ícone de **lápis ✏️** ("Edit this file"), no canto superior direito do arquivo.
3. Faça as alterações no texto.
4. Role até o final da página e clique no botão verde **"Commit changes..."**.
5. Escreva um resuminho do que você mudou e confirme em **"Commit changes"**.
6. **Pronto!** Em poucos minutos o site se atualiza sozinho. ✅

### ⏱️ O que acontece depois que eu salvo?

O site é **gerado automaticamente** sempre que alguém salva uma mudança. Depois de salvar, espere **cerca de 2 a 5 minutos** e atualize a página no navegador (`https://sicam.com.br`). Você **não precisa fazer mais nada**.

### 📝 Sobre os arquivos `.qmd`

As páginas do site são arquivos que terminam em **`.qmd`**. Por dentro, eles são quase texto comum, com algumas marcações simples:

| Para fazer isso | Você escreve |
|-----------------|--------------|
| **negrito** | `**negrito**` |
| *itálico* | `*itálico*` |
| Um título de seção | `## Título` |
| Um link | `[texto do link](https://endereco.com)` |
| Uma lista | `- item` (um por linha) |

Não tem problema errar — nada quebra o site de forma permanente, e sempre dá para voltar atrás. Na dúvida, use a **Opção 1** (abrir uma issue).

---

## 🗺️ Mapa de páginas — qual arquivo muda qual página

| Página no site | Arquivo para editar |
|----------------|---------------------|
| Página inicial | [`index.qmd`](index.qmd) |
| Sobre o SICAM | [`sobre-o-evento.qmd`](sobre-o-evento.qmd) |
| Equipe organizadora | [`equipe.qmd`](equipe.qmd) |
| Edições anteriores | [`edicoes-anteriores.qmd`](edicoes-anteriores.qmd) |
| Grupos temáticos | [`grupos-tematicos.qmd`](grupos-tematicos.qmd) |
| Submissão de trabalhos | [`submissao.qmd`](submissao.qmd) |
| Submissões aprovadas | [`submissoes-aprovadas.qmd`](submissoes-aprovadas.qmd) |
| Programação | [`programacao.qmd`](programacao.qmd) |
| Informações gerais | [`informacoes.qmd`](informacoes.qmd) |
| Menu, rodapé e título do site | [`_quarto.yml`](_quarto.yml) *(mais técnico)* |

### 📰 Aba "Novidades" (posts)

A aba **Novidades** da página inicial é montada pelos arquivos dentro da pasta [`posts/`](posts/). Cada arquivo é uma novidade. Para publicar uma nova, crie um arquivo `.qmd` nessa pasta (ou peça pela **Opção 1**).

### 🖼️ Imagens

As imagens ficam na pasta [`img/`](img/). Para trocar ou adicionar uma imagem, o mais simples é abrir uma **issue (Opção 1)** anexando o arquivo.

---

## 🆘 Precisa de ajuda ou de acesso?

Fale com a [**Beatriz Milz**](https://github.com/beatrizmilz). Na dúvida sobre qualquer coisa, abra uma [issue](https://github.com/sicam-iee-usp/site-sicam-2026/issues) — alguém vai te ajudar. 🙌

---

## 📖 Glossário rápido

- **Repositório (repo):** a "pasta" online onde ficam todos os arquivos do site.
- **Issue:** um pedido ou tarefa na nossa lista (Opção 1).
- **Commit:** salvar uma alteração. Cada commit fica registrado no histórico.
- **`.qmd`:** o tipo de arquivo que gera cada página do site.
- **Renderizar / build:** o processo automático que transforma os arquivos `.qmd` no site que aparece no navegador.

---

## 🔧 Informações técnicas (para quem desenvolve)

- O site é feito com **[Quarto](https://quarto.org/)** (engine `knitr`, usa R em algumas páginas).
- A cada `push` na branch `main`, um **GitHub Actions** ([`.github/workflows/render.yml`](.github/workflows/render.yml)) renderiza o site na pasta `docs/` e publica via **GitHub Pages** no domínio `sicam.com.br`.
- **Edições anteriores** ficam cada uma em seu próprio repositório e subdomínio: [`2024.sicam.com.br`](https://2024.sicam.com.br), [`2022.sicam.com.br`](https://2022.sicam.com.br), [`2021.sicam.com.br`](https://2021.sicam.com.br).
- **Rodar localmente** (opcional): instale o [Quarto](https://quarto.org/docs/get-started/) e o R, então use `quarto preview` para visualizar ou `quarto render` para gerar o site.
