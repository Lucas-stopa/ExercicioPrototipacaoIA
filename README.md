# CONECTA CONTÁBIL
## Documento de Descoberta de Requisitos – MVP

**Projeto:** Conecta Contábil  
**Tipo:** Aplicação Web Responsiva  
**Segmento:** Pequenos escritórios de contabilidade  
**Público-alvo:** Escritórios contábeis e empresas clientes  
**Versão:** 1.0

---

# 01. CONTEXT – Contexto e problemática

Pequenos escritórios de contabilidade enfrentam diariamente dificuldades na comunicação e no compartilhamento de documentos com seus clientes. Grande parte dessas interações acontece por meio de aplicativos de mensagens, e-mails e outros canais descentralizados, ocasionando retrabalho, perda de informações, dificuldade de localização de arquivos e solicitações repetitivas.

Além disso, muitos empresários não sabem quais documentos estão disponíveis, quais precisam encaminhar ao escritório ou quais são necessários para suas atividades contábeis e administrativas.

O **Conecta Contábil** propõe uma aplicação web responsiva que funcione como um canal centralizado de relacionamento entre o escritório contábil e seus clientes, permitindo disponibilizar, consultar, baixar, solicitar e encaminhar documentos de maneira simples e organizada.

O objetivo do MVP é reduzir tarefas operacionais repetitivas, melhorar a comunicação e facilitar o acesso às informações, sem substituir os sistemas contábeis já utilizados pelos escritórios.

# 02. PERSON – Personas

As personas a seguir foram geradas com auxílio de IA e representam hipóteses de usuários potenciais do sistema. Não correspondem a entrevistas reais.

## Persona 01 – Primária: Carlos Henrique

- **Idade:** 42 anos.
- **Profissão:** Contador e proprietário de escritório.
- **Cidade:** Lages/SC.
- **Experiência:** 15 anos na área contábil.
- **Familiaridade com tecnologia:** Intermediária.

**Dor principal:** Perde muito tempo atendendo solicitações repetitivas de clientes, reenviando documentos e procurando arquivos em conversas de WhatsApp e e-mails.

**Cenário de uso:** Durante o expediente, Carlos precisa disponibilizar documentos aos clientes, solicitar arquivos necessários para o fechamento contábil e consultar quais empresas ainda possuem pendências documentais.

**Métrica de sucesso:** Reduzir em pelo menos 30% o tempo gasto com solicitações e disponibilização de documentos.

## Persona 02 – Secundária: Mariana Oliveira

- **Idade:** 35 anos.
- **Profissão:** Proprietária de comércio varejista.
- **Cidade:** Lages/SC.
- **Familiaridade com tecnologia:** Básica a intermediária.

**Dor principal:** Não sabe onde encontrar documentos disponibilizados pelo contador e frequentemente precisa solicitá-los novamente.

**Cenário de uso:** Durante sua rotina empresarial, precisa acessar documentos como contratos, guias, comprovantes, certidões e outros arquivos disponibilizados pelo escritório contábil.

**Métrica de sucesso:** Encontrar e baixar um documento necessário em menos de dois minutos, sem precisar entrar em contato com o escritório.

## Persona 03 – Secundária: Roberto Almeida

- **Idade:** 29 anos.
- **Profissão:** Auxiliar administrativo de empresa cliente.
- **Cidade:** Correia Pinto/SC.
- **Familiaridade com tecnologia:** Avançada.

**Dor principal:** Precisa organizar e encaminhar documentos mensalmente ao escritório contábil, mas não possui um canal padronizado para acompanhar o que já foi enviado e o que ainda está pendente.

**Cenário de uso:** Acessa o aplicativo pelo computador ou celular, verifica solicitações do escritório, envia os arquivos necessários e acompanha o andamento das pendências.

**Métrica de sucesso:** Conseguir acompanhar todas as solicitações documentais da empresa em um único ambiente.

# 03. ENTREVISTA SIMULADA – Descoberta de necessidades

**Objetivo:** Simular, com auxílio de IA, uma entrevista com um profissional de contabilidade para identificar possíveis dificuldades na comunicação e no compartilhamento de documentos com clientes.

**Entrevistado simulado:** Carlos Henrique – Contador, 42 anos.

**Observação:** Esta entrevista foi inteiramente simulada por IA, conforme a proposta da atividade. As respostas são hipóteses para orientar a descoberta de requisitos, não dados coletados de um usuário real.

### Pergunta 01 – Como acontece atualmente a comunicação com seus clientes quando precisam de documentos?

**Resposta simulada:**  
A maior parte acontece pelo WhatsApp. Alguns clientes utilizam e-mail, mas normalmente preferem mandar mensagens. Quando precisam de algum documento, entram em contato diretamente com o escritório.

