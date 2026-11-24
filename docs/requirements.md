# Requirements — Partiu Aula

## 1. Identificação do projeto

- **Projeto:** Partiu Aula — aplicativo de caronas para estudantes
- **Instituição:** IFTO — Campus Paraíso
- **Turma:** 3ª série do Ensino Médio
- **Integrantes:** Ana Luísa Neiva, Emilly Roanny, Geovanna Gabrielly e João Guilherme
- **Professor:** Pedro Henrique Amaral

## 2. Descrição e justificativa

O Partiu Aula é uma proposta de aplicativo que conecta estudantes que precisam de transporte com outros estudantes que podem oferecer caronas. O projeto busca facilitar o deslocamento até as instituições de ensino, reduzir os gastos com transporte e incentivar a colaboração entre os alunos.

Estudantes do ensino médio, de cursos técnicos e do ensino superior enfrentam dificuldades para chegar às instituições de ensino devido ao alto custo do transporte público ou privado, às longas distâncias, à frota escassa e aos horários incompatíveis. Essas situações podem gerar atrasos, insegurança e desgaste financeiro.

**Objetivo principal:** conectar estudantes motoristas e passageiros que realizam trajetos acadêmicos semelhantes, promovendo caronas colaborativas, seguras, econômicas e acessíveis.

## 3. Público-alvo

Estudantes do ensino médio, cursos técnicos, institutos federais e universidades que buscam alternativas de transporte mais práticas e econômicas para chegar às aulas.

## 4. Persona principal

**Nome:** Ana Clara  
**Idade:** 17 anos  
**Perfil:** estudante do ensino médio em um Instituto Federal. Mora longe do campus e depende diariamente de transporte para assistir às aulas.

- **Necessidades:** encontrar caronas confiáveis, economizar dinheiro, organizar seus horários, reduzir os custos mensais com deslocamento e manter a pontualidade.
- **Dificuldades:** orçamento financeiro limitado, gastos com transporte, distância entre casa e escola, transporte público lotado ou demorado e poucas opções de trajetos diretos.
- **Objetivo:** chegar às aulas com mais praticidade, segurança e economia.

## 5. Requisitos funcionais

| ID | Requisito | Descrição |
|---|---|---|
| RF01 | Buscar caronas | Permitir pesquisar viagens informando origem, destino, data e horário. |
| RF02 | Filtrar resultados | Permitir filtrar ou ordenar as caronas pelo horário mais próximo e pelo menor valor. |
| RF03 | Exibir resultados | Apresentar caronas disponíveis com foto e nome do motorista, trajeto, horário, vagas restantes e preço. |
| RF04 | Consultar detalhes | Exibir informações da carona, mapa do trajeto, perfil resumido do motorista e suas avaliações. |
| RF05 | Solicitar reserva | Permitir que o passageiro solicite uma vaga em uma carona disponível. |
| RF06 | Atualizar reserva | Registrar a solicitação como “Pendente” e apresentar “Confirmado” quando a carona for aceita. |
| RF07 | Oferecer carona | Permitir cadastrar origem, instituição de destino, itinerário, horário de saída, quantidade de vagas e valor sugerido por passageiro. |
| RF08 | Publicar carona | Validar os dados preenchidos, confirmar a publicação e inserir a oferta na lista de buscas ativas. |
| RF09 | Gerenciar minhas caronas | Permitir visualizar e organizar viagens solicitadas, oferecidas, agendadas, concluídas e passadas. |
| RF10 | Cancelar carona | Disponibilizar uma opção de cancelamento na área “Minhas Caronas”. |
| RF11 | Conversar pelo chat | Permitir a comunicação direta entre motoristas e passageiros. |
| RF12 | Exibir status de mensagem | Apresentar o status online e a confirmação de leitura das mensagens. |
| RF13 | Compartilhar localização | Permitir o envio rápido da localização pelo chat. |
| RF14 | Avaliar viagem | Permitir atribuir uma nota de 1 a 5 estrelas e escrever um comentário após a viagem. |
| RF15 | Exibir perfil e avaliações | Apresentar foto, dados do usuário, instituição de ensino cadastrada, nota média e comentários recebidos. |
| RF16 | Enviar notificações | Notificar o motorista sobre novas solicitações e informar os usuários sobre atualizações relevantes da carona. |
| RF17 | Criar alerta de carona | Quando a busca não encontrar opções, permitir criar um alerta para receber aviso caso apareça uma vaga. |

