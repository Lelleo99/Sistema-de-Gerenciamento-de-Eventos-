# Sistema de Gerenciamento de Eventos 📅

Este é um sistema de gerenciamento de eventos desenvolvido em Java para execução via Console. O projeto foi construído utilizando o paradigma de Programação Orientada a Objetos (POO) e estruturado com base no padrão arquitetural MVC (Model-View-Controller). 

## 🎯 Objetivo do Projeto
O sistema permite que os usuários se cadastrem e gerenciem sua participação em diversos eventos locais. Ele organiza os eventos por data e hora, permitindo consultar o que está acontecendo no momento, eventos futuros e o histórico de eventos passados, além de salvar todas as informações de forma persistente.

## ✨ Funcionalidades
- **Cadastro de Usuário:** Coleta de dados básicos (Nome, Email, Idade) logo na inicialização.
- **Cadastro de Eventos:** Criação de eventos contendo Nome, Endereço, Categoria, Horário (Data e Hora) e Descrição.
- **Categorização:** Eventos divididos em categorias pré-definidas (Festa, Esporte, Show, Teatro, Workshop, Outros).
- **Gestão de Presença:** - Listagem de eventos futuros ordenados pelo horário mais próximo.
  - Opção para confirmar presença em eventos listados.
  - Visualização de eventos confirmados e opção de cancelamento de participação.
- **Controle de Tempo (DateTime):**
  - Identificação automática de eventos ocorrendo no momento exato da consulta.
  - Histórico de eventos que já ocorreram.
- **Persistência de Dados:** Todos os eventos cadastrados são salvos automaticamente em um arquivo de texto (`events.data`). Ao reabrir o programa, o sistema carrega o arquivo e restaura os eventos.

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Java
- **Bibliotecas:** `java.time` (para manipulação de datas e horários), `java.io` (para leitura e escrita de arquivos) e `java.util` (Coleções e Scanner).
- **Arquitetura:** MVC (Model, View, Controller)

## 📁 Estrutura do Projeto
O código-fonte está organizado da seguinte maneira para separar as responsabilidades:

- `models/`: Contém as classes de entidade (`Usuario`, `Evento` e o Enum `Categoria`).
- `controllers/`: Contém a classe `EventoController` responsável pela lógica de negócio, ordenação e manipulação do arquivo `events.data`.
- `views/`: Contém a classe `Main` com a interface de console interativa para o usuário.

## 🚀 Como Executar

1. Clone este repositório:
   ```bash
   git clone [https://seu-link-do-repositorio-aqui.git](https://seu-link-do-repositorio-aqui.git)
