# API de Inserção de CEPs
Este repositório contém uma API construída para a inserção de dados de CEPs em um banco de dados. A aplicação é desenvolvida para garantir a funcionalidade otimizada, gerando o banco de dados automaticamente durante o início, caso ainda não exista.


# Funcionalidades
Inserção de CEPs:  *A API permite a inserção de dados de CEPs no banco de dados. Caso o banco de dados não exista, ele será gerado automaticamente ao iniciar a aplicação.*

# Configuração Inicial
*Certifique-se de ter Node.js instalado em sua máquina antes de começar. Siga os passos abaixo:*

* Clone este repositório:
   ```
   https://github.com/MQSilveira/NodeDbInserter.git
   ```

* Navegue até o diretório do projeto:
   ```
   cd NodeDbInserter
   ```
* Instale as dependências:
   ```
   npm install
   ```
* Executando a Aplicação:
  Após a configuração inicial, você pode iniciar a aplicação com o seguinte comando:
   ```
   npm start
   ```
   *A API estará disponível em http://localhost:3001*

# Rotas da API
**Obtendo Todos os Endereços**
- **URL:** `http://localhost:3001/api/address/`
- **Método:** GET
- **Descrição:** Retorna todos os endereços cadastrados.

**Obtendo um Endereço Específico por CEP**
- **URL**: `http://localhost:3001/api/address/:cep`
- **Método:** GET
- **Descrição:** Retorna um endereço específico com base no CEP fornecido.

**Inserindo um Novo Endereço**
- **URL:** `http://localhost:3001/api/address/`
- **Método:** POST
- **Descrição:** Insere um novo endereço no banco de dados.
- **Corpo da Requisição:**
   ```
   {
      "cep": "01001-000",
      "logradouro": "Praça da Sé",
      "complemento": "lado ímpar",
      "bairro": "Sé",
      "localidade": "São Paulo",
      "uf": "SP",
      "ibge": "3550308",
      "gia": "1004",
      "ddd": "11",
      "siafi": "7107"
    }
   ```
