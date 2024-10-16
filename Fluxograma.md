```mermaid
graph TD
    A[Início] --> B{Autenticar usuário}
    B -- Válido? --> C[Tela Principal]
    B -- Inválido? --> B
    C --> D(Calendário)
    C --> E(Tarefas)
    C --> F(Chat)
    C --> G(Delegação de Funções)
    C --> H(Gerencia de Cargos)
    C --> I(Power BI)
    C --> J(Planilhas)
    C --> K(E-mail)
    C --> L(Log de Atividades)
    C --> M(Mensagens Importantes)
    D --> D1[Visualizar Calendário]
    D1 --> D2(Criar Evento)
    D1 --> D3(Editar Evento)
    D1 --> D4(Excluir Evento)
    D1 --> D5(Visualizar Detalhes)
    E --> E1[Visualizar Tarefas]
    E1 -- Nova Tarefa? --> E2(Criar Tarefa)
    E1 -- Não --> E3(Selecionar Tarefa)
    E3 --> E4{Ações?}
    E4 -- Sim --> E5(Executar)
    E4 -- Sim --> E6(Delegar)
    E4 -- Sim --> E7(Finalizar)
    E4 -- Sim --> E8(Adicionar Comentário)
    E4 -- Não --> E1
