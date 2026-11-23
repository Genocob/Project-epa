# Relatório Final de Desenvolvimento do projeto LayoutLab

## Identificação do projeto

**Projeto:** LayoutLab  
**Instituição:** Etec Sales Gomes  
**Curso:** 2º MTec/NT — Desenvolvimento de Sistemas  
**Disciplina:** Desenvolvimento de Sistemas  
**Turma/período:** 4º bimestre do 2º ano  

**Integrantes:**

- Davi Mariano da Silva
- Fabricio Eid Bertolini
- Filipe de Almeida Cisotto
- Gustavo Momberg Miranda
- Isaac Xavier Garcia
- Lucas Nunes da Silva
- Matheus Henrique dos Santos Brasil
- Miguel Alves Rocha
- Pietra Eid Gomes

---

## Apresentação do relatório

Este relatório reúne o planejamento inicial e a evolução do LayoutLab, desde a primeira conversa do grupo com uma ferramenta de Inteligência Artificial até os aprimoramentos realizados para a apresentação do projeto ao público.

A documentação mantém separadas duas fases que possuem objetivos diferentes. A primeira é a etapa de planejamento, registrada em 16 de setembro de 2026, na qual o grupo discutiu o problema, o público, os requisitos e as decisões técnicas, sem solicitar código à IA. A segunda corresponde à continuidade do projeto, quando a proposta foi transformada em uma aplicação e recebeu melhorias funcionais, educacionais e visuais.

As sugestões apresentadas pela IA são identificadas como recomendações, enquanto as escolhas do grupo são registradas como decisões. Essa distinção é importante porque nem toda sugestão discutida foi adotada e porque algumas características do projeto foram ampliadas depois da primeira etapa.

# 1. Registro da primeira interação com Inteligência Artificial

**Ferramenta utilizada:** Manus AI  
**Data da interação:** 16/09/2026

### 1.1. Contexto apresentado pelo grupo

Na primeira interação, o grupo se apresentou como estudante do curso de Desenvolvimento de Sistemas da Etec Sales Gomes e informou já ter estudado ou utilizado tecnologias e conteúdos como JavaScript, lógica de programação, HTML, CSS, SQL, MySQL, princípios de Design Digital, princípios de APS, Node.js, React básico, Python/Flask, Bootstrap, Firebase e APIs.

O grupo também informou ter experiência anterior com alguns layouts de sites e aplicações que utilizavam APIs. A principal necessidade apresentada era desenvolver uma ferramenta digital para o público jovem, relacionada a uma disciplina da grade curricular e capaz de auxiliar estudantes no aprendizado. A disciplina escolhida foi Design Digital.

### 1.2. Ideia apresentada inicialmente

A proposta inicial era criar um editor de layouts para a web, inspirado em ferramentas como Canva, Figma e FlutterFlow, mas com uma interface mais simples e acessível para pessoas com pouca ou nenhuma experiência em Design Digital.

O fluxo imaginado começaria em uma tela inicial com modelos de layout predefinidos. Depois de selecionar um modelo, o usuário seria encaminhado para um editor. Essa tela teria um menu lateral esquerdo com elementos que poderiam ser inseridos, como botões, blocos de texto, imagens, links e cards; um painel à direita para alterar propriedades, como cor, tamanho e posição; e uma área central, chamada canvas, para visualizar a composição.

Na ideia original também foi mencionado um botão “Gerar código”, que levaria a uma tela para exibir o código correspondente ao layout. Entretanto, o grupo deixou claro no prompt que, naquela primeira etapa, não desejava gerar código com a IA: o objetivo era discutir a proposta, os requisitos e as decisões técnicas antes de iniciar a implementação.

### 1.3. Prompt enviado à Manus AI

