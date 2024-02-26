## Considerações Técnicas
- Utilizar Angular 15 como framework principal para o desenvolvimento da funcionalidade.
- Reaproveitar os componentes da biblioteca interna da empresa, a "LibGestaoConteudoModule":
    - Para a listagem das empresas: `gc-company-card-list`
    - Para a listagem dos analistas: `gc-analsty-card-list`
    - Para a listagem dos relatórios: `gc-reports-list`
    - Esse aproveitamento dos componentes garantirá consistência visual e facilitará a manutenção futura, além de promover a coesão entre as diferentes partes da aplicação.
- Integrar as APIs específicas para busca:
    - API de relatórios: `/api/reports`
    - API de companhias: `/api/companies`
    - API de analistas: `/api/analysts`
- Realizar chamadas assíncronas para as APIs utilizando os serviços de HTTP fornecidos pelo Angular.
- Implementar tratamento de erros robusto para cenários de falha na chamada da API, exibindo mensagens de erro adequadas ao usuário e fornecendo opções para tentar novamente:
    - **Erro de Resultado Vazio:**
        - Se a busca não retornar resultados, exibir uma mensagem convidando o usuário a tentar uma nova busca. A mensagem deve ser clara e compreensível para o usuário (validar com a UX, Marina).
    - **Erro no Backend:**
        - Em caso de falha na conexão com o servidor, mostrar uma mensagem de erro indicando que houve um problema ao processar a solicitação. Oferecer a opção de tentar novamente. Se o problema persistir, sugerir que o usuário entre em contato com o suporte técnico. (validar com a UX, Marina).
- Implementar testes unitários e de integração utilizando Jest para garantir a qualidade e a estabilidade da funcionalidade de busca.
- Realizar o tagamento de acordo com as regras definidas pelo Product Owner (Leonardo) para rastreamento de eventos relacionados à busca.
- Garantir que a funcionalidade seja responsiva e ofereça uma boa experiência de usuário em diferentes dispositivos e tamanhos de tela.

## Repositório de Desenvolvimento
[Repositório no GitHub](https://github.com/itau-corp/itau-fw9-app-gestaoconteudo-home)