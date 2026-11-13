# CONECTA CONTÁBIL

## Documento de Descoberta de Requisitos -- MVP

**Projeto:** Conecta Contábil\
**Tipo:** Aplicação Web Responsiva\
**Segmento:** Pequenos escritórios de contabilidade\
**Público-alvo:** Escritórios contábeis e empresas clientes\
**Versão:** 1.0

------------------------------------------------------------------------

# 01. CONTEXT -- Contexto e problemática

Pequenos escritórios de contabilidade enfrentam diariamente dificuldades
na comunicação e no compartilhamento de documentos com seus clientes.
Grande parte dessas interações acontece por meio de aplicativos de
mensagens, e-mails e outros canais descentralizados, ocasionando
retrabalho, perda de informações, dificuldade de localização de arquivos
e solicitações repetitivas.

Além disso, muitos empresários não sabem quais documentos estão
disponíveis, quais precisam encaminhar ao escritório ou quais são
necessários para suas atividades contábeis e administrativas.

O **Conecta Contábil** propõe uma aplicação web responsiva que funcione
como um canal centralizado de relacionamento entre o escritório contábil
e seus clientes, permitindo disponibilizar, consultar, baixar, solicitar
e encaminhar documentos de maneira simples e organizada.

O objetivo do MVP é reduzir tarefas operacionais repetitivas, melhorar a
comunicação e facilitar o acesso às informações, sem substituir os
sistemas contábeis já utilizados pelos escritórios.

# 02. PERSON -- Personas

As personas a seguir foram geradas com auxílio de IA e representam
hipóteses de usuários potenciais do sistema. Não correspondem a
entrevistas reais.

## Persona 01 -- Primária: Carlos Henrique

-   **Idade:** 42 anos.
-   **Profissão:** Contador e proprietário de escritório.
-   **Cidade:** Lages/SC.
-   **Experiência:** 15 anos na área contábil.
-   **Familiaridade com tecnologia:** Intermediária.

**Dor principal:** Perde muito tempo atendendo solicitações repetitivas
de clientes, reenviando documentos e procurando arquivos em conversas de
WhatsApp e e-mails.

**Cenário de uso:** Durante o expediente, Carlos precisa disponibilizar
documentos aos clientes, solicitar arquivos necessários para o
fechamento contábil e consultar quais empresas ainda possuem pendências
documentais.

**Métrica de sucesso:** Reduzir em pelo menos 30% o tempo gasto com
solicitações e disponibilização de documentos.

## Persona 02 -- Secundária: Mariana Oliveira

-   **Idade:** 35 anos.
-   **Profissão:** Proprietária de comércio varejista.
-   **Cidade:** Lages/SC.
-   **Familiaridade com tecnologia:** Básica a intermediária.

**Dor principal:** Não sabe onde encontrar documentos disponibilizados
pelo contador e frequentemente precisa solicitá-los novamente.

**Cenário de uso:** Durante sua rotina empresarial, precisa acessar
documentos como contratos, guias, comprovantes, certidões e outros
arquivos disponibilizados pelo escritório contábil.

**Métrica de sucesso:** Encontrar e baixar um documento necessário em
menos de dois minutos, sem precisar entrar em contato com o escritório.

## Persona 03 -- Secundária: Roberto Almeida

-   **Idade:** 29 anos.
-   **Profissão:** Auxiliar administrativo de empresa cliente.
-   **Cidade:** Correia Pinto/SC.
-   **Familiaridade com tecnologia:** Avançada.

**Dor principal:** Precisa organizar e encaminhar documentos mensalmente
ao escritório contábil, mas não possui um canal padronizado para
acompanhar o que já foi enviado e o que ainda está pendente.

**Cenário de uso:** Acessa o aplicativo pelo computador ou celular,
verifica solicitações do escritório, envia os arquivos necessários e
acompanha o andamento das pendências.

**Métrica de sucesso:** Conseguir acompanhar todas as solicitações
documentais da empresa em um único ambiente.

# 03. ENTREVISTA SIMULADA -- Descoberta de necessidades

**Objetivo:** Simular, com auxílio de IA, uma entrevista com um
profissional de contabilidade para identificar possíveis dificuldades na
comunicação e no compartilhamento de documentos com clientes.

**Entrevistado simulado:** Carlos Henrique -- Contador, 42 anos.

**Observação:** Esta entrevista foi inteiramente simulada por IA,
conforme a proposta da atividade. As respostas são hipóteses para
orientar a descoberta de requisitos, não dados coletados de um usuário
real.

