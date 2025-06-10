# Requisitos

# ETAPA 1

### AUTORES

Aluno, Secretaria, Professores, Coordenadores, Diretorias

### LEVANTAMENTO DE REQUISITOS

GRUPO 01: ESSENCIAL 

RF01 - Consultar informações do aluno 

RF02 - Consultar notas

RF03 - Consultar faltas e percentual de frequência 

RF04 - Consultar horário das aulas 

RF05 - Consultar datas de avaliações 

RF16 - Consultar histórico acadêmico

RF07 - Realizar atrícula e trancar curso

RF08 - Realizar rematrícula

RF09 - Trancar curso

RF10 - Consultar mural de notícias 

GRUPO 02 - IMPORTANTE 

RF08 - Calendário acadêmico 

RF09 - Solicitação de exame

RF10 - Solicitação de proficiência

RF11 - Regime domciliar 

RF12 - Bibliografia 

RF13 - Materiais de aula

RF14 - Gerência de estágio

RF15 – Submeter processo de estágio obrigatório

RF16 - Solicitação de exame de aluno especial

RF17 – Enviar atestados médicos

GRUPO 3: NÃO FUNCIONAIS (especificar mais tarde) 

NRF01 - Login

NRF02 - Experiência do usuário

NRF03 - Interface

NRF04 - Acessibilidade

NRF05 - Desempenho

NRF06 - Usabilidade

NRF07 - Disponibilidade

NRF08 - Compatibilidade

NRF09 - Escalabilidade

NRF010 - Manutenibilidade

## Divisão de grupos para melhor clareza das ideias

### Grupo 1 – Acadêmico

- **Consultar informações do aluno**
- **✅Consultar notas**
- **✅ Consultar faltas e percentual de frequência**
- **Consultar horário das aulas**
- **Consultar datas de avaliações**
- **Consultar histórico acadêmico**
- **Consultar calendário acadêmico**

### Grupo 2 – Matrícula e Solicitações Especiais

- **Realizar matrícula**
- **Realizar rematrícula**
- **Solicitar trancamento de curso**
- **Solicitar exame de aluno especial**
- **Solicitar exame de proficiência**
- **Solicitar regime domiciliar**
- **Enviar atestados médicos**

### Grupo 4 – Comunicação (HOME)

- **✅Consultar mural de notícias e avisos**

### NARRATIVAS DE CASOS DE USO

CASO DE USO 1: 

**Nome:** Fazer login

**Atores:** Aluno

**Descrição:** Permite que o aluno acesse o aplicativo por meio da autenticação com usuário e senha.

**Pré-condições:** O aluno deve ter um cadastro ativo no sistema.

**Fluxo principal de eventos:**

1. O aluno acessa o aplicativo.
2. O sistema solicita matrícula e senha.
3. O aluno insere as credenciais.
4. O sistema verifica as informações.
5. O sistema libera o acesso ao sistema.
    
    **Fluxo alternativo:**
    
- 3a. Se os dados estiverem incorretos, o sistema exibe uma mensagem de erro.
- 3b. Após 3 tentativas incorretas, o acesso é temporariamente bloqueado.
    
    **Pós-condições:** O aluno acessa a tela inicial do sistema.
    

CASO DE USO 2:

**Nome:** Consultar notas

**Atores:** Aluno

**Descrição:** Permite que o aluno visualize as notas obtidas nas disciplinas cursadas.

**Pré-condições:** O aluno precisa estar logado no sistema.

**Fluxo principal de eventos:**

1. O aluno seleciona a opção “Notas” no menu.
2. O sistema exibe as disciplinas cursadas e as respectivas notas.
    
    **Fluxo alternativo:**
    
- 2a. Se o aluno não estiver matriculado em nenhuma disciplina, o sistema exibe uma mensagem informativa.
    
    **Pós-condições:** As notas são apresentadas ao aluno na interface.
    

CASO DE USO 3:

**Nome:** Enviar atestados

**Atores:** Aluno, Secretaria

**Descrição:** Permite que o aluno envie atestados médicos ou documentos para justificar ausências.

**Pré-condições:** O aluno deve estar logado e possuir o documento digitalizado.

**Fluxo principal de eventos:**

1. O aluno acessa a funcionalidade “Enviar Atestados”.
2. O aluno seleciona o arquivo e insere uma descrição.
3. O sistema envia o documento para análise da Secretaria.
4. A Secretaria recebe a solicitação.
    
    **Fluxo alternativo:**
    
- 2a. Se o arquivo estiver em formato inválido, o sistema exibe mensagem de erro.
    
    **Pós-condições:** O atestado fica pendente de validação pela Secretaria.
    

CASO DE USO 4: 

**Nome:** Consultar dados acadêmicos

**Atores:** Aluno

**Descrição:** Permite que o aluno acesse diversas informações relacionadas ao seu desempenho e à organização do curso.

**Pré-condições:** O aluno precisa estar logado no sistema.

**Fluxo principal de eventos:**

1. O aluno acessa o menu “Acadêmico”.
2. O sistema apresenta opções como:
    - Notas
    - Faltas e frequência
    - Horário das aulas
    - Data das avaliações
    - Histórico acadêmico
    - Grade curricular
3. O aluno seleciona a opção desejada.
4. O sistema exibe as informações correspondentes.
    
    **Fluxo alternativo:**
    
- 3a. Caso não haja dados disponíveis (ex: aluno sem matrícula ativa), o sistema exibe uma mensagem informativa.
    
    **Pós-condições:** As informações acadêmicas selecionadas são exibidas corretamente.
    

CASO DE USO 5: 

**Nome:** Realizar matrícula, rematrícula ou trancar curso

**Atores:** Aluno, Secretaria

**Descrição:** Permite ao aluno realizar matrícula, rematrícula e trancamento de curso diretamente pelo sistema.

**Pré-condições:** O período para a ação deve estar aberto e o aluno logado.

**Fluxo principal de eventos:**

1. O aluno acessa o menu “Matrícula”.
2. Escolhe entre:
    - Matrícula inicial
    - Rematrícula
    - Trancamento de curso
3. O aluno escolhe as disciplinas (caso aplicável) e envia a solicitação.
4. O sistema registra a solicitação e informa o status.
    
    **Fluxo alternativo:**
    
- 3a. Caso o período de matrícula esteja fechado, o sistema exibe uma mensagem de aviso.
    
    **Pós-condições:** A solicitação é salva e enviada à secretaria, com possibilidade de acompanhamento do status.
    

CASO DE USO 6: 

**Nome:** Enviar documentos e abrir solicitações especiais

**Atores:** Aluno, Secretaria

**Descrição:** Permite que o aluno envie documentos e solicite situações especiais como exames ou regime domiciliar.

**Pré-condições:** O aluno precisa estar logado e com os documentos digitalizados.

**Fluxo principal de eventos:**

1. O aluno acessa o menu “Solicitações”.
2. Escolhe o tipo de solicitação:
    - Atestado médico
    - Exame especial
    - Exame de proficiência
    - Regime domiciliar
3. O aluno preenche os dados e anexa o documento.
4. O sistema envia para a secretaria.
    
    **Fluxo alternativo:**
    
- 3a. Se o arquivo for inválido ou estiver corrompido, o sistema exibe mensagem de erro.
    
    **Pós-condições:** A solicitação é enviada para análise da secretaria.
