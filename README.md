# FlutterAlura
Aprofundando os conhecimentos em flutter

# Instalação do Flutter
Instalando o Flutter no Windows
A instalação no Windows normalmente é bem rápida, pois necessitamos apenas do Git instalado e do próprio SDK do Flutter (que já tem o SDK do Dart embutido).

Para instalar e configurar o Flutter no Windows, veja os passos a seguir:

1 - O Flutter depende do Git para funcionar. Então, é necessário que o Git esteja instalado na máquina antes de instalarmos o Flutter. Para isso, basta baixar o cliente do Git para Windows da sua página oficial. A instalação é no estilo Avançar> Avançar> Concluir. Quando o download for concluído, basta clicar no instalador do Git para que o processo de instalação seja iniciado.

2 - Baixe o arquivo zip da última versão do Flutter. Esse arquivo pode ser encontrado na página oficial do Flutter, dentro da seção “Get the Flutter SDK”. O nome do arquivo normalmente é flutter_windows_x.x.x-stable.zip, no qual as letras “x” são os números da versão mais atual disponível.

3 - Extraia o arquivo zip com o Flutter SDK para uma pasta onde não sejam necessários privilégios de administrador. A documentação do Flutter recomenda que o SDK seja extraído para C:\flutter.

4 - Para utilizarmos o Flutter CLI (interface de linha de comandos) diretamente em qualquer linha de comando, os seguintes passos são necessários:

Vá em Painel de Controle > Contas de usuário > Alterar as variáveis do meu ambiente.

Na seção de variáveis de ambiente de usuário, procure a variável chamada “Path”.

Adicione à variável “Path” o caminho para a pasta C:/flutter/bin. Não se esqueça de separar a nova entrada das entradas pré-existentes com um ponto e vírgula (;).

Reinicie o Windows.

Abra uma instância do git bash ou cmd e digite o comando Flutter. O help do Flutter deve ser exibido.

5 - E por último, mas não menos importante, execute em uma linha de comando do Windows o comando flutter doctor, para que ele dê o diagnóstico completo e informe se a instalação foi realizada corretamente. Caso ainda haja pendências, ele dirá quais são e como resolvê-las.

# Instalando o Flutter no Linux
A instalação no Linux normalmente é bem rápida para quem tem o hábito de trabalhar com a linha de comandos com a linha de comandos. Necessitamos apenas do Git instalado e do próprio SDK do Flutter (que já tem o SDK do Dart embutido).

Para instalar e configurar o Flutter no Linux (Synaptics, Ubuntu ou Debian), veja os passos a seguir:

1 - O Flutter depende do Git para funcionar. Para isso, instale o Git através de seu gerenciador de pacotes por meio do comando apt-get install git-all.

2 -Verifique se sua distribuição Linux é 64 bits. O Flutter só funciona em sistemas operacionais de 64 bits.

3 - Baixe a última versão do Flutter SDK para Linux. O SDK pode ser baixado em sua página oficial na seção “Get the Flutter SDK”.

4 - Extraia o Flutter para uma pasta que não exija elevação de privilégios. A documentação recomenda que o Flutter SDK seja extraído para uma pasta chamada “flutter” na raiz do seu usuário.

5 - Adicione o Flutter às variáveis de ambiente com o comando export PATH=pwd/flutter/bin:$PATH em uma instância do Terminal. Porém, este export funcionará apenas enquanto o terminal estiver aberto. Uma maneira de configurar definitivamente no path do Linux está no artigo Update your path da documentação do Flutter.

6 - Rode o comando ´flutter´ no terminal. O help do Flutter CLI deve ser exibido. E por último, mas não menos importante, execute em uma linha de comandos do seu Linux o comando flutter doctor para que ele dê o diagnóstico completo se a instalação foi realizada corretamente. Caso ainda haja pendências, ele dirá quais são e como resolvê-las.

# Instalando o Flutter no macOS
O processo de instalação do Flutter no macOS é bastante similar ao do Linux.

A instalação no macOS normalmente é bem rápida para quem está habituado(a) com a linha de comandos. Necessitamos apenas do Git instalado e do próprio SDK do Flutter (que já tem o SDK do Dart embutido).

1 - O Flutter depende do Git para funcionar. Para isso, instale o Git através de seu gerenciador de pacotes (utilizaremos aqui o homebrew) por meio do comando brew install git.

3 - Baixe a última versão do Flutter SDK para macOS. O SDK pode ser baixado em sua página oficial na seção “Get the Flutter SDK”.

4 - Extraia o Flutter para uma pasta que não exige privilégios de administrador. A documentação recomenda que o Flutter SDK seja extraído para uma pasta chamada “flutter” na raíz do seu usuário.

5 - Atualize o PATH da máquina para que este aponte para o Flutter SDK. Para isso, basta rodar o comando export PATH=pwd/flutter/bin:$PATH em uma instância do Terminal. Este export funcionará apenas enquanto o terminal estiver aberto. Uma maneira de configurar definitivamente no path do macOS está no artigo Update your path da documentação do Flutter.

6 - Rode o comando ´flutter´ no terminal. O help do Flutter CLI deve ser exibido. E por último, mas não menos importante, execute em uma linha de comandos do seu macOS o comando flutter doctor para que ele dê o diagnóstico completo se a instalação foi realizada corretamente. Caso ainda haja pendências ele dirá quais são e como resolvê-las.

# Configurando plugin do Flutter no Intellij Idea

1 - Abra o Intellij Idea. 2 - Na aba do lado esquerdo chamada "Plugins", selecione a aba superior "Marketplace". Pesquise primeiro "Dart" e instale. Depois repita o processo pesquisando por "Flutter" e instalando a extensão do Flutter.

3 - Feche o Intellij Idea, vá para a linha de comandos e navegue até uma pasta qualquer da sua máquina, na qual você deseja criar um projeto Flutter. Feito isso, dê ao Flutter o comando flutter create my_app.

4 - Abra a pasta my_app com o Intellij Idea e verifique se o projeto foi reconhecido como um projeto Dart/Flutter e se é possível pressionar o botão de play na parte superior da tela. Caso seja possível, o Flutter vai rodar o seu aplicativo no emulador Android.


# Android studio
1 - Habilite "Android SDK Command-line Tools"
    - No projeto onde foi criado o flutter
    - rode o comando "flutter doctor" para ver o que está faltando.

2 - Atualize o android SDK build.

3 - no adv, la em cima atualizar "plataform-tools-adv".

4 - Atualize Android SDK Plataform-Tools.

5 - rode o comando "flutter doctor --android-licenses" dentro do projeto para criar as licensas necessário, via linha de comando.

6 rode o comando "flutter run --enable-software-rendering" caso necessário apra ele renderizar o aplicativo.

