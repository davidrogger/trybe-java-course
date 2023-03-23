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

