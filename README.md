# 1. Escopo do Projeto

O projeto consiste no desenvolvimento de um **sistema digital para gestão de infrações disciplinares** em instituições de ensino, com foco inicial no Instituto Federal do Piauí (IFPI). O sistema permitirá o registro, acompanhamento e conclusão de ocorrências disciplinares, garantindo transparência, comunicação eficiente com os responsáveis, rastreabilidade e total conformidade com a **Organização Didática do IFPI** (Resolução Normativa 143/2022 – CONSUP/IFPI). O sistema abrangerá desde a comunicação da infração até a aplicação de penalidades, incluindo notificações, ciência dos envolvidos e assinaturas digitais das autoridades competentes.

# 2. Problema

## 2.1 Instrução do Problema

| | |
|---|---|
| **o problema é** | A dificuldade das escolas em registrar e organizar as ocorrências de indisciplina dos alunos, além da demora ou falha em comunicar os responsáveis, agravada pela fragmentação dos processos e pela dependência exclusiva da coordenação. |
| **o que acontece** | As ocorrências são frequentemente registradas de forma manual (papel, planilhas), o que causa perda de informações, atrasos na comunicação, falta de rastreabilidade e dificuldade em identificar reincidências. A comunicação com os pais é lenta e muitas vezes inexistente, prejudicando o acompanhamento familiar e a aplicação de medidas corretivas adequadas. |
| **o impacto do problema é** | Falta de controle do comportamento dos alunos, pais desinformados, sobrecarga da coordenação, morosidade nas decisões e risco de não conformidade com as normas institucionais (Capítulo XVIII da Organização Didática). |
| **uma solução seria** | Criar um sistema digital para registrar ocorrências, organizar o histórico dos alunos, sugerir penalidades com base nas regras da Organização Didática, enviar notificações automáticas aos responsáveis e garantir a ciência formal e as assinaturas necessárias, assegurando um processo transparente, rápido e auditável. |

## 2.2 Problemas a serem resolvidos

| Problema | Descrição |
|----------|-----------|
| **Demora para avisar os pais** | A comunicação com os responsáveis é lenta e, muitas vezes, não acontece, dificultando o acompanhamento e a aplicação de medidas corretivas. |
| **Perda de informações importantes** | Registros feitos em papel ou planilhas podem ser perdidos, danificados ou esquecidos, comprometendo o histórico disciplinar. |
| **Sobrecarga da coordenação** | A coordenação precisa buscar informações manualmente, analisar reincidências sem apoio automatizado e gastar tempo excessivo com tarefas burocráticas. |
| **Falta de rastreabilidade** | Não há um histórico claro e auditável das infrações, das penalidades aplicadas e das comunicações realizadas. |
| **Dificuldade em identificar reincidências** | Sem um sistema centralizado, é complexo verificar se um aluno já cometeu infrações anteriores, dificultando a aplicação de penalidades proporcionais. |
| **Risco de não conformidade legal** | O processo manual pode desrespeitar prazos, competências e formalidades exigidas pela Organização Didática (arts. 137 a 140). |

# 3. Descrição da Parte Interessada e do Usuário

- **Escola (Direção Geral e Direção de Ensino):** desejam supervisionar o processo disciplinar, assinar penalidades mais graves (suspensão e cancelamento) e garantir a conformidade com as normas.
- **Coordenador de Curso:** responsável por analisar as infrações, definir a penalidade adequada, registrar a fundamentação e acompanhar o fluxo até a conclusão.
- **Professores:** precisam registrar comportamentos inadequados de forma rápida e simples durante ou após as aulas.
- **Equipe Pedagógica:** pode auxiliar no registro e na análise de infrações, especialmente em casos que envolvem aspectos educacionais.
- **Aluno:** envolvido na infração; deve dar ciência formal da penalidade e cumprir as medidas aplicadas.
- **Pais e Responsáveis:** recebem notificações sobre as infrações, acompanham o comportamento do aluno e precisam registrar ciência formal.

