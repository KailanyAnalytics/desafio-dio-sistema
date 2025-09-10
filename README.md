# Sistema de Oficina Mecânica - Modelo Conceitual (EER)

## 📖 Descrição
Este projeto apresenta um **modelo conceitual** (EER) para um sistema de controle e gerenciamento de ordens de serviço em uma oficina mecânica.  
O objetivo é criar um diagrama claro para representar clientes, veículos, ordens de serviço, mecânicos, equipes, serviços e peças utilizadas.

## 🧾 Contexto
- Clientes levam veículos para conserto ou revisão.
- Cada veículo gera uma Ordem de Serviço (OS), com status, datas e autorização do cliente.
- Mecânicos são organizados em equipes e responsáveis pelos serviços.
- Valores de serviços vêm de uma tabela de referência de mão de obra, enquanto peças também possuem preço unitário.
- A OS agrupa todos os serviços e peças utilizados.

## 🔑 Entidades
- **Cliente**: dados básicos de identificação.
- **Veículo**: ligado a um cliente.
- **Ordem de Serviço (OS)**: registro de execução de serviços e peças.
- **Equipe**: grupo responsável pela OS.
- **Mecânico**: integra uma equipe.
- **Serviço**: tarefas realizadas na OS.
- **Peça**: itens utilizados para conserto ou revisão.

## 🔗 Relacionamentos
| Relacionamento            | Tipo |
|---------------------------|------|
| Cliente – Veículo         | 1:N  |
| Veículo – Ordem de Serviço| 1:N  |
| Equipe – Ordem de Serviço | 1:N  |
| Equipe – Mecânico         | 1:N  |
| Ordem de Serviço – Serviço| N:N  |
| Ordem de Serviço – Peça   | N:N  |

## 🛠️ Observações
- Entidades associativas **OS_Servico** e **OS_Peca** foram criadas para armazenar a quantidade de serviços e peças.
- Campos como endereço, telefone e email podem ser refinados conforme necessidade.
- Diagrama pode ser modelado em ferramentas como **dbdiagram.io**, **Lucidchart** ou **Draw.io**.


  
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/0be0876a-1f90-4ea7-b9d9-4885e12d33f3" />