```text
Olá! Somos estudantes do curso de Desenvolvimento de Sistemas da Etec Sales Gomes.

Atualmente estamos no 3º semestre do 2º ano.

Durante o curso já estudamos assuntos como:
- JavaScript
- Lógica de programação
- HTML e CSS
- SQL e MySQL
- Princípios de Design Digital
- Princípios de APS
- Node.js
- React básico
- Python/Flask
- Bootstrap
- Firebase
- APIs

Já tivemos contato com JavaScript, Node.js/Express, Python/Flask, HTML, CSS e React.

Nossa experiência com desenvolvimento de software envolve alguns layouts de sites e aplicações com APIs.

Temos um problema em que precisamos desenvolver um projeto para o público jovem. O objetivo é selecionar uma disciplina da grade curricular e criar uma ferramenta digital (site) capaz de auxiliar estudantes nessa área.

Como grupo, optamos pela disciplina de Design Digital. Nossa proposta consiste em desenvolver um criador de layouts inspirado em ferramentas como Canva, Figma e FlutterFlow, porém com uma identidade visual mais simples e acessível, voltada especialmente a usuários com pouca ou nenhuma experiência na área.

A experiência do usuário começa em um menu inicial, no qual é possível escolher entre layouts predefinidos. Ao selecionar uma opção, o usuário é direcionado a uma página de editor de layout, onde pode personalizar o design conforme desejar.

Nessa tela, há um menu lateral esquerdo com elementos disponíveis para inserção no layout, como botões, blocos de texto, imagens, links e cards. Do lado direito, encontra-se um painel de propriedades para ajustes de cor, tamanho, posição e outras configurações. O canvas de edição fica posicionado no centro da tela.

Ainda nessa página, o usuário pode clicar no botão “Gerar código”, sendo então redirecionado a uma nova tela que exibe o código correspondente ao layout criado.

Precisamos desenvolver um projeto que será apresentado ao público. O público principal são estudantes, especialmente do Ensino Médio, em contexto educacional da Etec Sales Gomes.

Nesta primeira etapa, não queremos gerar código. Queremos discutir a ideia, os requisitos e as decisões técnicas do projeto.
```

# 2. Análise da proposta e contribuições da IA

A Manus AI considerou a ideia adequada ao contexto de Design Digital, mas alertou que tentar reproduzir a quantidade de recursos de plataformas profissionais poderia tornar o projeto amplo demais para o prazo e para a experiência do grupo.

A principal recomendação foi posicionar o LayoutLab como uma ferramenta educacional introdutória, e não como um concorrente de Canva ou Figma. O objetivo sugerido foi ajudar estudantes iniciantes a compreender a composição de páginas, a organização visual, a hierarquia das informações, o uso de cores e a relação entre design e desenvolvimento web.

### 2.1. Público e problema discutidos

A IA recomendou concentrar o público principal em estudantes do Ensino Médio e da Etec que estivessem começando a estudar Design Digital e desenvolvimento web. Professores, visitantes da Etec de Portas Abertas e outros iniciantes poderiam constituir públicos secundários.

A análise também apontou que “criar layouts” poderia significar diferentes coisas, como produzir peças para redes sociais, páginas web, interfaces de aplicativos ou protótipos. Por isso, recomendou delimitar o produto à criação de páginas web simples, evitando uma proposta genérica demais.

O problema foi relacionado às dificuldades que iniciantes podem encontrar para começar uma composição do zero, organizar elementos, escolher cores e tamanhos, utilizar ferramentas profissionais e entender como um layout visual se relaciona com HTML e CSS.

### 2.2. Recomendações para o funcionamento do editor

Entre as recomendações apresentadas estavam:

- oferecer alguns modelos prontos e também a possibilidade de iniciar um layout vazio;
- organizar o editor em uma área central de visualização, um menu de elementos e um painel de propriedades;
- começar com componentes básicos, como títulos, textos, imagens, botões, cards, links e seções;
- permitir selecionar um elemento e alterar suas propriedades;
- atualizar a visualização à medida que o usuário modifica o layout;
- oferecer meios de remover elementos e reiniciar a composição;
- disponibilizar uma visualização final sem os controles do editor;
- salvar o trabalho localmente no navegador;
- apresentar orientações simples para apoiar usuários iniciantes.

A IA também recomendou que o grupo evitasse, no primeiro protótipo, recursos que aumentariam muito a complexidade, como edição totalmente livre, sistema avançado de camadas, colaboração em tempo real, histórico completo de versões, publicação automática de sites e geração avançada de código.

