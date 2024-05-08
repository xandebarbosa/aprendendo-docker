No windows
Instalar o docker e iniciar o programa.

docker --version
docker run hello-world

Vamos lançar um container com base na imagem do ubutun 24.04
*podemos ver várias imagens disponíveis no site: hub.docker.com

executar o comando: docker run -ti ubuntu:22.04
*ti = para podemos integir o "t" serve para lançar um falso terminal, "i" para interagir.

Para visualizar os container em execução: docker ps

Agora vamos lançar uma imagem customizada, uma imagem para guardar a minha aplicação.

docker file é um arquivo onde especifico como vai ser a minha imagem

Criar o arquivo Dockerfile_ubuntu, adicionar o texto FROM ubuntu.24.04 RUN mkdir teste1

Para construir a imagem utilizamos o comando: docker build -f Dockerfile -t aprendendo-docker .

*aprendendo-docker = nome da imagem
* . = passando o contexto, diretorio onde vai encontrar os arquivos

Para rodar:  docker run -ti aprendendo-docker

Para ver o conteúdo da pasta digitar no terminal o comando: ls


PAREI NO MINUNTO 00:27:06

BOOTCAMP IMERSÃO AWS