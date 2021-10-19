Referência para escrita do readme.md [Documentaçao Oficial](https://docs.docker.com/reference/). :v:

# Comandos básicos

## Verificando a lista de containers

Para visualizar a lista de containers de um determinado Docker host utilizamos o comando ```docker ps```.
Esse comando é responsável por mostrar todos os containers, mesmo aqueles não mais em execução.

- ``` docker container list ``` <parâmetros>  
- ``` docker ps ``` <parâmetros>

| Parâmetro        | Explicação      | 
| ------|-----|
| -a  	| *Lista todos os containers, inclusive os desligados*      |
| -l  	| *Lista os últimos containers, inclusive os desligados*    |
| -n  	| *Lista os últimos N containers, inclusive os desligados*  |
| -q  	| *Lista apenas os ids dos containers, ótimo para utilização em scripts*  |

## Deletando containers

Para deletar containers do Docker host utilizamos o comando

- ``` docker rm ``` <id_container>
- ``` docker rm ``` <name_container>

## Deletando imagens

Para deletar imagens do Docker host utilizamos o comando

- ``` docker rmi ``` <id_image>
- ``` docker rmi ``` <name_image>