### 2.3. Organização dos dados e posicionamento dos elementos

A discussão técnica destacou que o layout deveria ser representado por dados, e não apenas como algo desenhado na tela. A IA sugeriu que um projeto pudesse armazenar informações como identificador, nome, modelo, dimensões do canvas, elementos e data de alteração. Cada elemento poderia guardar identificador, tipo, conteúdo, posição, dimensões, cor, tamanho de fonte e propriedades específicas.

Também foram discutidas duas formas de organizar os elementos: posicionamento livre, semelhante ao de editores profissionais, ou organização por seções e blocos. A recomendação foi começar com uma estrutura baseada em seções e componentes controlados. Essa alternativa diminuiria a complexidade, facilitaria a responsividade e aproximaria o resultado da estrutura de uma página web.

### 2.4. Requisitos de qualidade, avaliação e etapas sugeridas

Além das funções do editor, a IA apresentou recomendações de qualidade para a aplicação: interface compreensível, respostas rápidas às alterações, responsividade, legibilidade e contraste adequados, organização em componentes reutilizáveis, compatibilidade com navegadores atuais, segurança no tratamento dos dados e consistência visual.

Também sugeriu avaliar o protótipo observando se um estudante consegue criar um layout sem explicações extensas, localizar os elementos, identificar o item selecionado, alterar propriedades, remover componentes, visualizar o resultado e compreender a finalidade da ferramenta. A recomendação foi testar com pessoas que não participaram do desenvolvimento, pois elas poderiam encontrar dificuldades que o próprio grupo não perceberia.

Como sequência de trabalho, a IA propôs um roteiro em etapas: planejamento e definição dos modelos; protótipo visual; implementação do editor básico; salvamento local; testes com usuários e correções; e, somente depois, possíveis evoluções, como geração de HTML e CSS, mais componentes, exportação e recursos online.

# 3. Funcionalidades levantadas no planejamento inicial

O registro inicial reuniu funcionalidades que o grupo considerava importantes para a ferramenta. Elas podem ser organizadas por finalidade:

| Área | Funcionalidades consideradas | Finalidade registrada ou discutida |
|---|---|---|
| Início e modelos | Tela inicial de apresentação, galeria de modelos e opção de começar com um layout vazio | Explicar a proposta e oferecer pontos de partida para quem não sabe como iniciar. |
| Edição | Editor organizado em seções e componentes, canvas central, menu lateral e painel de propriedades | Concentrar a criação e a personalização em uma interface visual. |
| Elementos | Inserção de títulos, textos, imagens, botões, links, cards e seções | Permitir criar páginas simples com componentes comuns. |
| Seleção e personalização | Seleção visual de elementos e edição de textos, cores, tamanhos, alinhamentos e aparência básica | Dar ao usuário controle sobre a composição e facilitar a identificação do elemento editado. |
| Organização | Remoção de elementos e opção de limpar ou reiniciar o layout | Permitir corrigir escolhas e iniciar uma nova demonstração. |
| Visualização | Visualização do resultado sem os controles do editor | Mostrar a composição de forma mais próxima da página final. |
| Salvamento | Salvamento e recuperação por meio do `localStorage` | Evitar a perda do trabalho sem exigir conta ou banco de dados remoto. |
| Apoio ao usuário | Orientações simples para iniciantes e validações básicas | Ajudar o usuário a utilizar a ferramenta e corrigir preenchimentos inadequados. |
| Qualidade do produto | Identidade visual própria, responsividade, componentes React reutilizáveis, documentação e testes básicos de usabilidade | Melhorar consistência, manutenção, acessibilidade e compreensão da ferramenta. |


# 4. Discussão e alternativas técnicas

A conversa com a IA comparou cinco possibilidades de arquitetura. As alternativas foram registradas da seguinte forma:

## 4.1. Alternativa 1 — HTML, CSS e JavaScript sem React

**Tecnologias:** HTML, CSS, JavaScript e `localStorage`.