# 4. Visão Geral do Produto

## 4.1 Perspectiva do Produto

O sistema será uma aplicação web responsiva (compatível com dispositivos móveis e desktop) que centraliza o gerenciamento disciplinar. Ele servirá como ponte entre professores, coordenação e responsáveis, permitindo comunicação rápida e segura. Poderá ser integrado futuramente ao sistema acadêmico existente do IFPI, aproveitando dados de matrícula e contatos.

## 4.2 Resumo dos Recursos

- Registro de ocorrências em tempo real, com campos padronizados (baseados no art. 139 da Organização Didática).
- Histórico disciplinar completo por aluno.
- Notificações automáticas para responsáveis (e-mail, SMS ou push).
- Sugestão de penalidades com base em regras e reincidências.
- Registro de ciência digital do aluno e dos responsáveis.
- Fluxo de assinaturas digitais para autoridades (coordenador, direção de ensino, direção geral), conforme a gravidade da penalidade.
- Painel de acompanhamento com filtros e relatórios gerenciais.
- Classificação automática de reincidências.

# 5. Recursos do Produto (Funcionalidades)

- **Registro de ocorrências:** permitir que professores, coordenadores e equipe pedagógica registrem infrações com dados como aluno, descrição, tipo de indisciplina (menu baseado no art. 139), data, horário, local e evidências (fotos, arquivos).
- **Notificações automáticas:** enviar alertas aos responsáveis e à coordenação imediatamente após o registro.
- **Análise e definição de penalidade:** exibir ao coordenador as penalidades possíveis (art. 138), identificar reincidências automaticamente e sugerir a penalidade adequada com base nas regras.
- **Ciência eletrônica:** permitir que o aluno (via login) e os responsáveis (via link seguro) registrem ciência formal, com data/hora e IP.
- **Assinaturas digitais:** possibilitar que as autoridades assinem digitalmente a infração, com configuração por tipo de penalidade (ex.: advertência oral só coordenador; suspensão exige direção de ensino; cancelamento exige direção geral).
- **Conclusão e arquivamento:** alterar o status para "Concluída" automaticamente após cumprimento de todas as etapas, mantendo o histórico acessível.
- **Relatórios:** gerar relatórios individuais e estatísticos para reuniões pedagógicas e auditorias.
- **Área do responsável:** portal com login para visualizar ocorrências e dar ciência.
- **Identificação de reincidência:** alerta automático quando o aluno já possui infrações anteriores.

# 6. Caso de Uso

## 6.1 Diagrama de Casos de Uso

