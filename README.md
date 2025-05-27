# ConexaoSaude

# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 

Link do Padlet:
https://padlet.com/neto0309/requisitos-de-software-glri12evthgxkqlf

## 1. Introdução
  
  ***1.1.  Grupo 6***

helder659
rafinhagvianna
FernandesHigor
GustavGomes36

  ***1.2.  Nome do Sistema***

Conexão Saúde

  ***1.3.  Propósito do Sistema***

  Objetivo: O objetivo do software é ajudar grupos vulneráveis da sociedade, informando e localizando postos de saúde, hospitais e outras instituições de saúde pública que possam suprir suas necessidades específicas. Além disso, busca priorizar, de modo eficiente, a redução do processo consultivo e auxiliar no transporte desses grupos vulneráveis até as instituições.

  ***1.2.  Público Alvo***

  Público-alvo: Pais com filhos pequenos e necessidades médicas, idosos, pessoas com doenças degenerativas, gestantes, entre outros.

  ***1.3. Descrição dos usuários***

  Pais com filhos pequenos e necessidades médicas: Geralmente buscam produtos e serviços que ofereçam segurança, conforto e praticidade. Estão preocupados com saúde, alimentação, bem-estar e desenvolvimento infantil.

  Idosos: Podem ter demandas voltadas à acessibilidade, conforto, saúde, entretenimento e qualidade de vida. Muitos valorizam a autonomia, mas também podem precisar de suporte para mobilidade e assistência médica.

  Pessoas com doenças degenerativas: Necessitam de acompanhamento contínuo e soluções que melhorem sua qualidade de vida. Terapias alternativas, equipamentos médicos e assistência personalizada são essenciais para o dia a dia.

  Gestantes: Buscam informação, produtos e serviços que garantam uma gravidez tranquila e saudável. Itens como roupas adaptadas, alimentação balanceada, suporte emocional e médico são prioritários.

  ***Personas:***

