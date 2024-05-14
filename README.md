# M2_grupo_resilia

# Sistema de Gerenciamento de Curso Resilia

Este é um sistema de gerenciamento de curso desenvolvido para a plataforma Resilia. Ele permite o cadastro de cursos, alunos, facilitadores, módulos, turmas e o acompanhamento do progresso dos alunos.

## Estrutura do Banco de Dados

O banco de dados é organizado em um esquema chamado `resilia`, que contém as seguintes tabelas:

- **Cursos**: Armazena informações sobre os cursos oferecidos.
- **Alunos**: Contém dados dos alunos matriculados nos cursos.
- **Facilitadores**: Registra informações sobre os facilitadores que ministram as aulas.
- **Módulos**: Guarda detalhes sobre os módulos dos cursos.
- **Turmas**: Registra as turmas criadas para cada curso.
- **Alunos_Turmas**: Tabela de relacionamento entre alunos e turmas.
- **Facilitadores_Turmas**: Tabela de relacionamento entre facilitadores e turmas.
- **Porcentagem_Evasao_Por_Turma**: View que mostra a porcentagem de evasão por turma.
- **Log_Status_Alunos**: Tabela para registrar atualizações de status dos alunos.
- **Trigger atualizacao_status_aluno**: Trigger que popula a tabela `Log_Status_Alunos`.

## Funcionalidades Principais

- **Criação de Tabelas e Procedimentos Armazenados**: Utiliza procedimentos armazenados para criar as tabelas e inserir dados iniciais.
- **Consulta de Dados**: Fornece consultas para obter informações como o total de alunos, facilitadores em múltiplas turmas e alunos matriculados em cada turma.
- **Visualização de Porcentagem de Evasão**: Mostra a porcentagem de evasão por turma.
- **Registros de Atualização de Status**: Registra as atualizações de status dos alunos em uma tabela de log.
- **Trigger para Atualização de Status**: Associa uma trigger à tabela de alunos para registrar automaticamente as atualizações de status.
- **Perguntas Estratégicas**: Fornece consultas para responder perguntas estratégicas da empresa.

## Uso

Para utilizar o sistema, basta executar os scripts SQL fornecidos neste repositório em um ambiente PostgreSQL.

### Pré-requisitos

- PostgreSQL instalado e configurado.
- Cliente SQL (por exemplo, pgAdmin) para executar os scripts.

### Passos

1. Execute o script `criar_tabelas_resilia.sql` para criar as tabelas e procedimentos armazenados.
2. Execute o script `inserir_dados_resilia.sql` para inserir dados iniciais.
3. Execute o script `inserir_relacionamentos_resilia.sql` para estabelecer os relacionamentos entre os dados.
4. Explore as consultas fornecidas para obter insights sobre os dados do sistema.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue para relatar problemas ou propor melhorias.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter mais detalhes.

---

Certifique-se de ajustar o conteúdo conforme necessário e adicionar quaisquer outras informações relevantes sobre o seu projeto.
