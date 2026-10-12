# Brutal Brawl — protótipo Android

O projeto contém um protótipo web jogável e arquivos de configuração para criar um APK Android de teste usando GitHub Actions (compilação na nuvem).

## O que está incluído
- `www/index.html`: protótipo jogável com controles de toque, vida, cronômetro e adversário de IA simples.
- `package.json` e `capacitor.config.json`: configuração do Capacitor.
- `.github/workflows/android-apk.yml`: fluxo de trabalho que compila um APK de depuração e o publica como artefato para baixar.

## Como obter o APK usando apenas o celular
1. Baixe e extraia o ZIP.
2. Entre no GitHub pelo navegador do celular e crie um repositório novo chamado `brutal-brawl`.
3. Envie todos os arquivos e pastas deste projeto ao repositório, mantendo a pasta `.github/workflows/` e o arquivo `android-apk.yml`.
4. Abra a aba **Actions** do repositório e permita Actions se o GitHub pedir.
5. Abra o workflow **Gerar APK Android** e toque em **Run workflow**. Também inicia automaticamente ao enviar commits para `main`.
6. Quando a execução terminar com sucesso, abra a execução e baixe o artefato **Brutal-Brawl-APK-debug**. Dentro dele estará `app-debug.apk`.
7. Baixe o APK no celular e abra-o para instalar. Se o Android pedir, permita instalação de apps dessa origem.

## Limitações importantes
- Este pacote ainda não é um APK compilado; o APK só existirá após a execução bem-sucedida do workflow.
- O workflow usa GitHub Actions e depende de uma conta/repositório com Actions habilitado e cota disponível.
- Este é um protótipo inicial: o lutador é um desenho provisório em Canvas, não uma arte final baseada diretamente na fotografia. IA, balanceamento, animações e compatibilidade precisam de testes no aparelho.
- Para publicar na Play Store, será necessário preparar assinatura de lançamento e os requisitos da loja. Não compartilhe senhas ou chaves de assinatura em arquivos públicos.