**Vantagens discutidas:** utiliza tecnologias conhecidas pelo grupo, não exige aprender React e pode ser suficiente para um protótipo pequeno.

**Desvantagens discutidas:** a manipulação direta do DOM poderia se tornar difícil de manter conforme o editor crescesse; também seria mais trabalhoso manter sincronizados o canvas e o painel de propriedades e evitar repetição de código.

## 4.2. Alternativa 2 — React com armazenamento local

**Tecnologias:** React, JavaScript, HTML, CSS, `localStorage` e Vite.

**Vantagens discutidas:** aproveita conhecimentos que o grupo já possuía, permite dividir a interface em componentes, facilita a atualização do canvas conforme o estado da aplicação muda e não exige a criação de um backend para o escopo inicial.

**Desvantagens discutidas:** exige compreender estados, propriedades e eventos do React; o armazenamento local tem limitações e os projetos permanecem no navegador e dispositivo em que foram salvos, sem sincronização em nuvem.

## 4.3. Alternativa 3 — React com Node.js e Express

**Tecnologias:** React no front-end, API em Node.js/Express e banco de dados.

**Vantagens discutidas:** permitiria cadastro, login, armazenamento centralizado e compartilhamento de projetos, além de possibilitar futuras funcionalidades no servidor.

**Desvantagens discutidas:** aumentaria a complexidade, exigiria desenvolver e testar uma API, configurar banco de dados e tratar autenticação, segurança e hospedagem. Também criaria mais dependências para a apresentação.

## 4.4. Alternativa 4 — React com Firebase

**Tecnologias:** React e serviços Firebase, como Authentication, Firestore e Storage.

**Vantagens discutidas:** ofereceria serviços prontos para autenticação, banco de dados, armazenamento de arquivos e hospedagem, reduzindo a necessidade de construir um backend próprio.

**Desvantagens discutidas:** acrescentaria dependência de serviço externo, configuração e regras de segurança. Foi considerada desnecessária caso o protótipo precisasse apenas de salvamento local.

## 4.5. Alternativa 5 — React com Flask

**Tecnologias:** React no front-end e API em Python/Flask.

**Vantagens discutidas:** o grupo já havia tido contato com Python e Flask, e a tecnologia poderia atender a uma API pequena ou a futuros processamentos no servidor.

**Desvantagens discutidas:** introduziria uma segunda linguagem na aplicação, exigiria manter front-end e back-end separados e não havia uma necessidade concreta que justificasse essa arquitetura naquele momento.

## 4.6. Escolha registrada pelo grupo

O grupo registrou a escolha da **Alternativa 2**, com React e armazenamento local. A justificativa anotada foi que essa opção utilizava tecnologias com as quais os integrantes já tinham familiaridade. O registro também aponta que a Alternativa 3, embora fosse uma possibilidade forte, incluía funcionalidades que o grupo não pretendia utilizar.

A escolha procurou manter o desenvolvimento concentrado no editor visual, sem acrescentar a complexidade de um servidor e de um banco de dados que não eram necessários para a primeira versão planejada.

# 5. Decisões técnicas iniciais

Ao final da primeira etapa, as decisões registradas foram:

| Item | Decisão do grupo |
|---|---|
| Problema | Pessoas sem conhecimento em Design Digital e desenvolvimento web podem ter dificuldade para compreender conceitos da área e organizar uma composição visual. |
| Público-alvo | Pessoas iniciantes ou leigas em Design Digital, com foco no contexto de estudantes e público jovem apresentado no prompt. |
| Tipo de aplicação | Aplicação web. |
| Stack escolhida | HTML, CSS, JavaScript e React. |
| Banco de dados | Não utilizar banco de dados na primeira versão. |
| Funcionalidades destacadas na síntese das decisões | Limpar ou reiniciar o layout, salvar com `localStorage`, oferecer orientações para iniciantes, realizar validações básicas, desenvolver identidade visual, considerar responsividade e fazer testes de usabilidade. |

# 6. Limitações, riscos e medidas preventivas

