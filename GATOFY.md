# Gatofy Launcher (fork de techgenius1/tvOS-Launcher)

Fork do tvOS Launcher (Apache-2.0) para uso com o Gatofy TV (`me.gatofy.tv`).

## Mudanças em relação ao original
- **Continue Watching ligado por padrão** (`cw_enabled`), para a fileira de "Continuar" e as sugestões
  que o Gatofy TV publica (Watch Next e canal de sugestões) aparecerem sem mexer em configurações.
- **Pedido de `READ_TV_LISTINGS` corrigido**: só é feito com a janela em foco e uma vez por processo
  (antes, um pedido descartado por um diálogo na frente marcava "já pedi" para sempre).
- **Atualizador** aponta para `glaujack/gatofy-launcher` (antes baixaria o APK do projeto original por cima)
  e a atualização automática vem desligada.

## Build
`source <env do toolchain>; bash build.sh` gera `build/tvos-home.apk` (chave de depuração local, não versionada).

## Instalação / launcher padrão
Instalar não troca o launcher. Ver "Make Home Screen" no app (ADB local, desativar o launcher nativo,
ajuste do botão Home por acessibilidade ou a tela de launcher padrão do Android).
