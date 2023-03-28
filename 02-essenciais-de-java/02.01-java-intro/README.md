# Intro ao Java

Mais de 25 anos, é a linguagem de programação mais utilizada ao redor do mundo, está entre os primeiros há muito tempo nos indices de populariedade. É caracterizado por sua portibilidade, sendo possivel sua compilação para os mais diversos tipos de aparelhos, é a linguagem mais usada para criação de aplicativos android e sua retrocompatibilidade possibilita que suas versões atuais continuam reconheciendo códigos feitos em versões antigas.

# Instalando oracle java 11 (Debia e Ubuntu e derivados)

Aplique atualizações ao sistema e instale o java development kit versão 11.

```
sudo apt update
sudo apt install openjdk-11-jdk
```

Após a instalação verifique a versão do java, para verificar se a instalação ocorreu com sucesso.
```
java -version

openjdk version "11.0.18" 2023-01-17
OpenJDK Runtime Environment (build 11.0.18+10-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.18+10-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)
```

E verifique a versão do compilador do java

```
javac -version
```

# Removendo a instalação do java

Usando o comando:
```
sudo apt remove openjdk-11*
```

Como são instalados outros modulos juntamente com o jdk, é necessário usar o coringa no final do remove, para realizar a remoção de todas instalações relacionadas ao opendk-11.

# Instalando Eclipse

Eclipse é o IDE(Integrated Development Environment), ambiente de desenvolvido onde serão desenvolvidas as aplicações usando o java. Eclipse também tem suporte a outras linguagem por meio de plugins como [C](https://www.youtube.com/watch?v=6mUCcsnCn08), [C++](https://www.youtube.com/watch?v=AQdABlihlGs), [PHP](https://www.youtube.com/watch?v=AqDj3OSV0mM), [ColdFusion](https://pt.wikipedia.org/wiki/ColdFusion), [python](https://www.youtube.com/watch?v=uOgDa1rlqjE), [scala](https://www.devmedia.com.br/conheca-a-linguagem-scala/32850) e [kotlin](https://www.youtube.com/watch?v=BfjRYBN7Ur8).

- Acessando a área de [downloads do eclipse](https://www.eclipse.org/downloads), deve-se procurar pela versão Enterprise Java and Web Developers.

Basta descompactar o arquivo tar, e acessar a posta, ao executar o arquivo eclise na pasta, o eclise será aberto, para adicionar o eclipse à biblioteca do ubuntu deve-se criar um arquivo ao seguinte caminho:
```
touch ~/.local/share/applications/Eclipse.desktop
```

Abrindo o editor nesse arquivo, deve ser adicionado as seguintes configurações:
```
[Desktop Entry]
Comment=Eclipse
Terminal=false
Name=Eclipse
Exec=/caminho/para/versao/eclipse/eclipse
Type=Application
Icon=/caminho/para/icone/eclipse/icon.xpm
StartupWMClass=Eclipse
```

O arquivo descompactado deve ser alocado em um local apropriado para permanecer lá, para a inicialização do eclipse.

Para tornar o arquivo executável:
```
chmod a+x ~/.local/share/applications/Eclipse.desktop
```

Ao buscar por eclise na área de busca do ubuntu, o eclipse ja será encontrado.

# Integrando o Docker ao Eclipse

É necessário baixar um plugin, acessando a parte de "help" e "Eclipse Marketplace".
Deve procurar por `Jboss-tools`.

Aguarde a conclusão da instalação e a solicitação de reinicio do eclipse. Acessando o open perspective no canto superior direito, acessando Docker tooling, demonstra o sucesso na integração com docker.

# Integrando o Git ao Eclipse

Seguindo os mesmos passos anteriores buscando por EGit.

# Nota Adicional durante a execução do Eclipse

Por estar usando o WSL2 foi apontado um erro com relação ao swt gtk 4, realizando a instalação do libswt gtk os erros pararam:

```
sudo apt update
sudo apt install libswt-gtk-4-jni
```

# Criando um "Hello World"

1. Acessando no eclipse na opção `File`, `new` e `project`;
2. Escolhendo o tipo do projeto como `Java Project`;
3. Definir um nome para o projeto. Por padrão é criado no diretório de trabalho. É possivel alterar o local.
4. Essa janela pode-se apenas avançar, e finalizar, definindo para abrir em modo perspective.

Agora observando ao clicar no canto esquerdo, nota-se uma janela com dois quadrados, ao passar o mouse é indicado como restore, ao clicar nele, a aba com o nome do projeto é apresentada com a área de trabalho do projeto.

Acessando o nome do projeto, no diretório SRC, é necessário criar um pacote.

1. Clicando com o botão direito, acessando new e package.
2. Será solicitado um nome para o pacote.
3. O nome do package pode ser o nome que desejar, desde que seja em letra minuscula, e seu espaçamento seja realizado com o ponto ".".

## Criando uma classe no pacote

Clicando com o botão direito no pacote criado, acessando new e class, é solicitado necessário definir as configurações iniciais da classe.

agora no pacote trybe.main, criando uma class chamada "HelloWorld", onde o method main, apenas escreve no console "Hello World".

```
package trybe.main

public class HelloWorld {
  
  public static void main(string[] args) {
    System.out.println("Hello World");
  }

}
```