![Diagrama de Casos de Uso](https://github.com/user-attachments/assets/36658c47-7da7-4bd9-ba59-1abc404f8572)



## 6.2 Fluxos dos Casos de Uso

### Registrar Ocorrência
- **Atores:** Professor, Coordenador, Equipe Pedagógica  
- **Descrição:** Registrar uma ocorrência disciplinar no sistema, incluindo todos os dados exigidos.
- **Fluxo:**
  1. O usuário acessa o sistema e autentica-se.
  2. Seleciona a opção "Registrar Ocorrência".
  3. Busca e seleciona o(s) aluno(s) envolvido(s).
  4. Preenche os dados: tipo de infração (baseado no art. 139), descrição detalhada, data, horário, local e, opcionalmente, anexa evidências.
  5. O sistema valida os campos obrigatórios e salva a ocorrência.
  6. O sistema dispara notificações automáticas para os responsáveis e para a coordenação.
  7. A ocorrência fica com status "Aguardando Análise".

### Analisar Infração e Aplicar Penalidade
- **Atores:** Coordenador de Curso  
- **Descrição:** Analisar a infração registrada, verificar reincidências e definir a penalidade adequada.
- **Fluxo:**
  1. O coordenador acessa a lista de ocorrências pendentes.
  2. Seleciona uma ocorrência específica.
  3. O sistema exibe o histórico de infrações do aluno e destaca reincidências.
  4. O sistema sugere penalidades possíveis conforme a gravidade e as regras (art. 138 e 139).
  5. O coordenador escolhe a penalidade, registra a fundamentação e o prazo para ciência.
  6. O sistema atualiza o status para "Aguardando Ciência".

### Registrar Ciência
- **Atores:** Aluno, Responsável  
- **Descrição:** O aluno e/ou responsável registram ciência formal da infração e da penalidade.
- **Fluxo:**
  1. O sistema envia notificação ao aluno (via e-mail ou portal) e ao responsável (via link seguro).
  2. O aluno acessa o sistema com seu login e visualiza a ocorrência; clica em "Registrar Ciência".
  3. O responsável acessa o link, confirma sua identidade (ex.: token enviado por e-mail) e registra ciência.
  4. O sistema registra data/hora e IP da ciência.
  5. Status alterado para "Aguardando Assinaturas".

### Assinar Penalidade
- **Atores:** Coordenador, Direção de Ensino, Direção Geral (conforme a penalidade)  
- **Descrição:** Autoridades competentes assinam digitalmente a infração, conforme definido no art. 138.
- **Fluxo:**
  1. O sistema notifica as autoridades necessárias (baseado na penalidade aplicada).
  2. Cada autoridade acessa a ocorrência e clica em "Assinar Digitalmente".
  3. O sistema valida a assinatura e registra o ato.
  4. Após todas as assinaturas obrigatórias, o status muda para "Concluída".

### Consultar Histórico
- **Atores:** Aluno, Responsável, Coordenador, Direção  
- **Descrição:** Consultar o histórico de ocorrências de um aluno específico.
- **Fluxo:**
  1. O usuário acessa a funcionalidade de consulta.
  2. Busca pelo nome ou matrícula do aluno.
  3. O sistema exibe a lista de infrações, com status, penalidades e datas.
  4. É possível filtrar por período, tipo de infração ou status.

### Notificar Responsável
- **Atores:** Sistema  
- **Descrição:** Enviar notificação ao responsável sempre que uma infração for registrada ou houver atualização relevante.
- **Fluxo:**
  1. Uma ocorrência é registrada ou tem seu status alterado.
  2. O sistema identifica os contatos do responsável (e-mail, telefone).
  3. O sistema envia a notificação com os detalhes da ocorrência e um link para acesso.
  4. O envio é registrado no log da ocorrência.

# 7. Restrições

## 7.1 Restrições de Design

- Interface simples e intuitiva, priorizando facilidade de uso por professores com diferentes níveis de familiaridade tecnológica.
- Cores neutras e layout acessível (contraste adequado, suporte a leitores de tela).
- Compatibilidade com dispositivos móveis e desktop (design responsivo).
- Navegação clara e com poucos cliques para as tarefas mais comuns.

## 7.2 Restrições de Segurança

- Dados dos alunos e responsáveis devem ser protegidos por criptografia (em repouso e em trânsito).
- Acesso ao sistema somente por usuários autenticados e autorizados, com perfis distintos (professor, coordenador, direção, responsável, aluno).
- Registro de logs de todas as ações (quem, quando, o quê) para auditoria.
- Conformidade com a Lei Geral de Proteção de Dados (LGPD).
- Utilização de assinatura digital com validade jurídica (certificado digital ou token seguro).

## 7.3 Restrições de Metodologia (Processos e Ferramentas)

- Desenvolvimento baseado em ciclo iterativo e incremental, com validação frequente com usuários reais.
- Utilização de banco de dados relacional seguro (ex.: PostgreSQL) para armazenamento das informações.
- Versionamento de código com Git e hospedagem em repositório privado.
- Documentação contínua das decisões de design e regras de negócio.
- Testes de usabilidade e segurança antes da implantação.
- Atualizações e manutenção programadas, com backup periódico dos dados.
•Atualizações e manutenção periódicas.

•Sistema deve ser desenvolvido com tecnologias que permitam escalabilidade.