### Pergunta 01 -- Como acontece atualmente a comunicação com seus clientes quando precisam de documentos?

**Resposta simulada:**\
A maior parte acontece pelo WhatsApp. Alguns clientes utilizam e-mail,
mas normalmente preferem mandar mensagens. Quando precisam de algum
documento, entram em contato diretamente com o escritório.

### Pergunta 02 -- Quais são as maiores dificuldades nesse processo?

**Resposta simulada:**\
O maior problema é a repetição. Muitos clientes solicitam documentos que
já foram enviados anteriormente. Precisamos procurar nas conversas ou
nos arquivos para encaminhar novamente. Isso acaba tomando bastante
tempo da equipe.

### Pergunta 03 -- Como você organiza os documentos que disponibiliza aos clientes?

**Resposta simulada:**\
Temos pastas no computador e documentos armazenados nos sistemas que
utilizamos. Entretanto, não existe um local único onde o cliente possa
acessar tudo sozinho.

### Pergunta 04 -- Se existisse um aplicativo para centralizar esses documentos, o que seria mais importante?

**Resposta simulada:**\
Seria importante que cada cliente tivesse seu próprio acesso, pudesse
consultar os documentos disponíveis, baixar arquivos e também visualizar
quando o escritório estivesse solicitando alguma documentação.

### Pergunta 05 -- Qual seria o principal benefício que você esperaria dessa solução?

**Resposta simulada:**\
Reduzir o volume de mensagens e ligações sobre documentos, economizar
tempo da equipe e deixar o relacionamento com os clientes mais
organizado.

### Principais dores identificadas na simulação

1.  Solicitações repetitivas de documentos.
2.  Informações descentralizadas em diferentes canais.
3.  Dificuldade para localizar arquivos anteriormente enviados.
4.  Falta de acompanhamento das pendências documentais.
5.  Tempo excessivo gasto em atividades operacionais.

# 04. RF -- Requisitos Funcionais

Os requisitos funcionais representam as ações e funcionalidades que o
sistema deverá executar.

  -----------------------------------------------------------------------
  ID                                  Requisito funcional
  ----------------------------------- -----------------------------------
  RF01                                O sistema deverá permitir o
                                      cadastro, edição, consulta e
                                      exclusão de empresas clientes,
                                      contendo razão social, nome
                                      fantasia e CNPJ.

  RF02                                O sistema deverá permitir o
                                      cadastro, edição, consulta e
                                      exclusão de categorias para
                                      organização dos documentos.

  RF03                                O sistema deverá permitir que o
                                      escritório disponibilize documentos
                                      digitais vinculados a uma empresa
                                      cliente e a uma categoria.

  RF04                                O sistema deverá permitir que o
                                      cliente consulte e faça download
                                      dos documentos disponibilizados
                                      pelo escritório.

  RF05                                O sistema deverá permitir que o
                                      escritório registre solicitações de
                                      documentos vinculadas a uma empresa
                                      cliente, informando descrição e
                                      prazo de entrega.

  RF06                                O sistema deverá permitir que o
                                      cliente envie documentos digitais
                                      em resposta às solicitações
                                      realizadas pelo escritório.

  RF07                                O sistema deverá permitir a
                                      consulta e o acompanhamento do
                                      status das solicitações
                                      documentais, identificando
                                      pendências e documentos enviados.

  RF08                                O sistema deverá permitir
                                      autenticação de usuários e controle
                                      de acesso conforme seus respectivos
                                      perfis, diferenciando escritório e
                                      cliente.
  -----------------------------------------------------------------------

# 05. RNF -- Requisitos Não Funcionais

Os requisitos não funcionais definem critérios de qualidade, segurança,
desempenho e usabilidade da aplicação.

  -----------------------------------------------------------------------
  ID                                  Requisito não funcional
  ----------------------------------- -----------------------------------
  RNF01                               A interface deverá ser responsiva,
                                      permitindo utilização em
                                      computadores, tablets e
                                      smartphones, com largura mínima de
                                      320 pixels.

  RNF02                               As principais páginas e consultas
                                      deverão apresentar carregamento em
                                      até 3 segundos em condições normais
                                      de conexão.

  RNF03                               O sistema deverá implementar
                                      autenticação e controle de acesso,
                                      garantindo que cada cliente
                                      visualize exclusivamente os
                                      documentos e solicitações
                                      vinculados à sua empresa.

  RNF04                               Os dados pessoais e documentos
                                      deverão ser protegidos, observando
                                      os princípios e requisitos
                                      aplicáveis da Lei Geral de Proteção
                                      de Dados (LGPD).

  RNF05                               Os documentos e informações
                                      cadastrados deverão possuir
                                      persistência em banco de dados,
                                      mantendo os registros disponíveis
                                      após encerramento e reinicialização
                                      da aplicação.
  -----------------------------------------------------------------------