## 6. Requisitos de interface e telas

Os documentos de cenários identificam sete telas principais. O protótipo visual anexado também apresenta telas de abertura, login/cadastro e tela inicial.

| Tela | Finalidade | Elementos identificados |
|---|---|---|
| **Splash / Abertura** | Apresentar a identidade do aplicativo. | Nome “Partiu Aula”, símbolo de carro com capelo e frase “Juntos no mesmo destino.” |
| **Login / Cadastro** | Permitir a entrada ou o cadastro do usuário. | Opções “Entrar” e “Cadastrar”, além de opções de acesso por contas externas ilustradas no protótipo. |
| **Tela Inicial (Home)** | Apresentar atalhos e caronas próximas. | Saudação ao usuário, atalhos “Buscar carona”, “Oferecer carona” e “Minhas caronas”, lista de próximas caronas e navegação inferior. |
| **1. Tela Inicial / Busca** | Permitir pesquisar caronas por origem, destino e horário. | Campos de origem e destino, seletor de data e horário e botão “Buscar”. No protótipo aparecem “Minha localização” e a instituição de destino. |
| **2. Resultados da Busca** | Apresentar opções de carona disponíveis. | Cards com nome do motorista, trajeto, horário, preço e botão “Ver detalhes”; o documento de interface também prevê foto e vagas restantes. |
| **3. Detalhes & Reserva** | Exibir informações completas da viagem e permitir solicitar uma vaga. | Mapa do trajeto, perfil resumido do motorista, pontuação, avaliações e botão “Solicitar Reserva”. |
| **4. Minhas Caronas** | Gerenciar as viagens do usuário. | Abas para caronas solicitadas, oferecidas e passadas; o documento também prevê “Próximas” e “Histórico”, status da reserva, cancelamento e acesso ao chat. |
| **5. Chat / Mensagens** | Permitir comunicação direta entre motorista e passageiros. | Caixa de diálogo em tempo real, status online e envio rápido de localização. |
| **6. Perfil e Avaliações** | Exibir dados e reputação do usuário. | Foto ou identificação do perfil, nome, e-mail exibido no protótipo, nota média, quantidade de avaliações e acesso às caronas e avaliações. |

## 7. Cenários de uso

### 7.1. Busca e reserva de carona

**Situação:** Ana Clara precisa chegar ao Instituto Federal às 07h30 para uma prova. O ônibus habitual atrasou e ela procura uma carona rápida e acessível.

**Objetivo:** encontrar um estudante motorista com trajeto compatível e reservar uma vaga.

**Ações do usuário:**
1. Abre o aplicativo e seleciona “Buscar Carona”.
2. Informa o ponto de partida, o destino, a data e o horário de chegada.
3. Filtra os resultados pelo horário mais próximo e pelo menor valor.
4. Seleciona uma carona e clica em “Solicitar Reserva”.

**Resposta do sistema:** exibe os trajetos disponíveis com foto do motorista, horário e valor; atualiza o pedido para “Pendente” e envia uma notificação ao motorista.

**Resultado esperado:** após a confirmação, a carona aparece em “Minhas Caronas”, com as informações do ponto de encontro e da viagem.

### 7.2. Oferta e cadastro de nova carona

**Situação:** Lucas, estudante universitário que vai de carro para o campus todos os dias, deseja compartilhar os custos de combustível oferecendo três vagas no veículo.

**Objetivo:** cadastrar um trajeto recorrente de ida e volta e disponibilizar vagas para outros estudantes.

**Ações do usuário:**
1. Acessa o menu principal e seleciona “Oferecer Carona”.
2. Preenche origem, instituição de destino, itinerário, horário de saída e quantidade de vagas.
3. Define o valor sugerido de contribuição por passageiro e seleciona “Publicar Carona”.

