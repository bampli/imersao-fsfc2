# Imersão Full Stack & FullCycle - Codelivery

## Descrição

Repositório do front-end feito com React.js (Front-end)

**Importante**: A aplicação do Apache Kafka, Golang e Nest.js deve estar rodando primeiro.

## Configurar /etc/hosts

A comunicação entre as aplicações se dá de forma direta através da rede da máquina.
Para isto é necessário configurar um endereços que todos os containers Docker consigam acessar.

Acrescente no seu /etc/hosts (para Windows o caminho é C:\Windows\system32\drivers\etc\hosts):
```
127.0.0.1 host.docker.internal
```
Em todos os sistemas operacionais é necessário abrir o programa para editar o *hosts* como Administrator da máquina ou root.

## Rodar a aplicação

Execute os comandos:

```
docker-compose up
```

Acessar http://localhost:3001.

### Para Windows 

Lembrar de instalar o WSL2 e Docker. Vejo o vídeo: [https://www.youtube.com/watch?v=usF0rYCcj-E](https://www.youtube.com/watch?v=usF0rYCcj-E) 

Siga o guia rápido de instalação: [https://github.com/codeedu/wsl2-docker-quickstart](https://github.com/codeedu/wsl2-docker-quickstart) 

### Npm Install

#### react-frontend
- React.js: Tempo real com websockets e geolocalização[video]](https://www.youtube.com/watch?v=QyG6vI8iTEk)
    npm install @material-ui/core --save
    npm install google-maps --save
    npm install @types/lodash --save
    npm install notistack --save
    npm install @material-ui/icons --save
    npm install @nestjs/websockets --save
    npm install @types/socket.io --save-dev
    npm install @types/socket.io-client socket.io-client@2.4.0 --save

#### nest-api
- Desenvolvimento de APIs com Nest.js [video](https://www.youtube.com/watch?v=IPlLwBXb8G0)
    npx @nestjs/cli new nest-api
    npm install mongoose @nestjs/mongoose --save
    npm install class-transformer class-validator --save
    npm install swagger-ui-express @nestjs/swagger --save