### Pergunta 02 – Quais são as maiores dificuldades nesse processo?

**Resposta simulada:**  
O maior problema é a repetição. Muitos clientes solicitam documentos que já foram enviados anteriormente. Precisamos procurar nas conversas ou nos arquivos para encaminhar novamente. Isso acaba tomando bastante tempo da equipe.

### Pergunta 03 – Como você organiza os documentos que disponibiliza aos clientes?

**Resposta simulada:**  
Temos pastas no computador e documentos armazenados nos sistemas que utilizamos. Entretanto, não existe um local único onde o cliente possa acessar tudo sozinho.

### Pergunta 04 – Se existisse um aplicativo para centralizar esses documentos, o que seria mais importante?

**Resposta simulada:**  
Seria importante que cada cliente tivesse seu próprio acesso, pudesse consultar os documentos disponíveis, baixar arquivos e também visualizar quando o escritório estivesse solicitando alguma documentação.

### Pergunta 05 – Qual seria o principal benefício que você esperaria dessa solução?

**Resposta simulada:**  
Reduzir o volume de mensagens e ligações sobre documentos, economizar tempo da equipe e deixar o relacionamento com os clientes mais organizado.

### Principais dores identificadas na simulação

1. Solicitações repetitivas de documentos.
2. Informações descentralizadas em diferentes canais.
3. Dificuldade para localizar arquivos anteriormente enviados.
4. Falta de acompanhamento das pendências documentais.
5. Tempo excessivo gasto em atividades operacionais.

# 04. RF – Requisitos Funcionais

Os requisitos funcionais representam as ações e funcionalidades que o sistema deverá executar.

| ID | Requisito funcional |
|---|---|
| RF01 | O sistema deverá permitir o cadastro, edição, consulta e exclusão de empresas clientes, contendo razão social, nome fantasia e CNPJ. |
| RF02 | O sistema deverá permitir o cadastro, edição, consulta e exclusão de categorias para organização dos documentos. |
| RF03 | O sistema deverá permitir que o escritório disponibilize documentos digitais vinculados a uma empresa cliente e a uma categoria. |
| RF04 | O sistema deverá permitir que o cliente consulte e faça download dos documentos disponibilizados pelo escritório. |
| RF05 | O sistema deverá permitir que o escritório registre solicitações de documentos vinculadas a uma empresa cliente, informando descrição e prazo de entrega. |
| RF06 | O sistema deverá permitir que o cliente envie documentos digitais em resposta às solicitações realizadas pelo escritório. |
| RF07 | O sistema deverá permitir a consulta e o acompanhamento do status das solicitações documentais, identificando pendências e documentos enviados. |
| RF08 | O sistema deverá permitir autenticação de usuários e controle de acesso conforme seus respectivos perfis, diferenciando escritório e cliente. |

# 05. RNF – Requisitos Não Funcionais

Os requisitos não funcionais definem critérios de qualidade, segurança, desempenho e usabilidade da aplicação.

| ID | Requisito não funcional |
|---|---|
| RNF01 | A interface deverá ser responsiva, permitindo utilização em computadores, tablets e smartphones, com largura mínima de 320 pixels. |
| RNF02 | As principais páginas e consultas deverão apresentar carregamento em até 3 segundos em condições normais de conexão. |
| RNF03 | O sistema deverá implementar autenticação e controle de acesso, garantindo que cada cliente visualize exclusivamente os documentos e solicitações vinculados à sua empresa. |
| RNF04 | Os dados pessoais e documentos deverão ser protegidos, observando os princípios e requisitos aplicáveis da Lei Geral de Proteção de Dados (LGPD). |
| RNF05 | Os documentos e informações cadastrados deverão possuir persistência em banco de dados, mantendo os registros disponíveis após encerramento e reinicialização da aplicação. |

# 06. US – Histórias de Usuário

As histórias de usuário descrevem as funcionalidades sob a perspectiva de quem utilizará o sistema.

## US01 – Cadastro de empresas clientes

**Prioridade:** MUST HAVE  
**Estimativa:** 3 pontos.

**Como** administrador do escritório contábil,  
**quero** cadastrar e gerenciar empresas clientes,  
**para** organizar os documentos e solicitações de maneira individualizada para cada empresa.

**Critérios de aceitação:**

- [ ] AC01: O sistema deverá exigir razão social e CNPJ para cadastrar uma empresa.
- [ ] AC02: O sistema deverá validar o formato do CNPJ informado.
- [ ] AC03: O sistema deverá impedir o cadastro de duas empresas com o mesmo CNPJ no mesmo escritório.
- [ ] AC04: Após o cadastro, a empresa deverá aparecer na listagem de clientes.
- [ ] AC05: O administrador deverá conseguir editar e excluir os dados de empresas cadastradas.

