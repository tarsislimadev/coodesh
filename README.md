# Node.js Challenge para a Coodesh

[Repositorio Coodesh](https://coodesh.com/)

Descrição completa em [README.old.md](./README.old.md)

## Task list

- [x] Utilizar o seu github pessoal para publicar o desafio. 

- [ ] O projeto back-end deverá ser desenvolvido usando em NodeJS

- [ ] Documentação para configuração do projeto em ambientes de produção (como instalar, rodar e referências a libs usadas)

- [x] Criar um banco de dados MongoDB usando Atlas: https://www.mongodb.com/cloud/atlas ou algum Banco de Dados SQL se não sentir confortável com NoSQL

- [ ] Criar uma REST API usando NodeJS com as melhores práticas de desenvolvimento.

- [ ] Integrar a API com o banco de dados criado para persistir os dados

- [ ] Recomendável usar Drivers oficiais para integração com o DB

- [ ] Desenvolver Testes Unitários

- [ ] `imported_t`: campo do tipo Date com a dia e hora que foi importado

- [ ] `status`: campo do tipo Enum com os possíveis valores draft, trash e published

- [ ] https://challenges.coode.sh/food/data/json/index.txt

- [ ] https://challenges.coode.sh/food/data/json/data-fields.txt

- [ ] Todos os produtos deverão ter os campos personalizados `imported_t` e `status`.

- [ ] Limitar a importação a somente 100 produtos de cada arquivo.

## API REST

- [ ] `GET /`: Detalhes da API, se conexão leitura e escritura com a base de dados está OK, horário da última vez que o CRON foi executado, tempo online e uso de memória.

- [ ] `PUT /products/:code`: Será responsável por receber atualizações do Projeto Web

- [ ] `DELETE /products/:code`: Mudar o status do produto para `trash`

- [ ] `GET /products/:code`: Obter a informação somente de um produto da base de dados

- [ ] `GET /products`: Listar todos os produtos da base de dados, adicionar sistema de paginação para não sobrecarregar o `REQUEST`.

## Opcionais

- [ ] **Diferencial 1** Front End con ReactJs, configurar um projeto web para listar os produtos cadastrados na REST API.

- [ ] **Diferencial 2** Configurar Docker no Projeto para facilitar o Deploy da equipe de DevOps

- [ ] **Diferencial 3** Configurar um sistema de alerta se tem algum falho durante o Sync dos produtos

- [ ] **Diferencial 4** Descrever a documentação da API utilizando o conceito de Open API 3.0

- [ ] **Diferencial 5** Escrever Unit Tests para os endpoints  GET e PUT do CRUD

- [ ] Deve conter o título de cada projeto

- [ ] Uma descrição de uma frase

- [x] Como instalar e usar o projeto (instruções)

- [ ] Não esqueça o [.gitignore](https://www.toptal.com/developers/gitignore)

## Stack

[Node.js](https://nodejs.org/en/)

[MongoDB](https://www.mongodb.com/)

[Nginx](https://nginx.org/)

[Docker (+ Docker Compose)](https://www.docker.com/)

## How to

### Development

```sh
bash env/pull.sh

bash env/install.sh

bash env/up.sh 
```

## License

[MIT](./LICENSE)
