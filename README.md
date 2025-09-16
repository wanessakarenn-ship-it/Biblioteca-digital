Plano de Requisitos para o Sistema de Gestão de Acervo da Biblioteca
Este documento descreve as funcionalidades e qualidades essenciais para a primeira versão do sistema, com base nas definições iniciais do grupo.
1. Requisitos Funcionais (O que o sistema faz?)
RF1: Cadastro de Livros

O sistema deve permitir que um bibliotecário adicione novos livros ao acervo.
•	Dados necessários: Título, Autor(es), Ano de Publicação, ISBN (opcional), Gênero, e uma contagem de cópias disponíveis.
RF2: Listagem de Livros
O sistema deve exibir uma lista completa de todos os livros cadastrados.

•	Detalhes da lista: A listagem deve incluir o Título, Autor e a disponibilidade de cada livro (total de cópias vs. cópias disponíveis).
RF3: Busca de Livros
O sistema deve oferecer uma funcionalidade de busca para localizar livros rapidamente.

•	Critérios de busca: A busca deve permitir encontrar livros tanto por Título quanto por Autor. A busca deve ser insensível a maiúsculas e minúsculas.
RF4: Gerenciamento de Empréstimos e Devoluções
O sistema deve rastrear a circulação de livros.

•	Fluxo de Empréstimo: Registrar que um livro foi emprestado por um aluno, anotando o nome do aluno e a data do empréstimo.
•	Fluxo de Devolução: Permitir que o bibliotecário registre a devolução de um livro, atualizando o status de disponibilidade do livro no acervo.
3. Requisitos Não Funcionais (Como o sistema deve ser?)
RNF1: Usabilidade e Interface

A interface do sistema deve ser fácil de usar e visualmente limpa.
•	Objetivo: Bibliotecários devem ser capazes de realizar as tarefas de forma intuitiva, com mensagens claras de sucesso ou erro.
RNF2: Compatibilidade de Navegador

O sistema deve funcionar corretamente em navegadores web modernos, como Chrome, Firefox e Edge.
•	Objetivo: A interface deve ser responsiva, adaptando-se a diferentes tamanhos de tela (desktop, tablet e celular) para garantir a acessibilidade.
RNF3: Segurança
O sistema deve proteger os dados do acervo e restringir o acesso a funções de gerenciamento.

•	Objetivo: Apenas bibliotecários autorizados devem ter permissão para cadastrar, editar ou registrar empréstimos. Uma forma simples de autenticação será necessária.
RNF4: Desempenho
O sistema deve responder às ações do usuário em tempo hábil.

•	Objetivo: Atrasos não devem exceder 2 segundos em ações comuns como buscar, listar ou cadastrar.