## US02 – Disponibilização e consulta de documentos

**Prioridade:** MUST HAVE  
**Estimativa:** 5 pontos.

**Como** profissional do escritório contábil,  
**quero** disponibilizar documentos digitais vinculados a uma empresa cliente,  
**para** permitir que o cliente consulte e baixe seus documentos sempre que necessário.

**Critérios de aceitação:**

- [ ] AC01: O sistema deverá permitir selecionar a empresa cliente e a categoria do documento antes de realizar o envio.
- [ ] AC02: O sistema deverá permitir anexar arquivos em formatos PDF, JPG e PNG.
- [ ] AC03: Após o envio, o documento deverá aparecer na área de documentos da empresa correspondente.
- [ ] AC04: O cliente deverá conseguir visualizar e baixar os documentos disponibilizados para sua empresa.
- [ ] AC05: O sistema deverá impedir que um cliente visualize documentos pertencentes a outra empresa.

## US03 – Solicitação e envio de documentos

**Prioridade:** MUST HAVE  
**Estimativa:** 5 pontos.

**Como** profissional do escritório contábil,  
**quero** solicitar documentos aos clientes e acompanhar o recebimento dos arquivos,  
**para** organizar as pendências documentais e facilitar as atividades contábeis.

**Critérios de aceitação:**

- [ ] AC01: O escritório deverá conseguir criar uma solicitação vinculada a uma empresa cliente, contendo descrição e prazo de entrega.
- [ ] AC02: O cliente deverá conseguir visualizar as solicitações pendentes em sua área de acesso.
- [ ] AC03: O cliente deverá conseguir anexar um documento para responder à solicitação.
- [ ] AC04: Após o envio do arquivo, o status da solicitação deverá ser atualizado para "Documento enviado".
- [ ] AC05: O escritório deverá conseguir consultar os documentos recebidos e acompanhar o status das solicitações.

# 07. PRIORIZAÇÃO – MoSCoW

A metodologia MoSCoW foi utilizada para definir as funcionalidades prioritárias do MVP.

| Prioridade | Funcionalidades |
|---|---|
| **MUST HAVE** | Cadastro de empresas, autenticação, disponibilização de documentos, consulta e download, solicitação e envio de documentos. |
| **SHOULD HAVE** | Organização avançada por categorias, filtros por período e notificações de novas solicitações. |
| **COULD HAVE** | Dashboard com indicadores de pendências, histórico de movimentações e personalização visual por escritório. |
| **WON'T HAVE** | Integração automática com sistemas contábeis, emissão de notas fiscais, cálculo de impostos e geração automática de obrigações acessórias. |

# 08. OUT – Fora do escopo do MVP

Para manter o desenvolvimento inicial simples e viável, algumas funcionalidades não serão contempladas nesta primeira versão:

1. Substituição dos sistemas contábeis utilizados pelos escritórios.
2. Cálculo automático de tributos e geração de guias de impostos.
3. Emissão de notas fiscais.
4. Integração automática com plataformas governamentais, como e-CAC e Receita Federal.
5. Integração automática com WhatsApp ou outros aplicativos de mensagens.
6. Assinatura digital de documentos.
7. Aplicativo nativo para Android ou iOS.
8. Inteligência artificial para interpretação, classificação ou análise automática de documentos.

# 09. VALIDAÇÃO HUMANA E CONSIDERAÇÕES FINAIS

O documento foi elaborado com auxílio de inteligência artificial, seguindo as etapas de descoberta e documentação de requisitos apresentadas na aula.

As personas e a entrevista simulada foram geradas por IA e representam hipóteses de usuários e necessidades que poderão ser investigadas em uma etapa posterior.

Os requisitos foram organizados considerando a problemática proposta, buscando manter clareza, coerência e critérios verificáveis. Também foram considerados aspectos de segurança, controle de acesso e proteção de dados, importantes para uma aplicação que manipula documentos empresariais.

O **Conecta Contábil** pretende oferecer uma solução simples e acessível para centralizar o relacionamento documental entre escritórios contábeis e empresas clientes, reduzindo atividades repetitivas e melhorando a organização das informações.

**Objetivo principal do MVP:** demonstrar que um canal digital centralizado pode simplificar a disponibilização, consulta e solicitação de documentos, proporcionando economia de tempo para o escritório e maior autonomia para seus clientes.

---

## 🚀 Protótipo Online

Acesse o protótipo navegável do Conecta Contábil desenvolvido no Lovable:

👉 [Clique aqui para acessar o Conecta Contábil](https://conecta-contabil-compass.lovable.app/)


**Projeto acadêmico – Prototipação Rápida de Aplicações com IA**
