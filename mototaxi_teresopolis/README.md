# BR Moto Táxi Teresópolis

Aplicativo Android com interface em português para solicitação de moto-táxi e entregas em Teresópolis, RJ.

## Recursos
- Interface responsiva para moto-táxi e entregas.
- Tarifa mínima de R$ 8,00 e tarifa de R$ 2,00 por quilômetro, conforme configuração atual.
- Busca de endereços pelo Nominatim/OpenStreetMap.
- Estimativa de distância e preço usando o serviço público OSRM.
- Preparação do pedido para envio pelo WhatsApp.
- Abertura da rota no Google Maps.
- Aplicativo Android baseado em WebView.

## Estrutura do projeto
- `app/src/main/assets/index.html`: interface e funcionalidades web.
- `app/src/main/java/br/com/mototaxi/teresopolis/MainActivity.java`: atividade Android.
- `app/src/main/AndroidManifest.xml`: configuração do aplicativo.
- `publicacao/BR-Moto-Taxi-Teresopolis.apk`: APK compilado disponível na pasta de publicação.

## Como compilar
1. Instale o Android Studio e os componentes do Android SDK necessários.
2. Abra a pasta `mototaxi_teresopolis` no Android Studio.
3. Aguarde a sincronização do Gradle.
4. Compile usando **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

Também é possível compilar pelo terminal, com o Gradle e o Android SDK configurados:

gradle assembleDebug
O APK de depuração será gerado em app/build/outputs/apk/debug/app-debug.apk.

## Observações importantes
- A busca de endereços e o cálculo de rotas exigem internet.
- Nominatim e OSRM são serviços públicos e podem apresentar indisponibilidade.
- Os valores são estimativas e podem variar conforme as condições da viagem.
- O pedido é preparado para o WhatsApp, mas o usuário precisa confirmar o envio.
- Teste o aplicativo em aparelhos reais antes de distribuí-lo.
