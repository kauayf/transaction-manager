
# 🔥 Gestão de Transações 🔥


 # ✅ Transaction-Manager
   🚀 API Para gestão de transações (Entrada, Saída, Balanço) 🚀


##  ✅ Features

- [x] Permitir que uma transação seja criada, e retorne um ```JSON``` com a transação criada.

- [x] Ao criar uma nova transação com uma categoria que não existe, seja criada e inserida no campo ```category_id``` da transação com o ```id``` que acabou de ser criado.

- [x] Ao criar uma nova transação com uma categoria que já existe, seja atribuído ao campo ```category_id``` da transação com o ```id``` dessa categoria existente, não permitindo a criação de categorias com o mesmo ```title```.

- [x] Retornar um array de objetos contendo todas as transações junto ao balanço de ```income, outcome e total``` das transações que foram criadas até o momento

- [x] Não deve permitir que uma transação do tipo outcome extrapole o valor total que o usuário tem em caixa (total de income), retornando uma resposta com código ```HTTP 400``` e uma mensagem de erro no seguinte formato: ```{ error: string }```.

- [x] Deve permitir que exclua uma transação, e ao fazer a exclusão, ele retorne uma resposta vazia, com ```status 204```

- [x] Deve permitir que seja importado um arquivo csv, contendo o seguinte modelo. Com o arquivo importado, deve permitir que seja criado no banco de dados todos os registros e categorias que estavam presentes nesse arquivo, e retornar todas as transactions que foram importadas.

## ✅ Demonstração da aplicação

### CRIAÇÃO, LISTAGEM, VALIDAÇÃO
<h1 align="center">
  <img src=src/assets/transaction_manager_1.gif />
</h1>

### IMPORTAÇÃO DE ARQUIVO CSV
<h1 align="center">
  <img src=src/assets/transaction_manager_2.gif />
</h1>


## ✅ Tecnologias utilizadas

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [TypeScript ⚡](https://www.typescriptlang.org/)
- [PostGreSQL ⚡](https://www.postgresql.org)
- [Node.js ⚡](https://nodejs.org/en/)
- [Insomnia ⚡](https://insomnia.rest/products/insomnia)
- [TypeORM ⚡](https://typeorm.io/)
- [ParseCSV ⚡](https://csv.js.org/parse/)
- [FS ⚡](https://nodejs.org/api/fs.html)
- [Express ⚡](https://expressjs.com/pt-br/)
- [Multer ⚡](https://www.npmjs.com/package/multer)
- [UUID ⚡](https://www.npmjs.com/package/uuid)


#### Clonando o projeto
```sh
$ git clone https://github.com/kauayf/transaction-manager.git
$ cd transaction-manager
```

#### Iniciando Testes
```sh
$ yarn test
```

#### Instalando dependências, iniciando migrations e API
 1° - ```$ yarn``` - "Dependencias do projeto"

 2° - ```$ yarn typeorm migration:run``` - "Criando as migrations no PostGreSQL"

 3° - ```$ yarn dev:server``` - "inicia o backend"


#### Iniciando o Frontend
```sh
Novidades em breve ... 🚀
```


### :memo: Licença

Este projeto é desenvolvido sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para saber mais detalhes.

<p align="center" style="margin-top: 20px; border-top: 1px solid #eee; padding-top: 20px;">Feito com 💙 by <strong>  🌠 Kauay Felipe 🌠 </strong> </p>


[![The MIT License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)](http://github.com/jvictorfarias/gobarber/LICENSE.md)
