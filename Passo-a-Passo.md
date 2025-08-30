# Passo a passo para rodar o Calisto Lobinhosii com Docker e Docker Compose

## 1. Carregar a imagem Docker

Execute o comando abaixo para importar a imagem localmente:

```bash
docker load -i calisto-lobinhosii.tar
```

## 2. Rodar o container manualmente

Se quiser rodar diretamente, use:

```bash
docker run -d -p 8080:80 calisto-lobinhos
```

## 3. Rodar com Docker Compose

1. Certifique-se de que o arquivo `docker-compose.yml` está na raiz do projeto.
2. Execute:

```bash
docker-compose up -d
```

## 4. Testar o funcionamento

Acesse `http://localhost:8080` no navegador para verificar se o serviço está rodando.

## 5. Parar o serviço

Para parar e remover os containers:

```bash
docker-compose down
```