# 06. US -- Histórias de Usuário

As histórias de usuário descrevem as funcionalidades sob a perspectiva
de quem utilizará o sistema.

## US01 -- Cadastro de empresas clientes

**Prioridade:** MUST HAVE\
**Estimativa:** 3 pontos.

**Como** administrador do escritório contábil,\
**quero** cadastrar e gerenciar empresas clientes,\
**para** organizar os documentos e solicitações de maneira
individualizada para cada empresa.

**Critérios de aceitação:**

-   [ ] AC01: O sistema deverá exigir razão social e CNPJ para cadastrar
    uma empresa.
-   [ ] AC02: O sistema deverá validar o formato do CNPJ informado.
-   [ ] AC03: O sistema deverá impedir o cadastro de duas empresas com o
    mesmo CNPJ no mesmo escritório.
-   [ ] AC04: Após o cadastro, a empresa deverá aparecer na listagem de
    clientes.
-   [ ] AC05: O administrador deverá conseguir editar e excluir os dados
    de empresas cadastradas.

## US02 -- Disponibilização e consulta de documentos

**Prioridade:** MUST HAVE\
**Estimativa:** 5 pontos.

**Como** profissional do escritório contábil,\
**quero** disponibilizar documentos digitais vinculados a uma empresa
cliente,\
**para** permitir que o cliente consulte e baixe seus documentos sempre
que necessário.

**Critérios de aceitação:**

-   [ ] AC01: O sistema deverá permitir selecionar a empresa cliente e a
    categoria do documento antes de realizar o envio.
-   [ ] AC02: O sistema deverá permitir anexar arquivos em formatos PDF,
    JPG e PNG.
-   [ ] AC03: Após o envio, o documento deverá aparecer na área de
    documentos da empresa correspondente.
-   [ ] AC04: O cliente deverá conseguir visualizar e baixar os
    documentos disponibilizados para sua empresa.
-   [ ] AC05: O sistema deverá impedir que um cliente visualize
    documentos pertencentes a outra empresa.

## US03 -- Solicitação e envio de documentos

**Prioridade:** MUST HAVE\
**Estimativa:** 5 pontos.

**Como** profissional do escritório contábil,\
**quero** solicitar documentos aos clientes e acompanhar o recebimento
dos arquivos,\
**para** organizar as pendências documentais e facilitar as atividades
contábeis.

**Critérios de aceitação:**

-   [ ] AC01: O escritório deverá conseguir criar uma solicitação
    vinculada a uma empresa cliente, contendo descrição e prazo de
    entrega.
-   [ ] AC02: O cliente deverá conseguir visualizar as solicitações
    pendentes em sua área de acesso.
-   [ ] AC03: O cliente deverá conseguir anexar um documento para
    responder à solicitação.
-   [ ] AC04: Após o envio do arquivo, o status da solicitação deverá
    ser atualizado para "Documento enviado".
-   [ ] AC05: O escritório deverá conseguir consultar os documentos
    recebidos e acompanhar o status das solicitações.

# 07. PRIORIZAÇÃO -- MoSCoW

A metodologia MoSCoW foi utilizada para definir as funcionalidades
prioritárias do MVP.

  -----------------------------------------------------------------------
  Prioridade                          Funcionalidades
  ----------------------------------- -----------------------------------
  **MUST HAVE**                       Cadastro de empresas, autenticação,
                                      disponibilização de documentos,
                                      consulta e download, solicitação e
                                      envio de documentos.

  **SHOULD HAVE**                     Organização avançada por
                                      categorias, filtros por período e
                                      notificações de novas solicitações.

  **COULD HAVE**                      Dashboard com indicadores de
                                      pendências, histórico de
                                      movimentações e personalização
                                      visual por escritório.

  **WON'T HAVE**                      Integração automática com sistemas
                                      contábeis, emissão de notas
                                      fiscais, cálculo de impostos e
                                      geração automática de obrigações
                                      acessórias.
  -----------------------------------------------------------------------

# 08. OUT -- Fora do escopo do MVP

Para manter o desenvolvimento inicial simples e viável, algumas
funcionalidades não serão contempladas nesta primeira versão:

