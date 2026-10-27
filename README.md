# Capinanças — Política de Privacidade

Página pública da política de privacidade do app **Capinanças** (Capivara
Studios), pronta para o **GitHub Pages**.

- `index.html` — página completa (pt-BR/en, responsiva, autocontida)
- `privacy-policy.md` — a mesma política em Markdown
- `.nojekyll` — evita o processamento do Jekyll no Pages

## Publicar no GitHub Pages

1. Crie um repositório **público** chamado `capinancas-privacy` no GitHub.
2. Envie estes arquivos:

   ```bash
   git add .
   git commit -m "docs: política de privacidade do Capinanças"
   git push origin master
   ```

3. No GitHub: **Settings → Pages → Build and deployment**
   - **Source:** Deploy from a branch
   - **Branch:** `master` · **Folder:** `/ (root)` → **Save**

4. Em cerca de 1 minuto a URL fica:
   `https://lasantos704.github.io/capinancas-privacy/`

5. Use essa URL no **Google Play Console** em
   **Conteúdo do app → Política de privacidade**.

> No plano gratuito, o repositório precisa ser **público** para usar o GitHub
> Pages.

## Atualizar

**A fonte desta página é o repositório do app**, onde a política é escrita junto
do código que trata os dados:

- `capinancas-app/docs/index.html` — a página (mesmo conteúdo, mesma marca);
- `capinancas-app/store/privacy-policy.md` — a política em Markdown.

Ali o `docs/index.html` é vigiado por `src/theme/mirror.test.ts`, que falha se as
cores da página divergirem do tema do app (`npm run test`). Mude lá, depois copie
para cá e faça commit + push — o GitHub Pages republica em ~1 minuto:

```bash
cp ../capinancas-app/docs/index.html index.html
cp ../capinancas-app/store/privacy-policy.md privacy-policy.md
```

Editar só este repo é o que deixa as duas versões diferentes (aconteceu com a
fonte da marca, em 23/10/2026).

## Pré-visualizar localmente

```bash
npx serve .
```

Ou abra `index.html` diretamente no navegador.

## Contato

contato.capistudios@gmail.com
