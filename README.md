# Partiu Aula

Protótipo web de uma plataforma de caronas entre estudantes. A proposta é ajudar alunos a encontrar colegas com trajetos compatíveis até o campus, combinar o embarque e dividir os custos da viagem.

> **Estado atual:** interface demonstrativa feita com HTML, CSS e JavaScript no navegador. Não há servidor, banco de dados, autenticação, integração de pagamentos nem notificações reais. Os nomes, perfis, avaliações e viagens iniciais são dados de exemplo.

## Conteúdo

- [Visão geral](#visão-geral)
- [Funcionalidades disponíveis](#funcionalidades-disponíveis)
- [Tecnologias e arquivos](#tecnologias-e-arquivos)
- [Como executar](#como-executar)
- [Dados e persistência](#dados-e-persistência)
- [Limitações do protótipo](#limitações-do-protótipo)
- [Referências do projeto](#referências-do-projeto)
- [Próximos passos](#próximos-passos)

## Visão geral

O Partiu Aula é voltado a estudantes que enfrentam dificuldades de deslocamento até a instituição de ensino, como custo, distância, horários rígidos e transporte público lotado. A interface atual apresenta um exemplo ambientado no IFTO — Campus Paraíso e usa o lema **“Juntos no mesmo destino”**.

O projeto prioriza caminhos simples para buscar ou oferecer uma carona, consultar solicitações, conversar sobre o ponto de encontro e visualizar informações de perfil. A identidade visual usa tons de verde, cartões e navegação adaptada a telas menores.

## Funcionalidades disponíveis

- **Início:** resumo e atalhos para buscar ou publicar uma carona, além de cartões de ofertas de exemplo.
- **Buscar carona:** pesquisa por origem, destino e data; permite inverter origem e destino, ordenar resultados por horário, valor ou avaliação e abrir detalhes de uma oferta.
- **Solicitar carona:** registra uma solicitação demonstrativa com status “Aguardando” e mostra uma mensagem de confirmação.
- **Oferecer carona:** formulário de origem, destino, data, horário, vagas, contribuição e ponto de encontro opcional. A oferta publicada aparece nos resultados da busca.
- **Minhas caronas:** consulta as listas de solicitadas, oferecidas e passadas; solicitações podem ser acompanhadas pelo status exibido.
- **Mensagens:** conversas e histórico de exemplo. É possível enviar mensagens na interface, mas elas não são entregues a outra pessoa.
- **Perfil e avaliações:** exibe informações e avaliações de exemplo; o fluxo demonstrativo permite registrar uma nota de 1 a 5 e um comentário opcional.
- **Estados e acessibilidade:** avisos temporários de confirmação, mensagens para busca sem resultados, navegação por teclado e adaptação para dispositivos móveis.

As telas incluem conteúdo pré-carregado para demonstrar os fluxos. A interface não implementa todos os requisitos descritos no documento de referência como serviços reais; consulte [Limitações do protótipo](#limitações-do-protótipo).

## Tecnologias e arquivos

O projeto não utiliza framework, gerenciador de dependências ou etapa de compilação.

| Arquivo ou pasta | Finalidade |
| --- | --- |
| `index.html` | Estrutura das telas, formulários, navegação e conteúdo da interface. |
| `styles.css` | Estilos, identidade visual, estados da interface e regras responsivas. |
| `app.js` | Navegação e interações do protótipo, renderização de caronas e persistência local. |
| `Docs/requirements (1).md` | Requisitos, cenários de uso, diretrizes de interface e questões em aberto. |
| `Docs/1.png`–`Docs/4.png` | Referências visuais fornecidas para o projeto. |

## Como executar

1. Baixe ou clone este repositório.
2. Abra `index.html` em um navegador moderno.

Também é possível iniciar um servidor estático local na pasta do projeto. Por exemplo, se Python estiver instalado:

```bash
python -m http.server 8000
```

Depois, acesse <http://localhost:8000>. Não é necessário instalar dependências. O servidor é opcional; a aplicação é composta por arquivos estáticos.

## Dados e persistência

As caronas e solicitações iniciais são definidas em `app.js`. Algumas alterações feitas durante o uso, como ofertas, pedidos, avaliações e ativação do aviso, são guardadas no `localStorage` deste navegador. Elas não são sincronizadas entre navegadores ou dispositivos e podem ser removidas ao limpar os dados locais do site.

O comportamento de `localStorage` depende de como o navegador trata arquivos abertos diretamente (`file://`). Para uma experiência mais previsível entre sessões, use um servidor estático local, conforme o comando acima.

## Limitações do protótipo

- Não há cadastro, login ou verificação real de vínculo estudantil; o usuário exibido é um exemplo.
- Não existe backend ou banco de dados compartilhado. O armazenamento é local ao navegador.
- A busca e as ofertas operam sobre dados de demonstração; não há localização, mapas ou cálculo de rota.
- Mensagens e avisos não são enviados a outros usuários nem por push, e-mail ou SMS.
- Os estados de solicitação, confirmação e conclusão são demonstrativos; não há fluxo real para motoristas aceitarem pedidos ou atualizarem uma viagem.
- Avaliações ficam no armazenamento local e não atualizam uma reputação compartilhada.
- Não há pagamentos, cancelamentos, denúncias, bloqueios ou mecanismos técnicos de segurança e privacidade.

O documento de requisitos também lista esses temas como aspectos que ainda precisam ser definidos antes de uma implementação de produção.

## Referências do projeto

Consulte `Docs/requirements (1).md` para os requisitos funcionais e não funcionais, cenários de uso, diretrizes extraídas do protótipo, observações de usabilidade e questões em aberto. As imagens `Docs/1.png` a `Docs/4.png` complementam esse material visualmente.

## Próximos passos

Antes de transformar o protótipo em um serviço real, será necessário definir autenticação e verificação de estudantes, regras para pedidos e cancelamentos, privacidade e retenção de dados, notificações, tratamento de incidentes e como será combinado ou processado o valor da contribuição. A escolha de tecnologias e plataformas também permanece em aberto nos documentos de referência.