1.  Substituição dos sistemas contábeis utilizados pelos escritórios.
2.  Cálculo automático de tributos e geração de guias de impostos.
3.  Emissão de notas fiscais.
4.  Integração automática com plataformas governamentais, como e-CAC e
    Receita Federal.
5.  Integração automática com WhatsApp ou outros aplicativos de
    mensagens.
6.  Assinatura digital de documentos.
7.  Aplicativo nativo para Android ou iOS.
8.  Inteligência artificial para interpretação, classificação ou análise
    automática de documentos.

# 09. VALIDAÇÃO HUMANA E CONSIDERAÇÕES FINAIS

O documento foi elaborado com auxílio de inteligência artificial,
seguindo as etapas de descoberta e documentação de requisitos
apresentadas na aula.

As personas e a entrevista simulada foram geradas por IA e representam
hipóteses de usuários e necessidades que poderão ser investigadas em uma
etapa posterior.

Os requisitos foram organizados considerando a problemática proposta,
buscando manter clareza, coerência e critérios verificáveis. Também
foram considerados aspectos de segurança, controle de acesso e proteção
de dados, importantes para uma aplicação que manipula documentos
empresariais.

O **Conecta Contábil** pretende oferecer uma solução simples e acessível
para centralizar o relacionamento documental entre escritórios contábeis
e empresas clientes, reduzindo atividades repetitivas e melhorando a
organização das informações.

**Objetivo principal do MVP:** demonstrar que um canal digital
centralizado pode simplificar a disponibilização, consulta e solicitação
de documentos, proporcionando economia de tempo para o escritório e
maior autonomia para seus clientes.

------------------------------------------------------------------------

**Projeto acadêmico -- Prototipação Rápida de Aplicações com IA**

------------------------------------------------------------------------

# 10. AULA 02 -- UX/UI E PROTOTIPAÇÃO DO MVP

## 10.1 Objetivo desta etapa

A partir dos requisitos, personas e histórias de usuário definidos na
Aula 01, esta etapa transforma as necessidades do Conecta Contábil em
uma proposta de interface visual navegável.

Um requisito descreve **o que** o sistema precisa fazer. O protótipo
demonstra **como** o usuário poderá realizar essas tarefas.

O objetivo é produzir quatro telas em alta fidelidade, com navegação
funcional entre elas, priorizando clareza, consistência visual,
acessibilidade básica e experiência mobile-first.

**Importante:** este material especifica um protótipo acadêmico para
validação de UX/UI. Não representa ainda a implementação definitiva do
sistema, banco de dados, autenticação real ou armazenamento efetivo de
documentos.

## 10.2 Diretrizes de UX

### UX e UI no Conecta Contábil

-   **UX (User Experience):** organiza a jornada, as tarefas, a
    navegação e a resolução das dores dos usuários.
-   **UI (User Interface):** define a apresentação visual, cores,
    tipografia, componentes, espaçamentos e estados da interface.

A experiência deve atender principalmente aos dois perfis de uso:

1.  **Profissional do escritório contábil:** precisa administrar
    clientes, disponibilizar documentos e acompanhar solicitações com
    agilidade.
2.  **Empresa cliente:** precisa localizar documentos, baixar arquivos e
    entender quais documentos foram solicitados pelo escritório.

### Jornada principal do MVP

1.  O profissional acessa o painel do escritório.
2.  Localiza ou seleciona uma empresa cliente.
3.  Consulta os documentos da empresa ou disponibiliza um novo arquivo.
4.  Cria uma solicitação documental com descrição e prazo.
5.  Acompanha se o cliente enviou o documento solicitado.

A interface deve reduzir a dependência de mensagens e contatos
repetitivos, mantendo as informações organizadas por empresa.

## 10.3 Mapa de telas e navegação

As quatro telas essenciais escolhidas para o protótipo são:

``` text
CONECTA CONTÁBIL
│
├── 01. Dashboard – Painel do escritório
│   ├── Indicadores gerais
│   ├── Atividades recentes
│   └── Atalhos para clientes, documentos e solicitações
│
├── 02. Gestão de clientes
│   ├── Listagem e pesquisa de empresas
│   ├── Cadastro de novo cliente
│   └── Acesso aos dados e documentos da empresa
│
├── 03. Central de documentos
│   ├── Seleção da empresa
│   ├── Filtros por categoria e período
│   ├── Listagem de arquivos
│   ├── Disponibilização de documento
│   └── Ação de visualizar ou baixar
│
└── 04. Solicitações documentais
    ├── Listagem de solicitações
    ├── Criação de solicitação
    ├── Definição de prazo
    └── Acompanhamento de status
```

