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
link para o acesso completo ao mapa da persona: https://www.canva.com/design/DAGm_WIvfpI/dtyuo0LkB_7ElQNZDLkcvA/edit?ui=eyJBIjp7fX0

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
| RF01   | O software deve notificar um alerta para os usuários médicos em caso de superlotação em postos de atendimentos da região | Alta | RF02, RF09, RF11, RNF02, RF12 |
| RF02   |  O software deve permitir que os usuários realizem uma consulta rápida para verificar se possuem prioridade no atendimento com base em critérios pré-definidos, como idade, estado de saúde e urgência. | Alta | RNF03, RF06, RF07, RF12 |
| RF03   | O software deve localizar o usuário para saber sua trajetória a um melhor destino, isso deve ocorrer após o usuário permitir a que o app acesse a sua localização | Alta | RNF02, RF07, RF09 |
| RF04   | O software deve todo mês mostrar ao usuário um evento e nesses evento enviar tasks para o usuário | Alta | RF12 |
| RF05   | O software deve priorizar certos pacientes, dependendo da sua situação de risco/saude ou seja hierarquia na fila/ criar uma fila para casos graves | Alta | RNF03, RF06, RF11, RF12 |
| RF06   | O usuário deve informar se está sozinho ou não, se consegue chegar ao posto mais acessível ou não, para assim o software entender se requisitar ajuda de transporte para o usuário | Alta | RNF02, RF08, RF07, RF12 |
| RF07   | O usuário poderá avaliar o atendimento (nota + comentário). E o software deve conectar/alocar esse comentário a comentários do posto e do médico que usuário refere-se | Alta | RNF05, RNF06, RF12 |
| RF08   | O software deve filtrar quais tipos de medicamentos devem ser indicados para o usuário (devido a alguma alergia, ou restrição que ele informou ) | Alta | RNF03, RF10, RF12 |
| RF09   | O Sistema deve possibilitar a busca de informações sobre postos de saúde,hospitais entre outras intituições de saúde publica: exibição de uma caixa de texto que servira de entrada do usuario para o sistema; exibe resultados com base em entradas parciais do usuario, em caixas em fileira; exibe informações simplificadas da instituição nas caixas infileiradas | Alta | RF11, RF07, RNF02 |
| RF10   | O usuário deve informar/selecionar qual tipo de atendimento procura (Pediatrico; Pronto-Atendimento; Hospital geral;) | Alta | RF06, RF07, RF09, RF12 |
| RF11 | O Sistema deve enviar uma notificação de onde o usuário esta na fila e exibir um aviso quando o usuário for o proximo | Alta | RNF16 |
| RF12 | O Sistema deve possibilitar a busca de informações sobre postos de saúde,hospitais entre outras intituições de saúde publica e os usos de filtros de pesquisa | Alta | RNF16 |



  ***2.2. Requisitos Não Funcionais***

| Identificador | Descrição    | Prioridade  | Depende de                  |
|:------:|:----------------------------------------------------:|:------------:|:------------------------:|
| RNF01   | O software deve garantir a segurança dos dados do usuário e médico | Alta | RF12 |
| RNF02   | O software deve permitir acesso á localização do usuário apenas com consentimento explícito | Alta | RF03, RF06, RF09 |
| RNF03   | O software deve validar dados de saúde do usuário, garantindo recomendações seguras | Alta | RF02, RF05, RF08, RF12 |
| RNF04   | O software deve oferecer interface intuitiva e acessível para os usuários | Média | RF07, RF09, RF10 |
| RNF05   | O software deve garantir que os comentários e avaliações dos usuários sejam armazenados corretamente e protegidos| Alta | RF07 |
| RNF06   | O software deve permitir que médicos visualizem feedback dos usuários sobre o atendimento | Alta | RF07, RF12 |
| RNF07   | O usuário poderá avaliar o atendimento (nota + comentário). E o software deve conectar/alocar esse comentário a comentários do posto e do médico que usuário refere-se | Alta | RNF05, RNF06, RF12 |
| RNF08   | O software deve filtrar quais tipos de medicamentos devem ser indicados para o usuário (devido a alguma alergia, ou restrição que ele informou ) | Alta | RNF03, RF10, RF12 |
| RNF09   | O Sistema deve possibilitar a busca de informações sobre postos de saúde,hospitais entre outras intituições de saúde publica: exibição de uma caixa de texto que servira de entrada do usuario para o sistema; exibe resultados com base em entradas parciais do usuario, em caixas em fileira; exibe informações simplificadas da instituição nas caixas infileiradas | Alta | RF11, RF07, RNF02 |
| RNF10 | O Sistema deve cachear consultas frequentes utilizando Redis para reduzir o tempo de acesso ao banco de dados | Alta |
| RNF11 | O Sistema deve utilizar o banco de dados para armazenar informações | Alta |
| RNF12 | O Tamanho total do sistema não deve ser maior que 100 mBytes | Alta |
| RNF13 | O Sistema deve suportar inicialmente pelo menos 500.000 usuarios concorrentemente | Alta |
| RNF14 | O Sistema deve estar disponivel 90% das vezes | Alta |
| RNF15 | O Sistema deve utilizar um Framework para criar a Interface Gráfica do sistema  | Alta | RNF16 |
| RNF16 | O Sistema deve utilizar uma linguagem orientada a objetos para a base do código do sistema | Alta |

  ***2.3. Perguntas***

*<Arquivo com as perguntas realizadas na entrevista .>*

  ***2.4. Entrevista***

*<Arquivo com as respostas do indivíduo entrevistado e link do drive com upload da gravação.>*

  ***2.5. Histórias do Usuário***

*<Imagem, arquivo (PDF), link com as Histórias de Usuário.>*

  ***2.6. Diagramas de Caso de Uso e Especificações***

*<Imagem, arquivo (PDF), link com Diagrama de Caso de Uso.>*

  ***2.7. Diagramas de Atividades***

*<Imagem, arquivo (PDF), link com Diagrama de Atividades.>*

  ***2.8. Matrizes de Rastreabilidade***

*<Imagem, arquivo (PDF), link com Matriz de Rastreabilidade.>*

  ***2.9. Protótipos***

*<Imagem, arquivo (PDF), link com Protótipo.>*

## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*

[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
