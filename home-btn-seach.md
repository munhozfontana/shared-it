## História: Barra de Busca

**Descrição:**
Como usuário da página inicial (home), desejo ter uma barra de busca funcional para pesquisar relatórios, empresas e analistas, permitindo uma navegação fácil e intuitiva para encontrar as informações desejadas.

**Critérios de Aceitação:**
1. Na página inicial (home), implementar uma barra de busca que permita ao usuário digitar texto.
2. Ao digitar na barra de busca, deve aparecer o botão "Search".
3. Caso o usuário selecione o botão "Search", a página deve navegar para a próxima tela que exibirá os resultados da busca, passando o texto da busca como argumento.
4. Se a barra de busca estiver vazia e o usuário pressionar Enter ou clicar no botão "Search", a ação padrão deve ser submeter a busca e a página deve navegar para os resultados da busca.
5. Caso a barra de busca esteja vazia, deve ser exibido o placeholder "Search reports, companies, analysts..." para orientar o usuário sobre o que pode ser pesquisado.

**Considerações Técnicas:**
1. Utilizar Angular 15 como framework principal para o desenvolvimento da funcionalidade da barra de busca.
2. Integrar a barra de busca à página inicial (home), garantindo uma experiência de usuário consistente.
3. Implementar lógica para a submissão da busca tanto ao pressionar Enter quanto ao clicar no botão "Search".
4. Utilizar o mecanismo de navegação do Angular para direcionar o usuário para a página de resultados da busca ao selecionar o botão "Search", passando o texto da busca como argumento.
5. Adicionar o placeholder "Search reports, companies, analysts..." na barra de busca conforme especificado pela UX para orientar o usuário sobre o que pode ser pesquisado.
6. Garantir que a barra de busca seja responsiva e se ajuste adequadamente em diferentes tamanhos de tela e dispositivos.
7. Realizar testes unitários utilizando Jest para verificar o comportamento da barra de busca em diferentes cenários de interação.