**Regra de navegação:** todas as telas devem possuir navegação principal
visível e permitir retorno ao Dashboard. Nenhuma tela pode deixar o
usuário preso em um fluxo sem saída. As quatro telas devem ser
alcançáveis em até dois níveis de navegação a partir do painel.

### Relação entre telas e requisitos

  Tela                       Requisitos relacionados   Histórias relacionadas
  -------------------------- ------------------------- ------------------------
  Dashboard                  RF01, RF03, RF05, RF07    US01, US02, US03
  Gestão de clientes         RF01                      US01
  Central de documentos      RF02, RF03, RF04          US02
  Solicitações documentais   RF05, RF06, RF07          US03

A autenticação prevista no RF08 deverá ser considerada como contexto de
acesso, mas a tela de login não faz parte das quatro telas principais
solicitadas nesta etapa.

## 10.4 Wireframes de baixa fidelidade (Lo-Fi)

Antes da definição visual final, a estrutura das quatro telas deverá ser
validada sem depender de cores, imagens ou detalhes estéticos.

### Lo-Fi 01 -- Dashboard

-   Cabeçalho com identificação do Conecta Contábil e usuário logado.
-   Menu lateral no desktop e navegação adaptada no celular.
-   Título "Visão geral".
-   Cards com total de clientes, documentos disponibilizados,
    solicitações pendentes e documentos recebidos.
-   Área de atividades recentes.
-   Atalhos para as áreas principais.

### Lo-Fi 02 -- Gestão de clientes

-   Cabeçalho com título "Clientes".
-   Campo de pesquisa por razão social, nome fantasia ou CNPJ.
-   Botão "Novo cliente".
-   Listagem com razão social, CNPJ e situação.
-   Ações para visualizar, editar e acessar os documentos da empresa.
-   Formulário de cadastro com razão social, nome fantasia e CNPJ.

### Lo-Fi 03 -- Central de documentos

-   Cabeçalho com título "Documentos".
-   Seletor de empresa cliente.
-   Filtros por categoria e período.
-   Botão "Enviar documento".
-   Listagem com nome do arquivo, categoria, data e empresa vinculada.
-   Ações de visualizar e baixar.
-   Formulário ou área de envio com seleção de arquivo e categoria.

### Lo-Fi 04 -- Solicitações documentais

-   Cabeçalho com título "Solicitações".
-   Indicadores ou filtros de pendentes, enviados e concluídos.
-   Listagem com empresa, descrição, prazo e status.
-   Botão "Nova solicitação".
-   Formulário com empresa, descrição da documentação solicitada e
    prazo.
-   Ação para consultar o documento recebido e atualizar o
    acompanhamento.

## 10.5 Tokens visuais e identidade da interface

A identidade visual proposta busca transmitir organização, confiança,
clareza e profissionalismo, características importantes para um sistema
utilizado por escritórios contábeis e empresas clientes.

### Paleta de cores proposta

  Token          Cor         Aplicação
  -------------- ----------- -----------------------------------------------
  Primary        `#2457A6`   Navegação, identidade e ações principais
  Primary Dark   `#173B73`   Hover e elementos de maior contraste
  Accent         `#16A6A1`   Destaques secundários e indicadores positivos
  Background     `#F5F7FA`   Fundo geral da aplicação
  Surface        `#FFFFFF`   Cards, formulários e painéis
  Text           `#1F2937`   Textos principais
  Text Muted     `#64748B`   Informações auxiliares
  Border         `#E2E8F0`   Divisórias e contornos
  Success        `#15803D`   Concluído e recebido
  Warning        `#D97706`   Pendente e atenção
  Danger         `#DC2626`   Erros e ações destrutivas

### Tipografia

-   Família sugerida: Inter ou outra fonte sans-serif de boa
    legibilidade.
-   Título principal: 28 a 32 px.
-   Título de seção: 20 a 24 px.
-   Subtítulos: 16 a 18 px.
-   Texto padrão: 16 px.
-   Texto auxiliar: mínimo de 13 a 14 px, respeitando legibilidade e
    contraste.

### Espaçamento e componentes

-   Utilizar escala baseada em múltiplos de 4 px: 4, 8, 12, 16, 24, 32 e
    48 px.
-   Bordas arredondadas: 6 a 8 px para campos e botões; 10 a 12 px para
    cards.
