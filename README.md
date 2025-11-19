<p align="center">
  <img src="./Banner Eco.png" width="850px" />
</p>

<p align="center">
  <img src="./demo.gif" width="650px" />
</p>


<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" />
  <img src="https://img.shields.io/badge/License-MIT-blue" />
  <img src="https://img.shields.io/badge/Database-MySQL-00758F?logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Model-MySQL%20Workbench-blue?logo=mysql" />
</p>


## 📑 Índice
- [Visão Geral do Modelo](#visão-geral-do-modelo)
- [Descrição Geral](#descrição-geral)
- [Estrutura do Banco de Dados](#estrutura-do-banco-de-dados)
- [Cardinalidades do Modelo](#cardinalidades-do-modelo)
- [Arquivos do Repositório](#arquivos-do-repositório)
- [Como abrir o projeto](#como-abrir-o-projeto)
- [Próximos Passos](#próximos-passos)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Objetivo](#objetivo)
- [Autor](#autor)
- [License](#license)






# 🛒 Modelo Lógico do Banco de Dados para E-commerce

Este repositório apresenta o **modelo lógico de um sistema de E-commerce**, desenvolvido como parte de um estudo sobre estruturação de banco de dados relacional.  
O objetivo é representar entidades, relacionamentos e regras de negócio comuns em operações de compras online.

---

##  Visão Geral do Modelo

O diagrama abaixo mostra a estrutura completa do banco:

![Modelo Lógico](modelo-e-commerce.png)

---

##  Descrição Geral

O modelo foi construído com foco em:

- Controle de produtos cadastrados na plataforma  
- Gestão de fornecedores e vendedores  
- Processamento de pedidos, pagamentos e entregas  
- Registro de clientes e métodos de pagamento  
- Relação entre produtos, estoque e disponibilidades  

---

##  Estrutura do Banco de Dados

O sistema contém as seguintes entidades principais:

- **Produto:** Catálogo de itens disponíveis na loja.  
- **Cliente:** Dados cadastrais, endereço e documentos.  
- **Pedido:** Solicitações feitas pelos clientes.  
- **Pagamento:** Formas de pagamento e status.  
- **Entrega:** Informações de rastreamento e envio.  
- **Fornecedor:** Empresas responsáveis pelos produtos.  
- **Terceiro/Vendedor:** Representações externas que vendem produtos.  
- **Estoque:** Controle de quantidade disponível por produto.

---

## Cardinalidades do Modelo

Cliente 1:N Pedido – um cliente pode realizar vários pedidos.

Pedido 1:N Pagamento – um pedido pode ter múltiplos registros de pagamento.

Pedido 1:N Entrega – cada pedido possui informações de envio e atualização.

Pedido N:N Produto – representado pela tabela intermediária de itens do pedido.

Produto 1:1 Estoque – cada produto possui um registro único de estoque.

Fornecedor N:N Produto – um produto pode ter vários fornecedores e vice-versa.

Vendedor N:N Produto – vendedores podem disponibilizar vários produtos.

---

##  Arquivos do Repositório

- **Banner Eco.png** — banner principal do projeto  
- **demo.gif** — demonstração animada de abertura do modelo no Workbench  
- **modelo-ecommerce.mwb** — arquivo editável do MySQL Workbench  
- **modelo-ecommerce.png** — imagem estática do modelo lógico  
- **LICENSE** — licença MIT do projeto  
- **README.md** — documentação do repositório

---

##  Como abrir o projeto

1. Faça o download do arquivo `.mwb`
2. Abra o MySQL Workbench
3. Vá em **File > Open Model**
4. Selecione o arquivo `modelo-logico-ecommerce.mwb`
5. Pronto! O modelo lógico estará disponível para visualização e edição.

<p align="center">
  <img src="./abrindo-modelo.gif" width="700px" />
</p>

---
##  Próximos Passos

- Criar modelo lógico no formato DER.
- Gerar scripts SQL automaticamente a partir do Workbench.
- Popular as tabelas com dados de teste (mock data).
- Criar consultas SQL para análise e relatórios.



---

##  Tecnologias Utilizadas

![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![Workbench](https://img.shields.io/badge/MySQL_Workbench-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

##  Objetivo

Este projeto foi criado para:

- Demonstrar boas práticas de modelagem de dados.
- Criar um modelo escalável para estudos e portfólio.


---

##  Autor

**Fabiano Ferreira**  
🔗 [LinkedIn](https://www.linkedin.com/in/fabianoferreira-bi/)

🔗 [GitHub](https://github.com/Fabianogf12)

---


##  License

This project is licensed under the MIT License.  
For more details, please refer to the **LICENSE** file in the root of this repository.

---


📌 *Projeto desenvolvido para fins educativos e de portfólio. Sugestões e melhorias são sempre bem-vindas!*  