O grupo identificou riscos que poderiam comprometer o desenvolvimento ou a demonstração do LayoutLab. As probabilidades, os impactos e as medidas preventivas abaixo correspondem ao quadro registrado na primeira etapa.

| Risco identificado | Probabilidade | Impacto | Medida preventiva registrada |
|---|---|---|---|
| Escopo muito amplo | Alta | Alto | Definir um MVP. |
| Dificuldade no editor visual | Alta | Alto | Começar com seções e posições controladas. |
| Estado mal organizado | Média | Alto | Definir uma estrutura de dados centralizada. |
| Limitações do `localStorage` | Média | Médio | Armazenar apenas dados essenciais. |
| Problemas de responsividade | Média | Médio | Priorizar o computador e testar a visualização em telas menores. |
| Geração de código complexa | Alta | Alto | Deixar essa funcionalidade para uma etapa posterior. |
| Conflitos no trabalho em grupo | Média | Médio | Utilizar Git e GitHub e dividir as tarefas com clareza. |
| Interface confusa | Média | Alto | Realizar testes com usuários. |
| Falta de tempo | Alta | Alto | Planejar as etapas e congelar funcionalidades. |
| Dependências externas | Baixa | Médio | Utilizar poucas bibliotecas. |
| Problemas com imagens e fontes | Baixa | Médio | Usar recursos livres e otimizados. |

A análise evidencia que os maiores cuidados deveriam estar no controle do escopo, na complexidade do editor, na organização do estado e no tempo disponível. A recomendação geral foi desenvolver primeiro uma versão funcional e restrita, em vez de tentar reproduzir ferramentas profissionais completas.

# 7. Escopo definido para a primeira versão

## 7.1. O projeto deveria possuir

- Tela inicial com apresentação da ferramenta.
- Galeria de modelos de layout e opção para iniciar um layout vazio.
- Editor visual baseado em seções e componentes.
- Área central para visualização do layout.
- Menu lateral com elementos disponíveis e painel de propriedades do elemento selecionado.
- Inserção de títulos, textos, imagens, botões, links, cards e seções.
- Seleção visual e personalização de elementos.
- Edição de textos, cores, tamanhos e alinhamentos.
- Remoção de elementos e opção para limpar ou reiniciar o layout.
- Visualização do resultado sem os controles do editor.
- Salvamento e recuperação utilizando `localStorage`.
- Orientações para usuários iniciantes e validações básicas.
- Identidade visual própria e responsividade, principalmente na tela inicial e na visualização final.
- Organização em componentes React reutilizáveis, documentação das decisões e testes básicos de funcionamento e usabilidade.

## 7.2. O projeto não deveria possuir na primeira versão

- Sistema de cadastro, login ou perfis individuais.
- Banco de dados remoto ou backend em Node.js, Express ou Flask.
- Sincronização entre dispositivos, colaboração em tempo real ou compartilhamento por link.
- Biblioteca online de imagens ou upload ilimitado de arquivos.
- Sistema completo de camadas e posicionamento totalmente livre como no Figma.
- Redimensionamento avançado, animações complexas ou histórico completo de versões.
- Sistema avançado de desfazer e refazer.
- Inteligência artificial para gerar layouts automaticamente.
- Publicação automática de sites ou exportação para vários formatos.
- Geração automática de HTML e CSS na primeira versão.
- Integração com redes sociais, grande quantidade de modelos ou reprodução de todas as funcionalidades do Canva ou do Figma.
- Garantia de compatibilidade com navegadores muito antigos.

# 8. Perguntas Feitas pelo Grupo

## Pergunta 1: Qual ideia conectaria o jovem com o ensino?
* **Grupo:** Como poderíamos desenvolver um projeto que realmente despertasse o interesse dos estudantes do Ensino Médio, transformando o aprendizado de Design Digital e programação em algo interativo, prático e distante das aulas puramente teóricas?
* **Decisão do grupo:** O grupo concluiu que a melhor forma de engajar os jovens seria adotar a premissa do "aprender fazendo" (*hands-on*). Em vez de estudar conceitos estáticos, o aluno criaria uma página web de forma visual, compreendendo instantaneamente a utilidade prática de cada elemento.