![image](https://github.com/user-attachments/assets/087783fe-9b34-4af6-9c62-84232df6bd01)
![image](https://github.com/user-attachments/assets/84a7c439-c949-42d3-b940-e17e96b2fa3e)
link para o acesso completo ao mapa da persona: 

https://www.canva.com/design/DAGm_WIvfpI/dtyuo0LkB_7ElQNZDLkcvA/edit?ui=eyJBIjp7fX0

  ***Análise da situação atual: antes da introdução de sua solução***

*`1. O que as pessoas fazem?`*

  Pessoas em situação de vulnerabilidade normalmente buscam atendimento de saúde de forma manual, ligando para unidades ou indo presencialmente até postos e hospitais, muitas vezes sem saber se há atendimento disponível, resultando em longas filas, deslocamentos desnecessários e falta de informação adequada.

*`2. Quais os artefatos envolvidos?`*

  Celulares para ligações, documentos físicos, transporte público ou privado, informações orais obtidas em comunidades, anotações em papel, além de recursos informais como redes sociais ou recomendações de conhecidos.

*`3. O que elas precisam saber?`*

  Precisam saber onde há atendimento próximo, se há especialidades compatíveis com suas necessidades, se o local está funcionando, qual o tempo de espera e como chegar até lá de forma acessível.

  ***Análise das tarefas depois: como serão executadas as suas tarefas com sua solução:***

*`1. O que as pessoas fazem?`*
   
   Utilizam o aplicativo Conexão Saúde para localizar rapidamente unidades próximas, filtrar por especialidades, verificar disponibilidade e agendar atendimentos prioritários, além de consultar rotas e solicitar transporte quando necessário.

*`2. Quais os artefatos envolvidos?`*

  Smartphone com o aplicativo Conexão Saúde, conexão com a internet, sistema de geolocalização, integração com bases como o CNES, aplicativos de transporte e notificações em tempo real.

*`3. O que elas precisam saber?`*

  Precisam apenas saber utilizar o aplicativo, pois a ferramenta irá fornecer informações completas e acessíveis sobre as unidades de saúde, tempos de espera, especialidades, localização e meios de transporte disponíveis.

  ***Cenário: Antes***

  Joana, mãe de uma criança asmática, precisa levá-la ao médico com urgência. Sem saber onde encontrar um pediatra disponível, ela tenta ligar para várias unidades de saúde, sem sucesso. Decide ir até o hospital da cidade, onde enfrenta uma fila de espera de horas, apenas para ser informada de que não há pediatras de plantão. Sem informações, ela volta para casa frustrada e preocupada com a saúde do filho.


  ***Cenário: Depois***

  Joana, ao perceber que seu filho apresenta sintomas, abre o aplicativo Conexão Saúde. Em segundos, ela localiza uma unidade próxima com atendimento pediátrico disponível, visualiza o tempo estimado de espera e solicita um carro de transporte parceiro pelo próprio app. Chega ao local em segurança e com prioridade de atendimento, garantindo o cuidado necessário com agilidade.


## 2. Documentos gerais no repositório

  ***2.1. Requisitos Funcionais***

| Identificador | Descrição    | Prioridade  | Depende de                  |
|:------:|:----------------------------------------------------:|:------------:|:------------------------:|
| RF01   | O software deve notificar um alerta para os usuários médicos em caso de superlotação em postos de atendimentos da região (ter uma demanda muito grande para a quantidade de médicos do posto,o próprio médico do posto pode requisitar ajudar o app, para os médicos mais próximos da região), a notificação deve chegar pelo próprio aplicativo. | M | RF02, RF09, RF11, RNF02, RF09 |
| RF02   |  O software deve permitir que os usuários realizem uma consulta rápida para verificar se possuem prioridade no atendimento com base em critérios pré-definidos, como idade, estado de saúde e urgência. Caso consiga prioridade, o usuário apareça a frente dos outros usuários, não prioritários, na fila | M | RNF03, RF06, RF07, RF09 |
| RF03   | O software deve localizar o usuário para saber sua trajetória a um melhor destino (mais próximo), isso deve ocorrer após o usuário permitir a que o app acesse a sua localização | M | RNF02, RF07, RF09 |
| RF04   | O software deve todo mês mostrar ao usuário uma campanha e nessas campanhas enviar tasks para o usuário, campanhas como "mês da dengue", tasks como "Confira se há água parada na sua residencia","Já armou sua telinha para não deixar a dengue entrar?" | C |  |
| RF05   | O software deve priorizar certos pacientes, dependendo da sua situação de risco/saude ou seja hierarquia na fila | S | RNF03, RF06, RF11 |
| RF06   | O usuário pode escolher uma opção de "transporte ajuda" e informar se está sozinho ou não, se consegue chegar ao posto mais acessível ou não, para assim o software requisitar ajuda de transporte para o usuário | C | RNF02, RF08, RF07 |
| RF07   | Após o atendimento e a confirmação da consulta no app, o usuário poderá avaliar o atendimento (nota + comentário). E o software deve adicionar esse comentário aos comentários do posto e do médico que usuário refere-se | C | RNF05, RNF06, RF12 |
| RF08   | O usuário pode ter a opção de dicas onde o software através de perguntas, sobre a situção de saúde atual do usuário, consiga ajudar o usuário com dicas de vitaminas, recomendações alimentáres, cuidados e caso o usuário estaja em situação de risco o software deve solicitar que ele procure um médico | C | RNF03, RF10, RF09 |
| RF09   | O Sistema deve possibilitar a busca de informações sobre postos de saúde,hospitais entre outras intituições de saúde publica: exibição de uma caixa de texto que servira de entrada do usuario para o sistema; exibe resultados com base em entradas parciais do usuario, em caixas em fileira; exibe informações simplificadas da instituição nas caixas infileiradas, todas essas informções devem estar armazenadas em um banco de dados | S | RF11, RF07, RNF02 |
| RF10   | O usuário deve informar/selecionar qual tipo de atendimento procura (Pediatrico; Pronto-Atendimento; Hospital geral;) | C | RF06, RF07, RF09, RF12 |
| RF11 | O Sistema deve enviar uma notificação de onde o usuário esta na fila e exibir um aviso quando o usuário for o proximo | S | RNF16 |

  ***2.2. Requisitos Não Funcionais***

| Identificador | Descrição    | Prioridade  | Depende de                  |
|:------:|:----------------------------------------------------:|:------------:|:------------------------:|
| RNF01   | O software deve garantir a segurança dos dados do usuário e médico com criptografia | M | |
| RNF02   | O software deve permitir acesso á localização do usuário apenas com consentimento explícito, o usuário a abrir o app deve escolher a opção "sim aceito saber minha localização" | M | RF03, RF06, RF09 |
| RNF03   | O software deve validar dados de saúde do usuário, com um questionário que deve aparecer ao usuário escolher a opção "ajuda/dicas", garantindo recomendações seguras | C | RF02, RF05, RF08, RF9 |
| RNF04   | O software deve oferecer interface intuitiva e acessível para os usuários | S | RF07, RF09, RF10 |
| RNF05   | O software deve garantir que os comentários e avaliações dos usuários sejam armazenados no banco de dados corretamente e protegidos (criptografia)| S | RF07 |
| RNF06   | O software deve permitir que médicos visualizem feedback dos usuários sobre o atendimento, esses feedbacks devem aparecer em local de comentáros no seu perfil. | C | RF07, RF09 |
| RNF07 | O Sistema deve cachear consultas frequentes utilizando Redis para reduzir o tempo de acesso ao banco de dados | S |
| RNF08 | O Sistema deve utilizar o banco de dados para armazenar informações | M |
| RNF09 | O Tamanho total do sistema não deve ser maior que 100 mBytes | S |
| RNF10 | O Sistema deve suportar inicialmente pelo menos 500.000 usuarios concorrentemente | M |
| RNF11 | O Sistema deve estar disponivel 90% das vezes | M |
| RNF12 | O Sistema deve utilizar um Framework para criar a Interface Gráfica do sistema (Abstract Window Toolkit)  | C |  |
| RNF13 | O Sistema deve utilizar uma linguagem orientada a objetos para a base do código do sistema (Java) | S |

  ***2.3. Perguntas***

## 📋 Pesquisa com Usuários: Melhorando o Atendimento em Postos de Saúde

Estamos desenvolvendo um aplicativo para facilitar o acesso aos serviços de saúde pública e gostaríamos de ouvir você! Suas respostas nos ajudarão a criar uma solução mais eficaz, acessível e centrada nas suas necessidades.

---

### 🏥 Experiência Atual com o Sistema de Saúde

- Você já enfrentou dificuldades em esperar por atendimento nos postos de saúde ou hospitais públicos?
- Quais são os principais desafios que você encontra ao buscar atendimento médico em postos de saúde ou hospitais públicos? *(Ex: longas filas, dificuldade para encontrar o posto certo, etc.)*
- Como você costuma saber qual é a sua posição na fila de atendimento nos postos de saúde?

---

### 📱 Uso de Aplicativos para Saúde

- O que você acha da ideia de usar um aplicativo para verificar se há filas nos postos de saúde e saber sua posição na fila?
- Qual é a sua principal expectativa ao utilizar um app para buscar atendimento médico?
- Você acha que seria útil receber notificações sobre sua posição na fila ou sobre a superlotação do posto? Como isso ajudaria no seu planejamento?

---

### 🧭 Funcionalidades e Usabilidade

- Se você fosse usar um aplicativo para encontrar postos de saúde, o que acha que deveria ser o mais fácil de acessar e visualizar?
- Você se sente confortável em usar aplicativos no seu smartphone? Qual é a sua experiência com esse tipo de tecnologia?
- O que você considera importante em um aplicativo para garantir que você consiga usá-lo facilmente?
- Se você fosse usar esse aplicativo, você gostaria que ele tivesse botões grandes e um design mais simples? Que tipo de ajustes você faria para que o app fosse mais fácil de usar?

---

### ♿ Acessibilidade

- Você tem dificuldades para ler ou entender textos pequenos ou complexos? Que tipo de recursos de acessibilidade seriam importantes para você? *(Ex: modo alto contraste, aumento de fonte, leitura em voz alta, etc.)*
- Quais dificuldades enfrenta para marcar, lembrar ou comparecer ás consultas e exames?
- O que um aplicativo de saúde poderia fazer para ajudar no seu acompanhamento médico?
- O que você acha desse app poder ajudar/acionar um transporte para que possa chegar até o posto?

---

### 🔔 Informações em Tempo Real

- Você acha que seria útil saber em tempo real se o posto de saúde está com superlotação? Como você gostaria de receber esse tipo de alerta?
- Quando você for ao posto de saúde, você gostaria de poder ver informações sobre os médicos, como especialidade ou avaliações de outros pacientes? Isso ajudaria a decidir em qual posto ir?
- Você gostaria de receber notificações sobre sua posição na fila e quando sera o proxim? isso é útil para seu planejamento?

---

### 📍 Localização e Transporte

- Você estaria disposto a permitir que o app acesse sua localização para te ajudar a encontrar o posto de saúde mais próximo ou mais acessível? O que te faria confiar nesse recurso?
- O que você pensa sobre a ideia de pedir ajuda para transporte, caso você não consiga se deslocar até o posto de saúde sozinho?

---

### 🔐 Privacidade e Segurança

- Você se sentiria confortável em fornecer informações de saúde (como condições médicas ou alergias) no app? O que você acha que seria importante para garantir que essas informações fiquem seguras?
- Quais são suas preocupações em relação ao uso de seus dados pessoais e médicos dentro de um aplicativo como esse?

---

### ⭐ Avaliações e Feedback

- Você gostaria de poder avaliar o atendimento médico depois de ser atendido no posto de saúde? O que você gostaria de poder comentar ou avaliar sobre o atendimento?
- O que você acha da ideia de ver comentários de outros usuários sobre um posto ou médico? Isso ajudaria na sua escolha?
- Se o sistema pedisse para você dar uma nota e um comentário após o atendimento, como você se sentiria em relação a essa funcionalidade?

---

### 👵 Público Idoso

- O que considera mais importante em um aplicativo para facilitar o seu uso? *(Ex: fontes grandes, textos claros, botões fáceis de clicar, etc.)*
- O senhor costumar usar o celular para se informar ou marcar consultas de saúde?
- Quais dificuldades o senhor já teve ao tentar marcar/ir de ultima hora a uma consulta ou exame pelo SUS?

---

### 🧪 Experiência com Apps de Saúde

- Você já usou algum aplicativo de saúde antes? Como foi essa experiência? O que você gostou ou não gostou?
- O que te faria sentir mais seguro ao usar um aplicativo de saúde? *(Ex: suporte fácil, explicações claras sobre o que fazer)*
- Se o aplicativo fosse muito técnico ou complicado, você teria dificuldades para usá-lo? O que faria você desistir de usá-lo?

---

### 🩺 Impacto e Continuidade

- Você acha que esse tipo de app poderia reduzir o tempo de espera e facilitar o acesso aos serviços de saúde? O que mais você esperaria dele?
- Como você se sentiria se o app ajudasse também a priorizar casos mais graves na fila? Isso seria importante para você?
- Quais seriam os maiores motivos para você continuar usando esse app a longo prazo?
- Se você tivesse que sugerir melhorias ou mudanças no aplicativo, quais seriam?

---

### 📞 Suporte e Atendimento

- Você gostaria de ter um atendimento ao usuário disponível diretamente no app, caso você tivesse dificuldades ou dúvidas sobre como usá-lo?


  ***2.4. Entrevista***

[Entrevista(parte1).docx](https://github.com/user-attachments/files/20447297/Entrevista.parte1.docx)
[Entrevista(parte2).docx](https://github.com/user-attachments/files/20447299/Entrevista.parte2.docx)


  ***2.5. Histórias do Usuário***

# RF01 - Notificações de Superlotação

## Descrição
Permitir que médicos recebam notificações sobre superlotação em postos de saúde da sua região, para facilitar o apoio rápido e melhorar o atendimento aos pacientes.

## História de Usuário
> **Como** médico usuário do aplicativo  
> **Quero** receber notificações de superlotação em postos da minha região  
> **Para** me disponibilizar para ajudar rapidamente e melhorar o atendimento dos pacientes

## Critérios de Aceitação
- O sistema detecta automaticamente superlotação com base em critérios definidos (número de pacientes/médicos).
- Médicos podem solicitar ajuda manualmente pelo aplicativo.
- Notificações são enviadas via push para médicos próximos.
- Notificações devem conter:
  - Nome do posto
  - Urgência
  - Número estimado de pacientes
 
 ---

 # RF02 - Verificação de Prioridade no Atendimento

## Descrição
Permitir que usuários verifiquem rapidamente se possuem prioridade no atendimento, garantindo que sejam atendidos conforme sua necessidade médica ou condição de risco.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** verificar rapidamente se tenho prioridade no atendimento  
> **Para** ser atendido de acordo com minha necessidade médica ou condição de risco

## Critérios de Aceitação
- O usuário informa dados como idade, sintomas e condição atual.
- O sistema classifica automaticamente se há prioridade.
- Usuários prioritários são destacados e movidos para o início da fila.
- A decisão é exibida de forma clara para o usuário.

---

# RF03 - Acesso à Localização e Direcionamento ao Posto de Saúde

## Descrição
Permitir que o usuário permita o acesso à sua localização para ser guiado até o posto de saúde mais próximo e acessível.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** permitir o acesso à minha localização  
> **Para** ser guiado até o posto de saúde mais próximo e acessível

## Critérios de Aceitação
- O app solicita permissão de localização.
- O app identifica o posto de saúde mais próximo.
- A rota é traçada e exibida em tempo real.
- Caso haja mais de uma opção, o usuário pode escolher.

---

# RF04 - Campanhas Mensais com Tarefas de Saúde

## Descrição
Enviar campanhas mensais com tarefas de saúde para manter o usuário informado e contribuir com a prevenção de doenças.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** receber campanhas mensais com tarefas de saúde  
> **Para** me manter informado e contribuir com a prevenção de doenças

## Critérios de Aceitação
- O sistema exibe uma nova campanha por mês.
- A campanha inclui tarefas (ex: verificar água parada).
- O usuário pode marcar tarefas como concluídas.
- As campanhas são temáticas e educativas.

---

# RF05 - Prioridade na Fila para Pacientes em Situação de Risco

## Descrição
Garantir que pacientes em situação de risco sejam priorizados na fila de atendimento para um atendimento mais rápido e adequado.

## História de Usuário
> **Como** paciente com situação de risco  
> **Quero** ser priorizado na fila de atendimento  
> **Para** garantir um atendimento mais rápido e adequado à minha saúde

## Critérios de Aceitação
- O sistema recebe dados médicos do paciente.
- A fila é reordenada conforme critérios médicos.
- A prioridade é exibida ao paciente e ao médico.
- O sistema atualiza automaticamente a posição.

---

# RF06 - Solicitação de Transporte para Usuários com Dificuldades de Locomoção

## Descrição
Permitir que usuários com dificuldades de locomoção solicitem ajuda de transporte até o posto de saúde para garantir o atendimento.

## História de Usuário
> **Como** usuário com dificuldades de locomoção  
> **Quero** solicitar ajuda de transporte até o posto de saúde  
> **Para** garantir que conseguirei atendimento mesmo sem condições de me deslocar sozinho

## Critérios de Aceitação
- O usuário responde perguntas sobre sua situação.
- O app detecta a necessidade de transporte.
- Uma solicitação é enviada a parceiros ou voluntários.
- O usuário recebe confirmação e estimativa de tempo.

---

# RF07 - Avaliação do Atendimento Recebido

## Descrição
Permitir que usuários avaliem o atendimento recebido para ajudar outros pacientes e melhorar a qualidade dos serviços.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** avaliar o atendimento recebido  
> **Para** ajudar outros pacientes e melhorar a qualidade dos serviços

## Critérios de Aceitação
- O app exibe formulário de avaliação após a consulta.
- O usuário pode dar uma nota e escrever um comentário.
- As avaliações ficam visíveis no perfil do médico/posto.
- O usuário pode editar ou excluir a avaliação.

---

# RF08 - Dicas Personalizadas e Alertas de Saúde

## Descrição
Fornecer dicas personalizadas e alertas para que o usuário cuide melhor da saúde e saiba quando procurar um médico.

## História de Usuário
> **Como** usuário preocupado com minha saúde  
> **Quero** receber dicas personalizadas e alertas  
> **Para** cuidar melhor da minha saúde e saber quando procurar um médico

## Critérios de Aceitação
- O app faz perguntas rápidas sobre sintomas e hábitos.
- Gera recomendações de saúde e bem-estar.
- Alerta o usuário caso haja risco.
- Recomenda procurar atendimento, se necessário.

---

# RF09 - Busca de Informações sobre Instituições de Saúde

## Descrição
Permitir que usuários busquem informações sobre instituições de saúde para encontrar o local mais adequado e entender os serviços disponíveis.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** buscar informações sobre instituições de saúde  
> **Para** encontrar o local mais adequado e entender os serviços disponíveis

## Critérios de Aceitação
- Caixa de busca com autocompletar.
- Resultados exibidos em cards com dados básicos.
- Informações puxadas de banco de dados.
- Exibição clara e organizada.

---

# RF10 - Seleção do Tipo de Atendimento

## Descrição
Permitir que o usuário selecione o tipo de atendimento desejado para ser direcionado ao serviço correto e receber atendimento adequado.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** selecionar o tipo de atendimento que procuro  
> **Para** ser direcionado ao serviço correto e receber o atendimento adequado

## Critérios de Aceitação
- Opções de tipos de atendimento disponíveis na interface.
- O usuário deve selecionar antes de prosseguir.
- A seleção influencia a fila e localização.
- Validação da escolha antes do envio.

---

# RF11 - Notificações da Posição na Fila

## Descrição
Enviar notificações automáticas para que o usuário saiba exatamente quando será atendido e possa se preparar.

## História de Usuário
> **Como** usuário do aplicativo  
> **Quero** receber notificações da minha posição na fila  
> **Para** saber exatamente quando será meu atendimento e me preparar

## Critérios de Aceitação
- Notificações enviadas automaticamente conforme posição muda.
- Aviso claro quando o usuário estiver próximo.
- Histórico das notificações disponível.
- Notificações funcionam mesmo com o app em segundo plano.

  ***2.6. Diagramas de Caso de Uso e Especificações***

*<Imagem, arquivo (PDF), link com Diagrama de Caso de Uso.>*

  ***2.7. Diagramas de Atividades***

*<Imagem, arquivo (PDF), link com Diagrama de Atividades.>*

  ***2.8. Matrizes de Rastreabilidade***

*<Imagem, arquivo (PDF), link com Matriz de Rastreabilidade.>*

  ***2.9. Protótipos***

![image](https://github.com/user-attachments/assets/501395a2-6fc1-4ba1-a063-b269c9968157)

Link para o arquivo no NinjaMock do Protótipo: https://ninjamock.com/Designer/Workplace/204713961/Page1


*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*

[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
