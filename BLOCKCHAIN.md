# O presente repósitorio será o local onde terei a adição dos resumos feitos durante o estágio

## Neste segundo momento falaremos sobre:

- **Bitcoin e Blockchain**
- **Assinaturas Digitais**
- **Moeda Digital**
- **Proof of work**
- **Evitando Gasto Duplo**
- **Carteiras Digitais**
- **Anonimato**
---


# Bitcoin e Blockchain

O Blockchain foi apresentado como um sistemas que permite você adicionar dados e não pode alterar. Possui um mecânismo em que as duas partes envolvidas precisam estar em consenso. Isso foi apresentado em etapas, sua explicação podendo ser compreendida de uma criança a um especialista na área.

O Bitcoin é visto como uma unidade de troca, uma reserva de valor. Foi idealizada em 2008 em um artigo de Satoshe Nakamoto, um pseudônimo. Pontos importantes são: *Criptografia*, *Blockchain*, *Redes descentralizadas* e *Engenharia de Incentivo*. Em 2009 surgiu o primeiro bloco do Blockchain ( Genesis Block). Vamos analisar as caracteristicas entre o Bitcoin e os sistemas tradicionais ou os Bancos.

| Caracteristicas       | Sistema Tradicional      | Bitcoin  |
|---------              |--------------            |----------    |
| Contabilidade         | Centralizado             |Blockchain       |
| Armazenamento         | Fracionado               |100%     |
| Segurança             | Institucional            |Criptográfia |
| Emissão de moeda      | Politica economica       |Algoritmos |
| Transações            | Centralizado             |Distribuido, peer-to-peer |
| Autenticação          | Centralizado             |Blockchain      |
| Regulamentação        | Banco central, Normas    |Ainda indefinida |
| Processo de decisão   | Arbitrário               |Consenso     |
| Controle do dinheiro  | Banco                    |Você |
----   

O blockchain tem um mecânismo que auxilia em sua segurança com relação a tentativas de fraudes, esse sistema funciona como correntes, onde um bloco sempre aponta para outro, ou seja, se houver uma tentativa de alteração no bloco ele precisaria mudar também os dados dos blocos subsequentes aquele, o que é uma coisa bastante improvável, pois a capacidade de poder computacional para isso é enorme. Então com relação a seu funcionamento, existem as **Assinaturas Digitais**, em visão geral se trata de um mecânismo onde: Só você pode assinar( Quem possui a chave, falaremos a seguir); Qualquer um pode verificar a assinatura e Assinatura atrelada ao documento. Sobre seu funcionamento, esse sistema funciona com base no par de *Chave secreta*(Que deve permanecer em segredo, pois esse sistema de validação é com base nessa verificação de chave, assim quem possui essa chave secreta a priori é o dono dela) e a *Chave pública* que é atrelada ao documento, em resumo, ao assinar um documento você usará a chave secreta, ela então fará uma chave pública para aquele documento baseada no hash. Algumas propriedades da chave pública são:
- Impossivel de falsificar
- Fácil de verificar
- Atrelada ao documento

Então com isso foi apresentado como **Criar uma Moeda Digital**, de inicio vamos falar sobre *hash*, onde o hash do bloco é como se fose seu nome:
- Transforma um texto de entrada de qualquer tamanho em um texto de saída de tamanho fixo, por exemplo os codigos de barras.
Então as funções hash criptográficas são:
- Fácil de computar
- Livre de colisão: Impossivel* dois inputs com o mesmo output           **muito, muito improvável**
- Unidirecional: Impossivel* descobrir o input dado seu output
- "Puzzle Friendly": Se modifica pouco na entrada muda muito na saída.

Ou seja, é inviável alterar os dados de um bloco, pois a hash é gerada pela entrada, alterando os dados, o hash muda, com isso toda a sequência que guardavam os dados da hash que foi alterada é quebrado, resultando em uma dependência de mudança em cadeia. Cada bloco armazena os dados relativos o seu hash e o hash do bloco anterior.

Foi então exemplificado os passos e caracteristicas das moedas e nesse exemplo havia uma unidade central que controlava o funcionamento, usada apenas para dar base para a compreensão, pois no **Bitcoin** essa unidade central é substituida por uma rede de computadores, sendo distribuida, sem hierarquia e baseada em protocolo de consenso, com isso qualquer computador conectado à rede blockchain é um nó desta rede, onde temos:
- Full Nodes:(Nós completos, mineradores)
  - Validam todas as transaçôes emeitidas pela rede
  - Mantêm a consistência da blockchain
- Lite Nodes:(Nós mais leves, podem ser carteiras)
  - Não armazenam toda a blockchain
  - Necessitam de informação de outros nós.

As transações possui os seguintes itens, assinatura, as moedas criadas para essa transação e a chave pública para quem está sendo enviada e as moedas que foram consumidas, para isso, as transações de bitcoin só são inseridas na blockchain quando são validadas pelos mineradores que também garante que todos os nós mantenham a mesma blockchain armazenada. Os mineradores então:
- Validam as transações recebidas e criam novos blocos
- Competem entre si pelo direito de adicionar o próximo bloco na blockchain
- Verificam blocos obtidos por outros mineradores e adicionam a blockchain quando válidos
- Sempre extendem o ramo mais longo da blockchain