## Pergunta 2: Qual aplicativo usaríamos como inspiração para o nosso sistema?
* **Grupo:** Para criar uma ferramenta de edição visual, deveríamos tentar copiar a complexidade de softwares profissionais de mercado como Canva, Figma ou FlutterFlow?
* **Decisão do grupo:** A equipe avaliou que tentar reproduzir ferramentas profissionais de grande escala inviabilizaria o desenvolvimento dentro do prazo escolar. Decidimos nos inspirar apenas na experiência visual de usabilidade desses softwares, mas simplificando drasticamente a interface — adotando um sistema focado em seções e componentes essenciais para garantir que o sistema fosse leve e funcional.

## Pergunta 3: Qual é o diferencial do nosso site?
* **Grupo:** Considerando que já existem diversos editores de layout na internet, qual seria o grande diferencial que faria o nosso projeto se destacar para o público e para a banca avaliadora?
* **Decisão do grupo:** O diferencial estabelecido pelo grupo foi o foco educacional e técnico da plataforma. O **LayoutLab** não serve apenas para desenhar layouts, mas funciona como uma ponte didática que une o design à estruturação de páginas web, contando com diferenciais exclusivos como um tutor de IA integrado (via Groq) treinado com materiais acadêmicos de design, exportação em código colável/pasta `.zip`, orientações em uma aba de *Design Guides* e uma identidade estética marcante (*Dark Deco*).

# 9. Evolução do projeto após a primeira etapa

Depois do planejamento, o grupo deu continuidade ao LayoutLab e transformou a proposta em uma aplicação voltada à criação visual de layouts e ao apoio de estudantes iniciantes em Design Digital. 

## 9.1. Aprimoramento da interface e dos recursos

A interface do editor foi simplificada e reorganizada para tornar a navegação mais clara para pessoas com pouca experiência em ferramentas de criação. A mudança manteve o propósito definido no planejamento: oferecer uma experiência introdutória e acessível, sem reproduzir a complexidade de um editor profissional.

Na evolução técnica, a base da aplicação foi desenvolvida com React, JavaScript, HTML e CSS, utilizando Vite como ferramenta de desenvolvimento e build. O `localStorage` foi utilizado para o salvamento no navegador, enquanto o tutor educacional foi integrado por meio da API do Groq. Essa integração representa uma ampliação em relação ao planejamento inicial, que priorizava uma aplicação sem serviços externos para o núcleo do editor.

Também foram acrescentados ou desenvolvidos os seguintes recursos:

| Recurso | Descrição | Relação com o planejamento inicial |
|---|---|---|
| Simplificação da interface | Revisão da organização visual e dos controles para facilitar o uso por iniciantes. | Reforça o requisito inicial de usabilidade e clareza. |
| Aba **Design Guides** | Área dedicada a diretrizes e orientações de Design Digital para apoiar o usuário durante a criação. | Desenvolve o caráter educacional que já estava previsto nas orientações para iniciantes. |
| Pré-visualização de templates | Janela pop-up que permite visualizar um modelo antes de carregá-lo no editor. | Aperfeiçoa a ideia inicial de galeria de modelos predefinidos. |
| Salvamento no navegador | Recurso para guardar e recuperar o projeto no próprio navegador. | Concretiza a proposta inicial de utilizar `localStorage`, sem depender de cadastro ou banco de dados remoto. |
| Exportação em arquivo ZIP | Opção para baixar o projeto em um arquivo compactado. | Amplia as possibilidades de guardar e transportar o trabalho. |
| Exportação em texto/código copiável | Opção para obter o conteúdo do projeto em formato que possa ser copiado para uso fora da plataforma. | Amplia a ideia inicial de exportação, que havia sido deixada fora da primeira versão em sua forma de geração automática de HTML e CSS. |
| Tutor de Inteligência Artificial | Integração de um tutor por meio da API do Groq. | Acrescenta uma forma de apoio educacional que não estava entre as funcionalidades decididas inicialmente. |

### Tutor de Inteligência Artificial e materiais didáticos

