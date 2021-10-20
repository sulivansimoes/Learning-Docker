Referência para escrita do readme.md :point_right: [Documentaçao Oficial](https://docs.docker.com/reference/) :point_left:

# Comandos básicos

## Verificando a lista de containers

Para visualizar a lista de containers de um determinado Docker host utilizamos o comando ```docker ps```.
Esse comando é responsável por mostrar todos os containers, mesmo aqueles não mais em execução (quando passado ```-a```).

- ``` docker container list ``` <parâmetros>  
- ``` docker ps ``` <parâmetros>

| Parâmetro     | Parâmetro              |                |
| ------        | ------                 | ------         |
| **Nome**      | **taquigrafia**        | **Explicação** |
| ```-all```    | ```-a```               | *Lista todos os containers, inclusive os desligados*      |
| ```--latest```| ```-l```               | *Lista os últimos containers, inclusive os desligados*    |
| ```--quiet``` | ```-q```               | *Lista apenas os ids dos containers*  |

## Verificando lista de imagens

Para visualizar a lista de imagens de um determinado Docker host utilizamos o comando.

- ``` docker image ls ``` <parâmetros>  

| Parâmetro     | Parâmetro              |                |
| ------        | ------                 | ------         |
| **Nome**      | **taquigrafia**        | **Explicação** |
| ```--all```   | ```-a```               | *Mostrar todas as imagens (o padrão oculta as imagens intermediárias*      |

## Iniciando containers parados
Para iniciar um ou mais contêineres parados utilizamos o comando 

- ```docker start```<id_container>
- ```docker start```<name_container>

## Parando containers em execução
Para um ou mais contêineres em execução

- ```docker stop```<id_container>
- ```docker stop```<name_container>

## Deletando containers

Para deletar containers do Docker host utilizamos o comando

- ``` docker rm ``` <id_container>
- ``` docker rm ``` <name_container>

| Parâmetro     | Parâmetro              |                |
| ------        | ------                 | ------         |
| **Nome**      | **taquigrafia**        | **Explicação** |
| ```--force``` | ```-f```               | *Força a remoção de um contêiner em execução (usa SIGKILL)* ``` docker rm -f ``` <id_container> |

## Deletando imagens

Para deletar imagens do Docker host utilizamos o comando

- ``` docker rmi ``` <id_image>
- ``` docker rmi ``` <name_image>

| Parâmetro     | Parâmetro              |                |
| ------        | ------                 | ------         |
| **Nome**      | **taquigrafia**        | **Explicação** |
| ```--force``` | ```-f```               | *Força remoção da imagem do docker* ``` docker rmi -f ``` <id_image>      |