Para a mineração usam o **Proof of work** que é o metodo de consenso, os blocos possuem em seu hash uma combinação e quando um minerador encontra a correta, eles entam em um conseso implicito para a adição desse bloco na blockchain, isso se dá quando começam a minerar sobre esse novo bloco buscando a combinação correta para o próximo, isso acontece em um intervalo de 10 minutos, existe também o conceito de *coinbase translaction*, onde o ganho por mineração cai pela metade a cada 4 anos. Com base em tudo apresentado, mineração em casa é práticamente impossível, dado o grande consumo de energia e processamento e mesmo assim não da garantia de éxito, existem as *Mining pools*, ela vai centralizar e dividir o ganho proporcionalmente a mineração de cada minerador, ela reduz os ricos e tem otimização. Graças ao PoW não existe o gasto duplo, que consiste básicamente em usar as mesmas moedas mais de uma vez, para que funcionasse um hacker precisaria de 51% de hash power, ele precisa minerar 5x mais que outros mineradores.

**Carteiras** apresentam 3 pilares: Disponibilidades, segurança e conveniência. Para formatos existem, a carteira de papel, que é litealmente um pedaço de papel e tem sua segurança tanto quanto um papel, um ponto positivo é não está na rede, sendo imune* a hackers. As carteira de hardware apresentam muitas váriedades são as mais seguras e permitem multiplos pares de CP/CS, que é sempre recomendado ter mais de uma chave pública. Existem as carteiras de software que funcionam em descktop e mobile e é tão segura quanto seu computador e as carteiras online as mais práticas, porém menos seguras, você não consegue saber seus pares de chave pública e privada.

As **Exchanges** surgem para apresentar formas de negociar criptomoedas, em resumo, elas centralizam as negociações onde pessoas tem cripto e querem vender e pessoas tem dinheiro e querem comprar criptos. Elas são básicamente um site. Em comparação com os Bancos, bancos são regulados, as exchanges( ainda não), em resumo você não tem nenhuma segurança com relação aos investimentos, por isso é sempre recomendado pesquisar bem antes de tomar qualquer decisão e saber que está correndo um riscode perder tudo que está colocando a jogo alí. Ficar sempre atento para não cair em esquemas de pirâmides que geralmente são apresentados como *Marketing Multi Nível*, *Marketing de Rede*, garante retornos com x% de lucro, é difícil sair dele, e tem as propostas que que quanto mais pessoas novas você trouxer mais lucrará.

Muitos tem a visão de o bitcoin é uma moeda de hackers pelo fato do **Anonimato**, porém não se trata bem disso, ao menos não em um nível totalmente anônimo de funcionamento:
- Bitcoin ID = chave pública --> Pseudônimo
- Transações rastreavéis, para aumento de segurança é sempre aconselhado usar mais de uma chave pública, uma pra cada transação de preferência
- Anonimato: Pseudônimo + Irrastreável

De-Anonimizando o Bitcoin
  - Muitos serviços baseados em bitcoin requerem sua identidade ou infirmações a seu respeito, por exemplo as exchanges, com isso é possivel traçar uma rota de gastos analisando os historicos ligados a chave pública, mas para isso é necessário que a pessoa queira muito descobrir seus históricos de transação, por isso o número de chaves públicas ajudam na segurança, pois dificultará o trabalho, outro exemplos são as carteiras. Já meios indiretos estão relacionados a hábitos de uso, endereços IP.

Boas práticas para aumentar a segurança:
- Novo pagamento --> Nova chave pública
- Usar navegadores que minimize a exposição na rede (TOR Browswer)
- Virtual Private Network (VPN), sistemas que ajudem na segurança do IP
- Mixing, vai misturar as chaves publicas de pessoas que o usam
- Coinjoin

Como um complemento falemos brevemente sobre o **Ethereum** que é similiar ao bitcoin, fazendo parte desse universo de criptomoedas, uma coisa que vai diferir o ethereum do bitcoin é que ao invés da aplicação expecífica, ele tem diversas aplicações possíveis. Ela tem sua mineração em *memory hard* e suas transações envolvem processamento e tranferências, faz uso de Smart Contracts( Que consistem em um conjunto de regras combinadas entre duas ou mais partes, traduzidas em código computacional, verificável e auto executável, possuindo endereço e balanço) e suas Origens são mais claras. Coordenada pela fundação Ethereum, que não tem poder decisório oficialmente, mas ajuda nessa estrutura. Essa rede então faz uso da Ethereum Virtual Machine (EVM) que trás a possíbilidade de que todos nós da rede rodem todos os códigos dos blocos, sua linguagem é a *Solidity*, o **GAS** é quem faz esse controle de processamento, pois qualquer transação tem um custo e quanto + complexo + caro, evita loops, pois toda operação vai ser executada até acabar normalmente, ou até atingir o GAS Limit ou fazer uso de todo o GAS enviado, basicamente seguindo um exemplo de que para um automóvel funcionar ele precisa de combústivel. 
Existem os contratos de segurança, onde por exemplo algo só será realizado se tiver a assinatura das duas partes, os Smart Contracts onde a sua solicitação é convertida em um produto, por exemplo de uma máquina de refrigerante e contratos de governança, onde exitem tokens que dão poder de voto e decisão do futuro da empresa, por exemplo. E pra finalizar, os Dapps, aplicativos descentralizados que podem ou não usar blockchain, não tem intermediários, são open source, alguns exemplos são:
- EtherDelta: cobra taxas
- HyperDragons: jogo de estrategia possibilitando lucros, similar ao Criptokids
- geon: disponibiliza tokens e é uma ferramenta de marketing que você pode usar para promover seu estabelecimento ao permitir mineração naquela lugar específico
- Maker: Criou uma moeda(Maker) que sempre vale 1 dollar.