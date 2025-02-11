---
title: Redes
description: Uma visão geral das redes Ethereum e onde obter ether (ETH) da rede de testes para testar seu aplicativo.
lang: pt-br
---

Redes são ambientes diferentes do Ethereum que você pode acessar para desenvolvimento, teste ou produção. Como o Ethereum é um protocolo, podem existir várias "redes" independentes em conformidade com o protocolo sem interagir umas com as outras.

Sua conta Ethereum funcionará nas diferentes redes, mas o saldo da sua conta e o histórico de transações não serão transferidos da rede Ethereum principal. Para fins de teste, é útil saber quais redes estão disponíveis e como obter a rede de testes ETH para brincar. Em geral, por razões de segurança, não é recomendado reutilizar contas da rede principal em redes de testes ou vice-versa.

## Pré-requisitos {#prerequisites}

Você deveria entender as [noções básicas do Ethereum](/developers/docs/intro-to-ethereum/) antes de ler sobre as diferentes redes, pois as redes de teste lhe darão uma versão barata e segura do Ethereum para brincar.

## Redes públicas {#public-networks}

As redes públicas são acessíveis a qualquer pessoa no mundo com uma conexão à Internet. Qualquer um pode ler ou criar transações em uma blockchain pública e validar as transações que estão sendo executadas. O consenso entre os pares decide sobre a inclusão de transações e o estado da rede.

### Rede Principal Ethereum {#ethereum-mainnet}

A rede principal é a blockchain de produção Ethereum pública primária, onde as transações de valor real ocorrem no livro-razão distribuído.

Quando as pessoas e as exchanges discutem os preços do ETH, eles estão falando sobre a rede principal ETH.

### Redes de Testes Ethereum {#ethereum-testnets}

Além da rede principal, existem redes de teste públicas. Essas são redes usadas por desenvolvedores de protocolo ou desenvolvedores de contrato inteligente para testar as atualizações de protocolo e também os contratos inteligentes em potencial em um ambiente de produção antes da implantação na rede principal. Pense nisso como um análogo a servidores de produção versus servidores de teste.

Você deve testar qualquer código de contrato que você escrever em uma rede de testes antes de publicar na Rede principal. Entre os dapps que se integram com contratos inteligentes existentes, a maioria dos projetos tem cópias publicadas em redes de teste.

A maioria das redes de teste começou usando um mecanismo de consenso de prova de autoridade permitido. Isso significa que um pequeno número de nós é escolhido para validar as transações e criar novos blocos, incluindo sua identidade no processo. Como alternativa, algumas redes de testes apresentam um mecanismo de consenso de prova de participação aberto, no qual todos podem testar a execução de um validador, assim como a Rede principal do Ethereum.

O ETH em redes de teste não tem valor real; portanto, não há mercados para ETH de redes de teste. Como você precisa do ETH para interagir de fato com o Ethereum, a maioria das pessoas obtém o ETH via "torneiras". A maioria das torneiras são aplicativos Web em que você pode inserir um endereço para o qual deseja que o ETH seja enviado.

#### Qual rede de testes devo usar?

As duas redes de testes públicas que os desenvolvedores dos clientes estão atualmente mantendo são Sepolia e Goerli. Sepolia é uma rede para desenvolvedores de contrato e aplicativos para testar seus aplicativos. A rede Goerli permite que os desenvolvedores de protocolo testem atualizações de rede e permite que os participantes façam testes usando validadores.

#### Sepolia {#sepolia}

\*\*\*\*Sepolia é a rede de teste padrão recomendada para desenvolvimento de aplicativos. A rede Sepolia usa um conjunto de validadores autorizados. É bastante novo, o que significa que seu estado e história são bastante pequenos. Isso significa que a rede é rápida para sincronizar e que a execução de um nó requer menos armazenamento. Isso é útil para usuários que desejam ativar rapidamente um nó e interagir diretamente com a rede.

- Conjunto de validadores fechado, controlado pelo cliente & equipes de teste
- Nova rede de teste, menos aplicativos implantados que outras redes de teste
- A sincronização rápida e a execução de um nó exigem um espaço de disco mínimo

##### Recursos

