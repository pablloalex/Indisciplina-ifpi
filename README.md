# 1. Escopo do Projeto

Delimitar as características do projeto. Descrever do que se trata,deixando claro o contexto abordado.

# 2. Problema
Gerenciamento de indisciplinas de alunos e dificuldade de avisar os pais.
## 2.1 Instrução do Problema
|    |    |
|---|---|
|o problema é|A dificuldade das escolas em registrar e organizar as ocorrências de indisciplina dos alunos, além da demora ou falha em comunicar os responsáveis.|
|o que acontece|As ocorrências muitas vezes são registradas de forma manual , o que causa perda de informações, atrasos na comunicação e falta de acompanhamento adequado. Isso afeta professores, coordenação e principalmente os responsáveis que não recebem os avisos a tempo.|
|o impacto do problema é|Falta de controle do comportamento dos alunos, pais desinformados.|
|uma solução seria|Criar um sistema digital para registrar ocorrências, organizar o histórico dos alunos e enviar notificações automáticas aos responsáveis, garantindo comunicação rápida, eficiente e centralizada.|
## 2.2 Problemas a serem resolvidos
|Problema   |Descrição   |
|---|---|
|Demora para avisar os pais|A comunicação com os responsáveis é lenta e, muitas vezes, não acontece, dificultando o acompanhamento.|
|Perda de informações importantes|Registros feitos em papel podem ser perdidos, danificados ou esquecidos.|
|Sobrecarga da coordenação|A coordenação precisa buscar informações manualmente, gastando tempo e aumentando erros.|

# 3. Descrição da Parte Interessada e do Usuário
•Escola (Direção e Coordenação): deseja registrar e acompanhar as ocorrências de forma eficiente.

•Professores: precisam registrar comportamentos rapidamente durante ou após as aulas.

•Pais e Responsáveis: recebem notificações e acompanham o comportamento do aluno.
# 4. Visão Geral do Produto
## 4.1 Perspectiva do Produto
O sistema será uma aplicação escolar que centraliza o gerenciamento disciplinar. Ele servirá como ponte entre professores, coordenação e responsáveis, permitindo comunicação rápida e segura. Pode ser integrado ao sistema acadêmico existente da escola.
## 4.2 Resumo dos Recursos
•Registro de ocorrências em tempo real.

•Histórico por aluno.

•Notificações automáticas para responsáveis (app, SMS, e-mail).
# 5. Recursos do Produto(Funcionalidades)
•Geração de relatórios para reuniões pedagógicas.

•Notificações automáticas enviadas aos responsáveis.

•Painel para visualização do histórico disciplinar.

•Área do responsável com login para acompanhar o aluno.
# 6. Caso de Uso

## 6.1 Diagrama de Casos de Uso
![Image](https://github.com/user-attachments/assets/36658c47-7da7-4bd9-ba59-1abc404f8572)
## 6.2 Fluxos dos Casos de Uso

### Registrar Ocorrência
- **Atores:** Professor, Coordenador  
- **Descrição:** Registrar uma ocorrência disciplinar no sistema.
- **Fluxo:**
  1. O usuário acessa o sistema.
  2. Seleciona o aluno.
  3. Preenche os dados da ocorrência.
  4. O sistema salva a ocorrência.

---

### Consultar Histórico
- **Atores:** Aluno, Responsável, Coordenador  
- **Descrição:** Consultar o histórico de ocorrências do aluno.
- **Fluxo:**
  1. O usuário acessa o sistema.
  2. Busca o aluno.
  3. O sistema exibe o histórico.

---

### Notificar Responsável
- **Atores:** Sistema  
- **Descrição:** Enviar notificação ao responsável após registro da ocorrência.
- **Fluxo:**
  1. Uma ocorrência é registrada.
  2. O sistema identifica o responsável.
  3. O sistema envia a notificação.
  4. O envio é registrado pelo sistema.

# 7. Restrições
## 7.1 Restrições de Design
•Interface simples e intuitiva para facilitar uso por professores.

•Cores neutras e layout acessível.

•Compatibilidade com dispositivos móveis e desktop.
## 7.2 Restrições de Segurança
•Dados dos alunos devem ser protegidos por criptografia.

•Acesso ao sistema somente por usuários autorizados.

•Logs de atividade para auditoria.
## 7.3 Restrições de Metodologia (Processos e Ferramentas)
•Uso de banco de dados seguro para armazenamento de informações.

•Atualizações e manutenção periódicas.

•Sistema deve ser desenvolvido com tecnologias que permitam escalabilidade.
