# FYAH Control — projeto Android

Aplicativo interno para organizar encomendas, produção, clientes e financeiro da FYAH. Não possui loja virtual.

## Estrutura
- `app/`: aplicativo Android.
- `app/src/main/assets/index.html`: interface do aplicativo.
- `.github/workflows/build-apk.yml`: compilação automática do APK pelo GitHub Actions.

## Gerar o APK pelo GitHub usando o celular
1. Envie **todo o conteúdo desta pasta** para a raiz do repositório `fyah-control`, preservando as pastas.
2. Abra a aba **Actions** no GitHub.
3. Se necessário, habilite GitHub Actions para o repositório.
4. Execute `Gerar APK FYAH Control` em **Run workflow**, ou faça um novo commit (o workflow também roda ao enviar alterações para `main`).
5. Quando o processo terminar com sucesso, abra a execução e baixe o artefato `FYAH-Control-APK`.
6. Extraia o arquivo baixado. Dentro estará `app-debug.apk`. Instale no Android.

## Observações
- Os dados são salvos localmente no aparelho, no armazenamento do WebView.
- Faça backup periódico pelo botão **Exportar backup** dentro do aplicativo.
- Este projeto usa Android Gradle Plugin 8.7.3, Gradle 8.9 e Java 17.
