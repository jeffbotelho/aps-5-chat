# APS - 5* Semestre - Arq. Redes

Atividade Prática Supervisionada - **APS** do curso de Ciência da Computação **CC**, 5º Semestre.

Disciplina vinculada: Redes de Computadores - **RC**.

**Prof. Orientador:** Hebert Silva.

Universidade Paulista - **UNIP**

## Tema
**"DESENVOLVIMENTO DE UMA FERRAMENTA PARA COMUNICAÇÃO EM REDE"**

## Proposta do trabalho

Criar uma aplicação que permita que duas ou mais pessoas possam se comunicar em uma rede, utilizando o protocolo TCP.

**Caso de uso:** a Secretaria do Estado do Meio Ambiente deseja saber quais atividades industriais estão gerando poluição do Rio Tietê desde sua nascente em Salesópolis (SP) até a sua passagem pela região da grande São Paulo.  Para tal ela precisa trocar informações das equipes de inspetores treinados e capacitados que estarão se revezando dentro de cada indústria, controlando os processos e passando informações online para a Secretaria.

### Objetivo

Desenvolver uma aplicação web broadcast que possibilite a comunicação entre os inspetores e a Secretaria por meio de mensagens instantâneas de texto.


# Instalação

Acesse o local onde deseja baixar o projeto via terminal e execute o comando:

```git clone https://github.com/jeffbotelho/aps-5-chat.git```

Logo após, acesse o projeto:

`cd monitoratiete`

Dentro do projeto, onde está o arquivo `pom.xml`, execute o comando:

`mvn clean compile package`

Será gerado um arquivo `.war` dentro do diretório `/target`

### Nota: é necessário que o Apache Tomcat esteja instalado em seu computador

Caso não tenha instalado, baixe o [Tomcat](https://tomcat.apache.org/download-90.cgi)

Baixe o arquivo compactado compatível ao seu Sistema Operacional.

> **Nota:** Não baixe a versão executável.

Após o download descompacte-o em uma pasta `tomcat`


#### Implantando o WAR no Tomcat

Para que nosso arquivo WAR seja implantado e executado no Tomcat, precisaremos concluir as seguintes etapas:

1. Copie o arquivo _WAR_ de `target/monitoratiete.war` para a pasta `tomcat/webapps/`
2. De um terminal, navegue até a pasta _tomcat/bin_ e execute
    1.  `catalina.bat run` (no Windows)
    2.  `./catalina.sh run` (em sistemas baseados em Unix)
3.  Vá para _http://localhost:8080/monitoratiete_

Esta foi uma configuração rápida do Tomcat, portanto, verifique o guia de [instalação do Tomcat](https://www.baeldung.com/tomcat) para obter um guia de configuração completo. Há também maneiras adicionais de [implantar um arquivo WAR no Tomcat](https://www.baeldung.com/tomcat-deploy-war) .


## Ferramentas e Tecnologias
- [Java](https://docs.oracle.com/en/java/)
 - [Maven](https://maven.apache.org/guides/)
- [SpringBoot](https://spring.io/projects/spring-boot)
- [JSR 356](https://www.oracle.com/technical-resources/articles/java/jsr356.html)
- [HTTP](https://devdocs.io/http/)

## Melhorias

:white_check_mark: Enviar mensagens

:ballot_box_with_check: Enviar Emoji

:ballot_box_with_check: Enviar arquivos

:ballot_box_with_check: Autenticação

## Integrantes

- [Jefferson](https://github.com/jeffbotelho)