**Resposta do sistema:** valida as informações, confirma a publicação com uma mensagem de sucesso e insere a oferta na listagem de buscas ativas.

**Resultado esperado:** a viagem passa a constar como ativa no painel do motorista e fica disponível para receber solicitações.

### 7.3. Comunicação via chat e avaliação pós-viagem

**Situação:** Ana Clara teve sua carona aceita, mas precisa combinar com o motorista um ponto de referência exato para o embarque.

**Objetivo:** esclarecer dúvidas sobre o embarque e registrar uma avaliação após a viagem.

**Ações do usuário:**
1. Acessa “Minhas Caronas”, seleciona a viagem confirmada e abre o “Chat”.
2. Envia uma mensagem combinando o ponto de encontro e aguarda a resposta.
3. Após o encerramento do trajeto, seleciona “Avaliar Viagem”, atribui uma nota e deixa um comentário.

**Resposta do sistema:** envia as mensagens com confirmação de leitura e, após a viagem, salva a nota e o comentário, atualizando a média no perfil do motorista.

**Resultado esperado:** o embarque é alinhado entre os usuários e a avaliação é contabilizada no perfil.

## 8. Requisitos de usabilidade e tratamento de situações

- **Ponto de encontro:** a etapa de alinhamento do ponto de encontro pode gerar dúvidas. A interface deverá oferecer sugestões de pontos de referência conhecidos, como pontos de ônibus e portões do campus.
- **Confirmação de ações:** o sistema deverá utilizar feedback visual e sonoro imediato, mensagens no estilo toast/banner, alteração clara do status para “Confirmado” e notificações push no celular.
- **Busca sem resultados:** quando nenhuma carona for encontrada, o sistema deverá apresentar uma tela informativa (empty state) e permitir a criação de um “Alerta de Carona”.
- **Erros de preenchimento:** os campos incorretos deverão ser destacados em vermelho, com mensagens claras e sem termos técnicos.
- **Testes de usabilidade:** a equipe deverá testar o protótipo de baixa fidelidade com estudantes que correspondam ao perfil da persona. Deverão ser observados o tempo de execução das tarefas, a taxa de sucesso e os pontos de hesitação durante o uso simulado.

## 9. Critérios de aceitação derivados dos cenários

1. **Busca:** ao informar origem, destino, data e horário, o usuário consegue visualizar as caronas disponíveis e filtrar os resultados por horário e valor.
2. **Reserva:** ao solicitar uma vaga, o pedido fica com status “Pendente” e o motorista recebe uma notificação. Após a confirmação, o status é atualizado e a viagem aparece em “Minhas Caronas”.
3. **Oferta:** ao preencher os dados da carona e publicá-la, o sistema valida as informações, exibe uma confirmação e inclui a oferta nas buscas ativas.
4. **Chat:** a partir de uma viagem em “Minhas Caronas”, os usuários conseguem abrir o chat e trocar mensagens.
5. **Avaliação:** após a viagem, o usuário consegue registrar uma nota e um comentário, que são exibidos no perfil e considerados na média.
6. **Busca sem resultados:** quando não houver caronas disponíveis, o sistema oferece a criação de um alerta.
7. **Erro de preenchimento:** quando houver informação incorreta, o sistema identifica o campo e apresenta uma mensagem clara para orientar a correção.

## 10. Referência do protótipo

O arquivo de proposta visual apresenta telas de abertura, login/cadastro, home, busca de carona, resultados, minhas caronas e perfil. O protótipo está indicado no seguinte link:

[Protótipo Partiu Aula no Figma](https://www.figma.com/design/2fFGP1rJzbjeAuJVZ7F7fU/Partiu-Aula?node-id=0-1&t=WuZ9wCzEjix9QhSt-1)

## 11. Observações sobre o escopo

Este documento reúne o conteúdo da **Proposta de Projeto**, do documento **Cenários de Uso & Requisitos de Interface** e das telas apresentadas no PDF do protótipo.

Foram organizados os requisitos descritos nos materiais, sem definir detalhes técnicos que não aparecem nas fontes, como tecnologia de desenvolvimento, banco de dados, autenticação, regras completas de privacidade, integração efetiva com mapas ou forma de pagamento.