O LayoutLab passou a contar com um tutor de Inteligência Artificial integrado por meio da API do Groq. Para orientar as respostas relacionadas à disciplina, foram utilizados como referência os PDFs de Design Digital fornecidos pelo professor Amauri.

A finalidade do recurso é auxiliar o usuário com recomendações e orientações relacionadas à composição visual, aproximando a utilização prática do sistema dos conteúdos estudados em Design Digital. O tutor amplia a dimensão educacional da ferramenta: além de permitir a criação de layouts, o projeto também oferece apoio para que o usuário reflita sobre as escolhas que realiza.

É importante distinguir esse tutor da ideia de uma IA que gera layouts automaticamente. A geração automática de layouts aparecia entre os recursos que não fariam parte da primeira versão; o recurso implementado na prática é um tutor de apoio pedagógico ao usuário.

## 9.2. Identidade visual: conceito Dark Deco

A identidade visual da apresentação passou por um processo de definição. Inicialmente, o grupo considerou uma inspiração mais ampla no universo das histórias em quadrinhos. Posteriormente, essa referência foi direcionada ao universo do Batman e consolidada em uma proposta visual denominada **Dark Deco**.

O conceito combina uma atmosfera escura, contrastes marcantes e elementos de sofisticação geométrica. A intenção foi criar uma linguagem visual própria e coerente para a apresentação do projeto.

A identidade não ficou restrita à decoração do estande: a mesma diretriz visual foi aplicada ao site LayoutLab. Dessa maneira, a aplicação e o espaço físico da apresentação passaram a compartilhar uma linguagem visual, reforçando a unidade entre o produto digital e sua demonstração.

A escolha também se relaciona diretamente à disciplina de Design Digital, pois envolveu definir uma referência, estabelecer uma linguagem visual e buscar consistência entre diferentes materiais e ambientes.

## 9.3. Organização e dinâmica de apresentação na Etec de Portas Abertas

Além do desenvolvimento da aplicação, o grupo planejou a forma como os visitantes conheceriam o LayoutLab durante a Etec de Portas Abertas (EPA). Na organização do estande, a posição da mesa foi alterada com o objetivo de melhorar a circulação e facilitar a aproximação dos visitantes.

O grupo também preparou uma dinâmica interativa baseada em um jogo de charadas. A proposta foi estimular a participação do público por meio de perguntas e desafios, utilizando a ideia de **“aprender fazendo”**. Em vez de apresentar somente explicações, a dinâmica convidava os visitantes a participar e a se envolver com a atividade e com a ferramenta.

### Distribuição de doces como parte da dinâmica

A distribuição de doces foi relacionada à participação dos visitantes. Ela foi utilizada como recompensa vinculada ao envolvimento com as charadas e à interação com o LayoutLab, fazendo parte da estratégia de gamificação da apresentação.

Assim, as charadas, a experimentação da ferramenta e a recompensa foram pensadas como partes de uma mesma experiência para despertar curiosidade, aproximar o público do estande e incentivar o contato com o conteúdo educacional do projeto.

## 9.4. Síntese da evolução

A evolução do LayoutLab ocorreu em três frentes complementares:

1. **Produto digital:** simplificação da interface, pré-visualização de modelos, salvamento no navegador e opções de exportação.
2. **Apoio educacional:** aba Design Guides e tutor de IA integrado à API do Groq, com referência aos materiais de Design Digital fornecidos pelo professor.
3. **Experiência de apresentação:** identidade visual Dark Deco, organização do espaço do estande e dinâmica interativa com charadas e distribuição de doces.

Essas mudanças ampliaram a proposta inicial, mas mantiveram sua finalidade principal: aproximar estudantes iniciantes dos conceitos de Design Digital por meio de uma ferramenta visual e de uma experiência prática.

# 10. Comparação entre o planejamento inicial e a evolução

