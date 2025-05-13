

# 1. Especificações do Projeto

#### 1.1. Usuários

| Tipo de Usuário   | Descrição | Responsabilidades |
|------------------|-----------|------------------|
| **Administrador do Sistema** | O proprietário do portfólio.| Manter o portfólio atualizado com novos projetos, informações sobre suas habilidades e formas de contato |
| **Recrutadores e Gerentes de Contratação** | Pessoas que estão buscando identificar e contratar talentos na área de tecnologia. | Navegar pelo seu portfólio para entender suas habilidades, experiência (mesmo que inicial em desenvolvimento), os projetos que eu  desenvolver e como entrar em contato.|
| **Outros Desenvolvedores** |Colegas de profissão que podem estar interessados em meus seus projetos, trocar ideias ou até colaborar no futuro. |Explorar seu código, entender suas abordagens para resolver problemas e talvez aprender algo com meus projetos.|


#### 1.2. Arquitetura

Este projeto do Sistema de Gestão de Eventos adota a seguinte arquitetura:

* **Front-end:**
    * **Tecnologia:** [React](https://react.dev/)
    * **Linguagem:** [TypeScript](https://www.typescriptlang.org/)
    * **Descrição:** A interface do usuário web será desenvolvida utilizando a biblioteca React, que permite a criação de interfaces dinâmicas e reativas. O uso de TypeScript adiciona tipagem estática ao JavaScript, melhorando a manutenibilidade e a detecção de erros durante o desenvolvimento.

* **Back-end:**
    * **Tecnologia:** [Node.js](https://nodejs.org/en/) com [Express.js](https://expressjs.com/)
    * **Linguagem:** [TypeScript](https://www.typescriptlang.org/)
    * **Descrição:** A lógica do servidor e a API (Application Programming Interface) serão construídas utilizando Node.js, um ambiente de execução JavaScript server-side, e o framework Express.js, que facilita a criação de aplicações web robustas e APIs RESTful. O uso de TypeScript no back-end garante consistência de tipos em toda a aplicação.

* **Banco de Dados:**
    * **Tecnologia:** [MySQL](https://www.mysql.com/)
    * **Descrição:** Os dados da aplicação, como informações de eventos, usuários e inscrições, serão persistidos em um banco de dados relacional MySQL.


### 1.3. Tecnologias

Este projeto utilizará as seguintes tecnologias principais:

* **Linguagens:**
    * TypeScript
    * JavaScript

* **Front-end:**
    * React

* **Back-end:**
    * Node.js
    * Express.js

* **Banco de Dados:**
    * MySQL

* **Outras Ferramentas:**
    * Git (para controle de versão)
    * npm ou yarn (gerenciadores de pacotes)

### 2. Requisitos

#### 2.1. Requisitos Funcionais

| ID | Descrição do Requisito | Prioridade |
|----|------------------------|------------|
|RF-001| O portfólio deve exibir suas informações relevantes, como sua área de atuação (desenvolvimento, UX, etc.), um breve resumo sobre você e seus objetivos profissionais.| ALTA | 
|RF-002| O portfólio deve listar suas habilidades técnicas (linguagens de programação, frameworks, ferramentas) de forma clara e organizada.| ALTA |
|RF-003| O portfólio deve apresentar seus projetos de forma individual, incluindo uma descrição, as tecnologias utilizadas e, idealmente, links para o código no GitHub e/ou uma demonstração online (se aplicável).| ALTA |
|RF-004| O portfólio deve fornecer formas claras para que os visitantes entrem em contato com você (e-mail, LinkedIn, etc.). | ALTA |
|RF-005| O portfólio deve ter um design visualmente agradável e se adaptar bem a diferentes tamanhos de tela (desktop, tablet, mobile) | ALTA |
|RF-006| O portfólio deve permitir que os visitantes naveguem facilmente entre as diferentes seções (sobre mim, habilidades, projetos, contato). | ALTA | 

### 2.2 Requisitos não Funcionais

| ID | Descrição do Requisito | Prioridade |
|----|------------------------|------------|
|RNF-001|O portfólio deve ser fácil de navegar e entender para os visitantes (recrutadores, outros desenvolvedores, etc.). A informação deve ser encontrada de forma intuitiva. | ALTA | 
|RNF-002|O layout do portfólio deve se adaptar bem a diferentes dispositivos e tamanhos de tela (desktops, tablets, smartphones), garantindo uma boa experiência de visualização em qualquer dispositivo. | ALTA |
|RNF-003| O portfólio deve carregar rapidamente para não afastar os visitantes. Otimização de imagens e código é importante. |  ALTA |
|RNF-004| O sistema deve preservar a integridade e privacidade dos dados cadastrados (Criptografia e Segurança). |  ALTA |
|RNF-005|O código do portfólio deve ser bem estruturado e fácil de atualizar, permitindo que você adicione novos projetos ou informações no futuro sem grandes dificuldades. | MÉDIA |
|RNF-006| A aplicação deve possuir backup de segurança automático em nuvem. | MÉDIA |
|RNF-007| Considerar a acessibilidade (WCAG) para garantir que pessoas com deficiência também possam navegar pelo seu portfólio. Isso pode incluir texto alternativo para imagens, uso correto de semântica HTML, etc.| ALTA |


#### 3.2. Restrições

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01|  O portfólio focará na apresentação de um número limitado de projetos (por exemplo, seus primeiros projetos mais relevantes). Funcionalidades mais complexas (como um blog integrado, sistema de comentários, etc.) podem ficar para futuras iterações. |
|02| A interatividade pode ser mantida em um nível básico, focando na navegação e exibição de informações, sem funcionalidades dinâmicas complexas (a menos que seus projetos as demandem).|
|03| O design será moderno e agradável, mas pode se basear em templates ou frameworks de UI para acelerar o desenvolvimento, em vez de um design totalmente personalizado desde o início.|
|04| O desenvolvimento se concentrará nas tecnologias que você está aprendendo ou já domina (React, TypeScript, HTML, CSS, etc.), evitando a introdução de tecnologias completamente novas apenas para o portfólio neste momento.|
|05| A hospedagem inicial pode ser em plataformas gratuitas como GitHub Pages, Vercel ou Netlify, o que pode trazer algumas limitações|

### 3. Diagrama de Caso de Uso

![image](https://github.com/user-attachments/assets/86adf374-cf46-4671-a381-1dc92cee71ac)

- Visualizar Página Inicial: O visitante acessa a página principal do seu portfólio.
- Navegar para a Seção "Sobre Mim": O visitante quer saber mais sobre sua trajetória e habilidades.
- Navegar para a Seção "Habilidades": O visitante quer ver suas competências técnicas.
- Visualizar Projetos: O visitante quer ver os projetos que você desenvolveu.
- Acessar Detalhes do Projeto: O visitante quer mais informações sobre um projeto específico (tecnologias, descrição, links).
- Visualizar Informações de Contato: O visitante quer saber como entrar em contato com você.


### 4. Projeto da Base de Dados

#### 4.1. Entidades e Relacionamentos

[Descrição das principais entidades e como elas se relacionam]

#### 4.2. Diagrama ER

[Seção para incluir o Diagrama Entidade-Relacionamento (pode ser uma imagem)]