-   Botões e áreas de toque com altura mínima recomendada de 44 px.
-   Manter padrões consistentes de botões primários, secundários,
    campos, tabelas, cards e indicadores de status.
-   Utilizar ícones acompanhados de rótulos quando necessário para
    evitar ambiguidades.

## 10.6 Diretrizes responsivas e acessibilidade

O protótipo deverá adotar estratégia **mobile-first**, expandindo o
layout para telas maiores.

-   **Mobile:** menu compacto ou navegação adaptada, conteúdo em uma
    coluna e ações acessíveis por toque.
-   **Tablet:** organização em duas colunas quando houver espaço
    suficiente.
-   **Desktop:** menu lateral, área de conteúdo ampla e tabelas com boa
    leitura.

### Acessibilidade -- princípios POUR

-   **Perceptível:** informações e estados não devem ser comunicados
    somente por cores; utilizar textos e ícones.
-   **Operável:** elementos interativos devem permitir navegação por
    teclado, com foco visível.
-   **Compreensível:** formulários devem ter rótulos claros e mensagens
    de erro que orientem a correção.
-   **Robusto:** utilizar estrutura semântica e componentes compatíveis
    com tecnologias assistivas na implementação.

Critérios visuais básicos: - Buscar contraste mínimo WCAG AA de 4,5:1
para textos normais. - Manter áreas de toque com pelo menos 44 × 44 px
sempre que possível. - Não utilizar somente placeholders como
identificação dos campos. - Prever estados de foco, hover, desabilitado,
carregamento, vazio e erro.

## 10.7 Especificação das quatro telas em alta fidelidade (Hi-Fi)

As telas deverão compartilhar o mesmo sistema visual, menu, cabeçalho,
padrões de componentes e comportamento responsivo.

### Tela 01 -- Dashboard / Visão geral

**Objetivo:** permitir que o profissional do escritório entenda
rapidamente a situação geral dos clientes e das movimentações
documentais.

**Conteúdo obrigatório:** - Identificação "Conecta Contábil". -
Navegação para Visão geral, Clientes, Documentos e Solicitações. -
Saudação e título "Visão geral". - Cards de indicadores: total de
clientes, documentos disponibilizados, solicitações pendentes e
documentos recebidos. - Lista de atividades recentes com empresa, ação e
data. - Atalhos para cadastrar cliente, enviar documento e criar
solicitação.

**Elemento de maior hierarquia:** os indicadores gerais e,
especialmente, a quantidade de solicitações pendentes.

**Ações de navegação:** menu Clientes abre a Tela 02; Documentos abre a
Tela 03; Solicitações abre a Tela 04.

### Tela 02 -- Gestão de clientes

**Objetivo:** centralizar o cadastro e a consulta das empresas atendidas
pelo escritório.

**Conteúdo obrigatório:** - Título "Clientes". - Campo de pesquisa. -
Botão destacado "Novo cliente". - Listagem de empresas com razão social,
nome fantasia, CNPJ e situação. - Ações de visualizar/editar. -
Formulário de cadastro com razão social, nome fantasia e CNPJ. -
Mensagens de validação para campos obrigatórios e CNPJ inválido.

**Elemento de maior hierarquia:** botão "Novo cliente" e identificação
clara da listagem.

**Ações de navegação:** Dashboard retorna à Tela 01; Documentos e
Solicitações abrem as respectivas telas.

### Tela 03 -- Central de documentos

**Objetivo:** facilitar a organização e a disponibilização de arquivos
para cada empresa cliente.

**Conteúdo obrigatório:** - Título "Documentos". - Seletor de empresa
cliente. - Filtros por categoria e período. - Botão "Enviar
documento". - Listagem com nome, categoria, empresa, data e formato do
arquivo. - Ações de visualizar e baixar. - Área de envio com seleção de
arquivo e categoria. - Indicação dos formatos aceitos no requisito: PDF,
JPG e PNG.

**Elemento de maior hierarquia:** botão "Enviar documento" e
identificação da empresa selecionada.

**Ações de navegação:** acesso às demais áreas pelo menu principal.

### Tela 04 -- Solicitações documentais

**Objetivo:** permitir que o escritório crie solicitações e acompanhe o
recebimento dos documentos.

**Conteúdo obrigatório:** - Título "Solicitações". - Filtros ou
indicadores de pendentes, documentos enviados e concluídos. - Botão
"Nova solicitação". - Listagem com empresa, descrição, prazo e status. -
Formulário para selecionar empresa, informar descrição e definir
prazo. - Status visual com texto e cor: "Pendente", "Documento enviado"
e "Concluído". - Ação para consultar o documento recebido.