| Aspecto | Planejamento da primeira etapa | Evolução implementada no projeto |
|---|---|---|
| Público e finalidade | Estudantes e pessoas iniciantes em Design Digital; ferramenta educacional simplificada. | Mantida a finalidade de apoiar iniciantes, com recursos adicionais de orientação. |
| Interface | Editor visual com canvas, menu de elementos e painel de propriedades. | Interface reorganizada e simplificada para facilitar a navegação. |
| Modelos | Galeria de templates predefinidos. | Pré-visualização em pop-up antes de carregar o template. |
| Orientação | Mensagens e orientações simples para iniciantes. | Aba Design Guides e tutor de IA com referência aos PDFs da disciplina. |
| Salvamento | `localStorage`, sem banco de dados remoto. | Salvamento no navegador incorporado à aplicação. |
| Exportação | Geração automática de HTML e CSS fora do escopo da primeira versão. | Implementadas a exportação completa do projeto em arquivo compactado (ZIP) e a opção para copiar o código/texto gerado diretamente para uso externo. |
| Identidade visual | Previsão de uma identidade visual própria. | Conceito Dark Deco, inspirado no universo do Batman, aplicado ao site e ao estande. |
| Apresentação pública | Demonstração do fluxo principal do sistema na EPA. | Organização do espaço, reposicionamento da mesa e dinâmica de charadas com recompensa. |

# 11. Reflexão sobre o uso da Inteligência Artificial

A primeira interação com a Manus AI foi fundamental para nos ajudar a organizar a ideia inicial e enxergar pontos técnicos que poderiam ter passado despercebidos no começo — como a delimitação clara do público-alvo, a definição de um MVP, a estruturação dos elementos visuais como dados, a diferença entre posicionamento livre e organização por seções, além dos riscos de tentarmos abraçar recursos demais ao mesmo tempo.

Embora a IA tenha apresentado diversas alternativas técnicas, nós não adotamos suas recomendações de forma automática. Analisamos e comparamos as opções propostas e decidimos pela arquitetura com React e armazenamento local (`localStorage`), pois avaliamos que essa escolha se alinhava melhor à familiaridade técnica da nossa equipe e às necessidades reais do projeto naquele momento.

A evolução posterior do **LayoutLab** também deixa claro que não ficamos presos ao planejamento inicial. Ao longo do desenvolvimento, tomamos a iniciativa de ir além das sugestões da primeira etapa: implementamos a aba de *Design Guides*, a exportação em código colável e `.zip`, e integramos nosso próprio tutor de IA via API do Groq alimentado com materiais de Design Digital, além de criarmos a identidade visual *Dark Deco* e a dinâmica interativa para o evento. Essas decisões refletem o protagonismo do nosso grupo em adaptar e amadurecer o projeto diante dos desafios reais que encontramos na prática.

# 12. Conclusão

O LayoutLab começou como uma proposta de ferramenta web para auxiliar estudantes iniciantes a compreender e organizar elementos de Design Digital. Na primeira etapa, realizada em 16 de setembro de 2026, o grupo utilizou a Manus AI para analisar a ideia, discutir o público, levantar funcionalidades, comparar arquiteturas e identificar riscos. A decisão técnica inicial foi utilizar React, JavaScript, HTML e CSS, sem banco de dados remoto, priorizando uma solução compatível com os conhecimentos do grupo e com o escopo previsto.

Com a continuidade do trabalho, a aplicação recebeu uma interface simplificada, a aba Design Guides, a pré-visualização de templates, o salvamento no navegador e opções de exportação. A integração de um tutor de IA por meio da API do Groq, orientado por materiais de Design Digital fornecidos pelo professor Amauri, ampliou o apoio educacional oferecido pela ferramenta.

O projeto também ganhou uma identidade visual própria, denominada Dark Deco, aplicada tanto ao site quanto à ambientação do estande. Para a apresentação na EPA, o grupo reorganizou o espaço e desenvolveu uma dinâmica de charadas com distribuição de doces como incentivo à participação.

Dessa forma, o resultado descrito neste relatório reúne três dimensões: desenvolvimento de uma aplicação web, apoio ao aprendizado de Design Digital e planejamento de uma experiência de apresentação ao público. O processo partiu de uma etapa de planejamento apoiada por IA, mas as escolhas, adaptações e ampliações do produto foram realizadas pelo grupo ao longo do desenvolvimento.
