# Partiu Aula

O **Partiu Aula** é um protótipo web de caronas colaborativas para estudantes. A proposta é aproximar quem precisa chegar ao campus de quem pode oferecer uma carona, ajudando a organizar o trajeto e dividir custos. O projeto tem como referência a comunidade do IFTO — Campus Paraíso.

> Este repositório contém um MVP demonstrativo no navegador. Não há servidor, autenticação, banco de dados ou integração real com mapas, pagamentos e notificações.

## Funcionalidades do protótipo

- **Início:** atalhos para as áreas principais e caronas em destaque.
- **Buscar carona:** pesquisa por origem, destino, data e horário, com ordenação por horário, preço ou avaliação.
- **Detalhes e reserva:** consulta o trajeto, motorista, vagas, valor e ponto de encontro; solicitações ficam pendentes.
- **Oferecer carona:** valida e publica uma oferta com trajeto, data, horário, vagas, contribuição e ponto de encontro.
- **Minhas caronas:** lista ofertas e solicitações, permite filtrar categorias e cancelar itens.
- **Mensagens e perfil:** telas demonstrativas de conversa, perfil e avaliações.

As caronas iniciais são dados de exemplo definidos em `app.js`. Ofertas, solicitações e alertas de busca são gravados no `localStorage` do navegador. Mensagens são adicionadas apenas à tela atual; o chat não é sincronizado entre usuários. A confirmação de reserva, notificações, avaliação de viagens e edição de perfil não possuem fluxo funcional completo.

## Estrutura do repositório

| Caminho | Conteúdo |
| --- | --- |
| `index.html` | Estrutura das telas, formulários e navegação. |
| `styles.css` | Estilos responsivos, componentes e estados de foco. |
| `app.js` | Dados de demonstração, navegação, busca e interações. |
| `docs/requirements.md` | Objetivos, público, requisitos funcionais e cenários de uso. |
| `docs/*.png` | Capturas de tela e referências visuais do projeto. |

## Como executar

Não há etapa de build nem dependências para instalar. Abra `index.html` diretamente em um navegador moderno. Para servir os arquivos por HTTP a partir da raiz do repositório:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000`. Os dados ficam no armazenamento local do navegador utilizado; limpar os dados do site remove as informações salvas pelo protótipo.

## Acessibilidade e layout

A interface está em português (`pt-BR`), inclui link para pular ao conteúdo, foco visível para teclado, rótulos nos campos e adaptação para telas menores. Também respeita a preferência do sistema por movimento reduzido. As fontes DM Sans e Manrope são carregadas do Google Fonts; sem conexão, o navegador usa fontes alternativas.

## Desenvolvimento e validação

Mantenha os arquivos sem dependências desnecessárias e preserve a separação entre estrutura (`index.html`), apresentação (`styles.css`) e comportamento (`app.js`). Não existe framework de testes ou comando automatizado de validação. Ao alterar o protótipo, confira manualmente navegação, busca e ordenação, detalhes e reserva, publicação e validação de oferta, visualização/cancelamento de caronas, foco por teclado e layout móvel.

Os requisitos de produto e cenários descritos em `docs/requirements.md` orientam a evolução. Esse documento também registra funcionalidades previstas que ainda não estão implementadas integralmente no MVP.

## Créditos e escopo do projeto

O projeto foi proposto para a comunidade estudantil do IFTO — Campus Paraíso. A documentação de requisitos identifica como integrantes Ana Luísa Neiva, Emilly Roanny, Geovanna Gabrielly e João Guilherme, sob orientação do professor Pedro Henrique Amaral. Consulte `docs/requirements.md` para detalhes da proposta e do protótipo visual.