**Elemento de maior hierarquia:** solicitações pendentes e botão "Nova
solicitação".

**Ações de navegação:** acesso às demais áreas pelo menu principal.

## 10.8 Orientação para geração com IA -- Prompt CTQF

O prompt abaixo deverá ser utilizado na ferramenta de prototipação
escolhida. A geração deve priorizar consistência entre telas e
navegação, não apenas imagens isoladas.

### Prompt base do projeto

**C -- Contexto**

Estamos criando o protótipo de alta fidelidade do Conecta Contábil, uma
aplicação web responsiva para pequenos escritórios de contabilidade e
suas empresas clientes. O sistema centraliza o cadastro de empresas, a
disponibilização e consulta de documentos e as solicitações de
documentos.

A persona principal é um contador ou profissional de escritório contábil
que precisa reduzir tarefas repetitivas e organizar o relacionamento
documental com seus clientes. O usuário secundário é o responsável de
uma empresa cliente, que precisa localizar documentos e responder às
solicitações do escritório.

**T -- Tarefa**

Crie quatro telas de alta fidelidade para o MVP:

1.  Dashboard -- Visão geral do escritório.
2.  Clientes -- Cadastro, pesquisa e gerenciamento de empresas.
3.  Documentos -- Consulta, organização, envio e download de arquivos.
4.  Solicitações -- Criação e acompanhamento de solicitações
    documentais.

As quatro telas devem representar o mesmo produto, com identidade visual
e componentes consistentes. Não criar telas desconectadas ou com estilos
diferentes.

**Q -- Quem**

Atue como um designer UX/UI sênior especializado em sistemas SaaS B2B,
aplicações administrativas e design responsivo. Considere usuários de
escritórios contábeis com familiaridade tecnológica intermediária e
empresários que precisam de uma experiência simples e objetiva.

**F -- Formato e requisitos**

-   Criar interface moderna, profissional, limpa e organizada.
-   Utilizar a paleta e os tokens definidos na seção 10.5.
-   Adotar estratégia mobile-first, com adaptação para desktop.
-   Criar menu de navegação funcional entre as quatro telas.
-   Manter cabeçalho, menu, botões, cards, campos e tabelas
    consistentes.
-   Utilizar dados fictícios realistas para demonstrar o funcionamento.
-   Não apresentar dados pessoais reais.
-   Utilizar textos em português do Brasil.
-   Dar destaque visual às ações principais de cada tela.
-   Prever estados vazios, carregamento, erro e confirmação quando
    aplicável.
-   Manter contraste adequado, rótulos visíveis e foco perceptível.
-   Não inventar funcionalidades fora do escopo definido nos requisitos.
-   A navegação e as ações demonstrativas podem utilizar dados
    simulados; não afirmar que existe integração real com banco de dados
    ou armazenamento.

**Resultado esperado:** um protótipo navegável contendo as quatro telas
principais do Conecta Contábil, pronto para avaliação visual e teste
heurístico.

### Instruções específicas para cada tela

Após aplicar o prompt base, gerar ou ajustar cada tela conforme sua
especificação na seção 10.7. Se a ferramenta aceitar geração de
múltiplas páginas em um único projeto, manter as quatro telas no mesmo
projeto e compartilhar os componentes.

Se a ferramenta gerar uma tela por vez, reutilizar o prompt base e
acrescentar a especificação da tela correspondente, preservando os
mesmos tokens e padrões visuais.

## 10.9 Navegação funcional do protótipo

A navegação entre as quatro telas é um item obrigatório da atividade.

  -----------------------------------------------------------------------
  Origem                  Ação                    Destino
  ----------------------- ----------------------- -----------------------
  Dashboard               Clicar em Clientes      Gestão de clientes

  Dashboard               Clicar em Documentos    Central de documentos

  Dashboard               Clicar em Solicitações  Solicitações
                                                  documentais

  Clientes                Clicar em Novo cliente  Formulário de cadastro
                                                  na tela de clientes

  Clientes                Acessar documentos de   Central de documentos
                          uma empresa             com empresa selecionada

  Documentos              Clicar em Solicitações  Solicitações
                                                  documentais

  Solicitações            Clicar em Nova          Formulário de criação
                          solicitação             na tela de solicitações

  Todas as telas          Clicar em Visão geral   Dashboard
  -----------------------------------------------------------------------

