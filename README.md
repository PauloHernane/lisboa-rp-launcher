# Lisboa RP Launcher (Android)

Launcher mobile no estilo "Brasil Play Shox SAMP Mobile", adaptado para o servidor
LISBOA ROLEPLAY (144.217.64.5:8591).

## Telas do app
- **Login**: nick + senha (salvo no aparelho; conecte depois a um sistema real de contas)
- **Home**: botao JOGAR, status do servidor em tempo real (API samp-api), copiar IP, menu, novidades
- **Personagem**: nome RP, idade, historia, escolha de skin e emprego (salvo no aparelho)
- **Loja VIP**: planos Bronze, Prata e Ouro com botao de compra (redireciona ao site)
- **Regras**: principais regras do servidor
- **Ajustes**: conta conectada, servidor e sair da conta

## Como gerar o APK
1. Instale o Android Studio (gratuito): https://developer.android.com/studio
2. Abra esta pasta (File > Open > selecione a pasta lisboa-rp-launcher)
3. Aguarde a sincronizacao do Gradle (ele baixa o SDK automaticamente)
4. Menu Build > Build App Bundle(s) / APK(s) > Build APK(s)
5. O APK sai em: app/build/outputs/apk/debug/app-debug.apk

Para publicar na Play Store: Build > Generate Signed Bundle / APK (crie uma keystore).

## Personalizar
- IP e API: app/src/main/assets/launcher.html (variaveis IP e API)
- Planos e precos da loja: bloco "view-loja" no launcher.html
- Nome do app: app/src/main/res/values/strings.xml
- Icone: app/src/main/res/drawable/ic_launcher.xml
