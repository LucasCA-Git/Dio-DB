# Gerenciador de Catálogos da Netflix com Azure Functions

## **Sobre o Projeto**  
O **Dio-DB** é um gerenciador de catálogos inspirado na Netflix, desenvolvido com **Azure Functions** para criar uma solução serverless e **banco de dados** para armazenar informações sobre filmes, séries e gêneros. O projeto exemplifica como criar, organizar e automatizar uma solução escalável para gerenciar catálogos de conteúdo.



![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)  
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)  
![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)  
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)  

---
## **Arquitetura do Projeto**

### **Componentes Principais**
1. **Backend Serverless com Azure Functions**
   - APIs RESTful para criação, leitura, atualização e exclusão de itens do catálogo.
   - Integração com Azure Cosmos DB ou Azure SQL Database para persistência de dados.

2. **Frontend Angular**
   - Interface moderna e responsiva para gerenciamento do catálogo.
   - Comunicação com APIs utilizando o módulo `HttpClient`.

3. **Banco de Dados**
   - **Cosmos DB** (NoSQL): Armazena informações estruturadas em JSON.
   - **SQL Database**: Alternativa relacional para modelagem de dados.

4. **Azure Blob Storage**
   - Gerencia imagens como pôsteres ou miniaturas de filmes/séries.
---
1. **APIs RESTful**  
   * **GET /movies**: Retorna todos os filmes.  
   * **POST /movies**: Adiciona um novo filme ao catálogo.  
   * **PUT /movies/{id}**: Atualiza informações de um filme.  
   * **DELETE /movies/{id}**: Remove um filme do catálogo.  
2. **Gerenciamento de Banco de Dados**  
   * Estrutura relacional ou NoSQL para organização dos dados.  
   * Modelagem flexível para permitir múltiplos gêneros por filme.  
3. **Armazenamento de Imagens**  
   * Upload de pôsteres de filmes no Azure Blob Storage.  
   * URLs públicas ou assinadas para consumo direto.  
4. **Escalabilidade e Segurança**  
   * APIs serverless com escalabilidade automática.  
   * Segurança baseada em autenticação JWT ou Azure AD.

---

## **Deploy e Execução**

1. **Backend**

Configure e publique as Azure Functions com o comando:  
``` bash  
 func azure functionapp publish <app-name>
 ```

*   
2. **Frontend**

Execute a aplicação Angular localmente com:  
```bash  
ng serve
```
*   
3. **Banco de Dados**  
   * Configure o Cosmos DB ou o SQL Database no portal Azure.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

 
