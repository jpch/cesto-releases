# Novidades

Alterações visíveis da app Cesto, da mais recente para a mais antiga.
O formato segue o [Keep a Changelog](https://keepachangelog.com/pt-PT/1.1.0/).

## [Por publicar]

## [1.8.0] - 2026-11-03
### Adicionado
- Compatível com o add-on Cesto 2.0.0: a sessão do Continente passa a viver no add-on Continente MCP. Um indicador vermelho «Add-on Continente indisponível» (também nas Definições) avisa quando esse add-on não responde.
- «Iniciar sessão no Continente», no início quando a sessão expirou e nas Definições, abre a página do add-on Continente MCP no Home Assistant. Não é preciso voltar a ligar o telemóvel.

## [1.7.1] - 2026-11-02
### Corrigido
- Fora de casa, o indicador mostra «Fora de casa (via Home Assistant): lista e carrinho» quando a opção `remote_cart` do add-on está ligada, em vez de dizer sempre que só a lista está disponível.

## [1.7.0] - 2026-11-01
### Adicionado
- «Produtos já enviados» (add-on 1.9.0+) substitui «Listas anteriores»: os produtos já enviados para o carrinho, os mais frequentes primeiro, com seleção múltipla e «Adicionar à lista (N)». Funciona fora de casa.
- Ajuda no campo de produto da lista, com um «?» que abre «Como escolhemos o produto».
### Alterado
- Todos os ecrãs interiores têm uma barra superior com seta para voltar, sem ficar por baixo da barra de estado.
- Ligar um produto ao editar um artigo abre o ecrã «Procurar produto».
### Removido
- O ecrã de listas arquivadas.

## [1.6.0] - 2026-11-01
### Adicionado
- Botão de atualizar e puxar para atualizar no início, que voltam a verificar a ligação e a sessão do Continente (add-on 1.8.0+).
- Indicador verde «Sessão Continente válida».
- Ecrã «Procurar produto»: procura escrita com resultados no mesmo ecrã e câmara em «Ler com a câmara».
- Na lista, «Procurar no Continente» abre a procura com o texto já escrito.
### Alterado
- Novos botões na lista e novos atalhos no início («Procurar produto», «Procurar promoções para o carrinho», «Carrinho no Continente»).
### Removido
- Ditado por voz e o botão «Adicionar por foto» da lista.

## [1.5.0] - 2026-10-31
### Adicionado
- Carrinho fora de casa: preparar, escolher, pré-visualizar, aplicar e procurar promoções através do Home Assistant, quando a opção `remote_cart` do add-on (1.7.0+) está ligada. Com a opção desligada, a app explica que só a lista funciona fora de casa e como ativar a opção.
- A pré-visualização fora de casa já não fica pendurada à espera do add-on.
### Corrigido
- As operações do carrinho seguem a ligação atual (casa ou Home Assistant) em vez de usarem sempre a rede de casa.

## [1.4.0] - 2026-10-31
### Alterado
- Novo aspeto das promoções: cada produto mostra a «Escolha atual», as opções em «Mudar escolha», os produtos «Em promoção» e os «Mais barato por litro/kg» comparados com a escolha atual.
- Depois da procura aparece uma vista geral com resumo e filtros (Todos / Promoção / Mais barato / Sem nada).
- A última proposta aparece logo ao abrir o ecrã enquanto é atualizada.
### Corrigido
- Alternativas mais baratas comparadas com a promoção errada e produtos repetidos (com add-on 1.6.0+).
- Não era possível escolher uma promoção ou alternativa que não estivesse nas opções.

## [1.3.0] - 2026-10-31
### Adicionado
- «Procurar promoções» mostra o progresso (add-on 1.4.0+) e pode ser cancelado, mostrando as promoções já encontradas.
- Resumo dos resultados, preço por litro ou kg, desconto e lista «Mais barato por litro/kg».

## [1.2.4] - 2026-10-31
### Corrigido
- Aviso «O servidor demorou demasiado a responder» sobre uma proposta que tinha carregado bem; os erros de promoções aparecem junto ao botão.

## [1.2.3] - 2026-10-31
### Corrigido
- «Preparar carrinho» já não fica parado nem termina em «Não foi possível contactar o servidor» (add-on 1.3.1+); mostra o progresso da procura.
- Mensagens de erro claras (tempo esgotado, sessão do Continente expirada, supermercado indisponível) e botão «Voltar» sempre visível.

## [1.2.2] - 2026-10-31
### Corrigido
- Uma alteração que não pode ser enviada já não bloqueia a sincronização; é descartada e indicada no aviso.

## [1.2.1] - 2026-10-31
### Corrigido
- «Falha ao sincronizar» quando um artigo da lista estava ligado a um produto do Continente.
### Alterado
- A lista explica a causa real de uma falha de sincronização (sem ligação, telemóvel desligado do add-on, versões incompatíveis, erro do servidor).

## [1.2.0] - 2026-10-31
### Adicionado
- Procura no Continente fora de casa (add-on 1.2.0+).
### Corrigido
- O acesso fora de casa através do Home Assistant não funcionava. Não é preciso voltar a ligar o telemóvel.

## [1.1.0] - 2026-10-31
### Adicionado
- Miniaturas dos produtos na pré-visualização, nas promoções e na procura.
- Tocar num artigo da lista para editar nome, quantidade, unidade, nota e produto ligado, também sem ligação.
### Alterado
- Apagar um artigo deslizando-o para o lado.
### Corrigido
- Alterações feitas sem ligação ao add-on perdiam-se em vez de ficarem à espera.

## [1.0.0] - 2026-10-31
### Alterado
- A app passa a chamar-se **Cesto** (pacote `app.cesto`, instala-se como app nova). Funciona com o add-on Cesto 1.0.0.
- «Procurar na rede» encontra o Home Assistant e usa a porta 8099 do add-on.
- APK publicados em cesto-releases para o Obtainium.
### Adicionado
- Assistente inicial: ler o código QR do add-on, procurar na rede ou escrever os dados.
- Pergunta «Em que supermercado compras?» quando há vários supermercados, e Definições > Supermercados.
- Funcionalidades que o supermercado não suporta ficam escondidas.
- Licença MIT.
