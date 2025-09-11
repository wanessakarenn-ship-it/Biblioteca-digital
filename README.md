# Biblioteca-digital
Proposta de Sistema de Gerenciamento de Acervo para Biblioteca Escolar
​1. Requisitos Funcionais (RF)
​Esta seção descreve as funcionalidades essenciais que o sistema deve executar para atender às necessidades dos bibliotecários e usuários.

​1.1 Módulo de Gerenciamento de Acervo
​RF-001 - Cadastro de Livros: O sistema deve permitir o cadastro de um novo livro no acervo. As informações a serem registradas incluem título, autor(es), editora, ano de publicação e número de exemplares disponíveis.

Critérios de Aceitação do RF-001: Cadastro bem-sucedido com todos os campos preenchidos: Dado que o bibliotecário está na tela de cadastro de livros, Quando ele preencher todos os campos obrigatórios com informações válidas e confirmação do cadastro, Então o sistema deve salvar o livro no acervo e exibir uma mensagem de sucesso. 

Campos obrigatórios não preenchidos: Dado que o bibliotecário está na tela de cadastro de livros, Quando ele tenta salvar sem preencher um ou mais campos obrigatórios (ex: título, autor, editora), então o sistema deve exibir uma mensagem de erro de referência quais campos estão faltando. Validação de formato do ISBN (ou outro código): Dado que o bibliotecário está preenchendo o campo de código de identificação, Quando ele insere um código em formato inválido, Então o sistema deve impedir o cadastro e informar que o código deve estar em um formato válido (ex: ISBN-13).

Verificação de duplicidade de livros (opcional, se aplicável): Dado que o bibliotecário está tentando cadastrar um novo livro, Quando o sistema identifica que um livro com o mesmo ISBN já está cadastrado, Então o sistema deve alertar o bibliotecário e sugerir atualização de exemplares ao invés de novo cadastro (se essa para a regra do sistema). Cadastro de exemplares múltiplos: Dado que o bibliotecário informa o número de exemplares disponíveis, Quando ele conclui o cadastro, então o sistema deve registrar corretamente a quantidade de exemplares no acervo.

​RF-002 - Listagem de Livros: O sistema deve exibir uma lista paginada de todos os livros cadastrados no acervo, com a opção de ordenação por título ou autor. A lista deve apresentar, no mínimo, o título, o autor principal e o status de disponibilidade.
​RF-003 - Busca de Livros: O sistema deve prover uma funcionalidade de busca, permitindo a localização de livros no acervo por título ou autor. A busca deve ser de texto livre e insensível a maiúsculas e minúsculas.

​1.2 Módulo de Controle de Empréstimos
​RF-004 - Registro de Empréstimo: O sistema deve permitir que um bibliotecário registre o empréstimo de um livro para um usuário cadastrado. A operação deve associar o livro (identificado por seu ISBN) a um usuário (identificado por um código de matrícula), registrar a data do empréstimo e calcular a data de devolução prevista. O status do exemplar deve ser alterado para "emprestado".
​RF-005 - Registro de Devolução: O sistema deve permitir que um bibliotecário registre a devolução de um livro. A operação deve alterar o status do exemplar para "disponível" e registrar a data da devolução.

​2. Requisitos Não Funcionais (RNF)
​Esta seção define as qualidades e restrições que o sistema deve seguir para garantir sua eficácia e usabilidade.
​2.1 Requisitos de Usabilidade

​RNF-001 - Interface Intuitiva: A interface do usuário (UI) deve ser intuitiva, com um fluxo de trabalho lógico e componentes de navegação claros, minimizando a necessidade de treinamento para os bibliotecários.

​2.2 Requisitos de Desempenho
​RNF-002 - Tempo de Resposta: O sistema deve responder a todas as ações (e.g., consultas, cadastro, empréstimo) em um tempo máximo de 2 segundos sob condições normais de uso.

​2.3 Requisitos de Segurança
​RNF-003 - Acesso Autorizado: O sistema deve exigir autenticação de usuário para o acesso a todas as funcionalidades. Apenas usuários com o perfil de "bibliotecário" devem ter permissão para realizar operações de cadastro e gerenciamento.

​2.4 Requisitos de Compatibilidade
​RNF-004 - Compatibilidade com Navegadores: O sistema deve ser compatível e funcional nos navegadores web mais comuns, como Google Chrome, Mozilla Firefox, Microsoft Edge e Safari, garantindo uma experiência de usuário consistente.

​RNF-005 - Otimização para dispositivos móveis: O sistema deve redimensionar imagens e texto para que se ajustem a diferentes tamanhos de ecrã, eliminando a necessidade de ampliar ou rolar horizontalmente para visualizar o conteúd