- [Website](https://sepolia.dev/)
- [GitHub](https://github.com/eth-clients/sepolia)
- [Otterscan](https://sepolia.otterscan.io/)
- [Etherscan](https://sepolia.etherscan.io)

##### Faucets

- [Faucet do QuickNode Sepolia](https://faucet.quicknode.com/drip)
- [Grabteeth](https://grabteeth.xyz/)
- [Faucet de PoW](https://sepolia-faucet.pk910.de/)
- [Faucet da Carteira da Coinbase | Sepolia](https://coinbase.com/faucets/ethereum-sepolia-faucet)
- [Faucet do Alchemy Sepolia](https://sepoliafaucet.com/)
- [Faucet do Infura Sepolia](https://www.infura.io/faucet)

#### Goerli _(suporte a longo prazo)_ {#goerli}

_Nota: [a rede de testes Goerli está obsoleta](https://ethereum-magicians.org/t/proposal-predictable-ethereum-testnet-lifecycle/11575/17) e será substituída por [Holesovice](https://github.com/eth-clients/holesovice) em 2023. Considere migrar seus aplicativos para a Sepolia._

Goerli é a rede de testes usada para testar a validação e a participação. A rede Goerli está aberta para usuários que queiram executar um validador na rede de testes. Os participantes que desejam testar atualizações de protocolo antes de serem implantados na rede principal devem, portanto, usar a Goerli.

- Conjunto de validadores abertos, com o qual os participantes podem testar atualizações de rede
- Estado grande, útil para testar interações complexas de contratos inteligentes
- Mais longo para sincronizar e requer mais armazenamento para executar um nó

##### Recursos

- [Site](https://goerli.net/)
- [GitHub](https://github.com/eth-clients/goerli)
- [Etherscan](https://goerli.etherscan.io)

##### Faucets

- [Faucet Goerli do QuickNode](https://faucet.quicknode.com/drip)
- [Grabteeth](https://grabteeth.xyz/)
- [Faucet de PoW](https://goerli-faucet.pk910.de/)
- [Faucet Goerli](https://faucet.goerli.mudit.blog/)
- [Faucet do Paradigm](https://faucet.paradigm.xyz/)
- [Faucet Goreli do Alchemy](https://goerlifaucet.com/)
- [Todas as faucets do nó Goerli](https://www.allthatnode.com/faucet/ethereum.dsrv)
- [Faucet da Carteira Coinbase | Goerli](https://coinbase.com/faucets/ethereum-goerli-faucet)

Para iniciar um Validador na rede de testes Goerli, use a barra de inicialização ["validador goerli barato"](https://goerli.launchpad.ethstaker.cc/en/) do ethstaker.

#### Rinkeby _(descontinuada)_ {#rinkeby}

_Observação: [a rede de testes Rinkeby foi descontinuada](https://blog.ethereum.org/2022/11/30/ropsten-shutdown-announcement) e não receberá mais atualizações de protocolo. Considere migrar seus aplicativos para a Sepolia._

Uma rede de testes de prova de autoridade para aqueles que executam versões antigas do cliente Geth.

##### Faucets

- [FaucETH](https://fauceth.komputing.org) (torneira multi-cadeia sem a necessidade de conta social)
- [Faucet Chainlink](https://faucets.chain.link/)
- [Faucet Paradigm](https://faucet.paradigm.xyz/)
- [Faucet Rinkeby](https://faucet.rinkeby.io/)

### Redes de testes de camada 2 {#layer-2-testnets}

[Camada 2 (L2)](/layer-2/) é um termo coletivo para descrever um conjunto específico de soluções de escalabilidade do Ethereum. Uma camada 2 é uma cadeia de blocos separada que estende o Ethereum e herda as garantias de segurança do Ethereum. Normalmente, as redes de teste de camada 2 estão fortemente associadas às redes de testes públicas do Ethereum.

#### Arbitrum Goerli {#arbitrum-goerli}

Uma rede de testes para [Arbitrum](https://arbitrum.io/).

##### Faucets

- [Faucet Chainlink](https://faucets.chain.link/)

#### Goerli otimista {#optimistic-goerli}

Uma rede de testes para [Optimism](https://www.optimism.io/).

##### Faucets

- [Faucet do Paradigm](https://faucet.paradigm.xyz/)
- [Coinbase Wallet Faucet | Optimism Goerli](https://coinbase.com/faucets/optimism-goerli-faucet)

## Redes privadas {#private-networks}

Uma rede Ethereum é uma rede privada se seus nós não estiverem conectados a uma rede pública (ex: Rede principal e rede de testes). Neste contexto, privado significa apenas reservado ou isolado, em vez de protegido ou seguro.

### Redes de desenvolvimento {#development-networks}

Para desenvolver um aplicativo Ethereum, você deve executá-lo em uma rede privada para ver como funciona antes de implantá-lo. Tal como você pode criar um servidor local em seu computador para desenvolvimento Web, você pode criar uma instância local de cadeia de blocos para testar seu dapp. Isso permite uma iteração muito mais rápida do que uma rede de testes pública.

Existem projetos e ferramentas dedicadas a ajudá-lo com isso. Saiba mais sobre [redes de desenvolvimento](/developers/docs/development-networks/).

### Redes de consórcio {#consortium-networks}

O processo de consenso é controlado por um conjunto predefinido de nós confiáveis. Por exemplo, uma rede privada de instituições acadêmicas conhecidas, cada uma administrando um único nó, e os blocos são validados por um limite de signatários dentro da rede.

Se uma rede pública Ethereum é como a internet pública, uma rede de consórcio é como uma intranet privada.

## Ferramentas relacionadas {#related-tools}

- [Chainlist](https://chainlist.org/) _Lista de redes EVM para conectar carteiras e fornecedores aos identificadores de cadeia e rede apropriados_
- [/Cadeias baseadas na EVM](https://github.com/ethereum-lists/chains) _repositório do GitHub com metadados de cadeias que alimenta a Chainlist_

## Leitura adicional {#further-reading}

- [Proposta: Ciclo de vida previsível da rede de testes do Ethereum](https://ethereum-magicians.org/t/proposal-predictable-ethereum-testnet-lifecycle/11575/17)
- [A evolução das redes de testes do Ethereum](https://etherworld.co/2022/08/19/the-evolution-of-ethereum-testnet/)