Para fins de prototipação, formulários, filtros, upload e botões podem
utilizar interações simuladas. O importante é demonstrar o fluxo de
navegação e os estados visuais sem sugerir que operações de backend já
foram implementadas.

## 10.10 Teste heurístico -- Avaliação das quatro telas

A avaliação deverá ser feita individualmente em cada tela, considerando
as cinco heurísticas destacadas na atividade:

1.  **Visibilidade do status do sistema:** o usuário recebe retorno ao
    clicar, salvar, enviar ou realizar uma ação?
2.  **Correspondência com o mundo real:** os termos utilizados são
    familiares ao público contábil e empresarial?
3.  **Controle e liberdade do usuário:** é possível cancelar, voltar ou
    corrigir uma ação?
4.  **Consistência e padrões:** botões, cores, ícones, menus e
    componentes mantêm o mesmo comportamento?
5.  **Prevenção de erros:** formulários orientam o preenchimento e ações
    destrutivas possuem confirmação?

### Checklist de avaliação

#### Tela 01 -- Dashboard

-   [ ] Indicadores e informações possuem hierarquia clara.
-   [ ] Os status das solicitações são compreensíveis.
-   [ ] Os atalhos levam às telas corretas.
-   [ ] A navegação mantém padrões consistentes.
-   [ ] As informações não ficam visualmente sobrecarregadas.

#### Tela 02 -- Gestão de clientes

-   [ ] A pesquisa e a listagem são fáceis de compreender.
-   [ ] O cadastro informa quais campos são obrigatórios.
-   [ ] Erros de preenchimento são apresentados claramente.
-   [ ] A edição e a exclusão possuem controle e confirmação adequados.
-   [ ] A navegação de retorno está disponível.

#### Tela 03 -- Central de documentos

-   [ ] A empresa selecionada fica claramente identificada.
-   [ ] Nome, categoria e data facilitam localizar arquivos.
-   [ ] O envio apresenta retorno visual ao usuário.
-   [ ] Os formatos permitidos são informados.
-   [ ] As ações de visualizar e baixar são claras.

#### Tela 04 -- Solicitações documentais

-   [ ] Os status são apresentados com texto e identificação visual.
-   [ ] A empresa vinculada à solicitação fica evidente.
-   [ ] A descrição e o prazo são fáceis de identificar.
-   [ ] O formulário apresenta validações claras.
-   [ ] O usuário consegue voltar ou cancelar a criação.

**Registro do teste:** para cada tela, anotar eventuais violações,
classificar como crítico, importante ou menor e corrigir primeiro os
problemas que bloqueiam a utilização.

O teste heurístico é uma avaliação inicial e não substitui testes com
usuários reais.

## 10.11 Checklist geral de entrega da Aula 02

-   [ ] Mapa de telas documentado.
-   [ ] Quatro wireframes Lo-Fi elaborados.
-   [ ] Tokens visuais documentados.
-   [ ] Quatro telas Hi-Fi geradas com auxílio de IA.
-   [ ] Navegação funcional entre as quatro telas.
-   [ ] Layout responsivo para celular e desktop.
-   [ ] Teste heurístico aplicado individualmente em cada tela.
-   [ ] Problemas críticos identificados e corrigidos.
-   [ ] Resultado revisado humanamente antes da entrega.

## 10.12 Validação humana e considerações da Aula 02

A inteligência artificial será utilizada como aceleradora da criação dos
layouts e componentes, mas suas sugestões deverão ser avaliadas antes de
serem incorporadas ao protótipo.

A revisão deverá observar principalmente:

-   Se cada tela atende aos requisitos e às histórias de usuário
    definidos na Aula 01.
-   Se a navegação representa um fluxo coerente e sem caminhos sem
    saída.
-   Se os componentes possuem aparência e comportamento consistentes.
-   Se os textos e ações são adequados ao contexto de escritórios
    contábeis.
-   Se a interface funciona em diferentes tamanhos de tela.
-   Se os elementos gerados pela IA são compreensíveis e podem ser
    justificados pelo aluno.

A geração visual não substitui a validação humana. O protótipo deverá
ser revisado, ajustado e testado antes de ser considerado concluído.

**Objetivo da etapa:** demonstrar visualmente como o Conecta Contábil
poderá simplificar a gestão de clientes, a disponibilização de
documentos e o acompanhamento de solicitações, transformando os
requisitos documentados em uma experiência de uso clara e navegável.

------------------------------------------------------------------------

**Projeto acadêmico -- Prototipação Rápida de Aplicações com IA -- Aulas
01 e 02**
