# Atelier - A.Y 

Site para compra de trajes formais de diversas culturas predominantes em cada continente do planeta.

**IMPORTANTE**: [**Cadastre seu projeto nesta planilha**](https://docs.google.com/spreadsheets/d/1bSb1-S9qOf46fNH8quyoFpcjcTuBMj_EdSPchOuFULY/edit?usp=sharing).

Professor: [Marco André Mendes](github.com/marcoandre)

Equipe:
- [Agatha Helena Schmidt de Oliveira](https://github.com/agathahelena)
- [Ana Laura Simonato](https://github.com/analaura3s)
- [Andressa Steffen](https://github.com/AndressaSteffen26)
- [Gabriela Heloisa Ramos](https://github.com/yuriramos223/yuriramos223)

Links do projeto:
(*Coloque aqui os links para a documentação do projeto e os repositórios e plubicação do backend e frontend.*)
-   [Documentação (esse documento)](github.com/marcoandre/pi-modelo)
-   Backend: [Repositório](https://github.com/Atelier-A-Y/Backend-Atelier.git) e [Publicação](https://backend-atelier-a-y.class.fabricadesoftware.ifc.edu.br/admin/login/?next=/admin/)
-   Frontend: [Repositório](https://github.com/Atelier-A-Y/FrontEnd.git) e [Publicação](https://paginahome-mu.vercel.app/)
   
# 1. Desenvolvimento 

**1.1. Ponto de Vendas (PDV)**

Optamos pelo modelo de Pontos de Vendas (PDV) para o nosso site por ser planejado para uma loja de roupas. Nosso sistema precisa permitir que os clientes adicionem os produtos no carrinho de compras, favoritem produtos que desejem adquirir, cadastrem suas informações (endereço, nome, email…), escolham a categoria de roupas que vão olhar e acompanhem em tempo real o status da entrega dos seus pedidos. Para os adm os pedidos serão cadastrados: Os que foram feitos, os que estão em entrega e os que foram entregues.


# 2. Situação Problema

 Atelier - A.Y.é uma loja de roupas de pequeno porte, composta por seis funcionários e administrada por quatro responsáveis. A loja local é pequena e funciona de segunda a sexta-feira, das oito horas da manhã às quatro horas tarde, com intervalo para almoço das 12h às 13h.
Ao final de cada dia a equipe faz  a conferência do caixa, a análise das vendas realizadas durante o dia, a verificação das peças mais vendidas e a conferência de possíveis faltas no estoque, além da organização e reposição das mercadorias.
No final do mês é necessário realizar o cálculo do lucro. Atualmente, esse processo é feito por meio de anotações manuais, registradas à mão ao longo dos dias. Esse método torna a tarefa ainda mais complicada pois não há um sistema digital que auxilie na organização das informações. 
Além disso, por atuar apenas de forma local e não possuir presença digital significativa, a loja ainda apresenta um alcance limitado de público. Dessa forma, torna-se importante pensar em estratégias e ferramentas que possam auxiliar na organização das vendas e ampliar a visibilidade do negócio.

# 3. Descrição da proposta

O software terá como foco principal a venda de roupas online, além da administração de vendas e controle de estoque. Para os usuários comuns, o sistema permitirá visualizar as roupas disponíveis, realizar cadastro e login, favoritar produtos, efetuar compras e acompanhar o status de entrega dos pedidos. Já para os administradores, haverá uma área exclusiva onde será possível visualizar o total de vendas diárias e mensais, controlar a quantidade de produtos em estoque e gerenciar pedidos de reposição de roupas.

De forma geral, o software permitirá o cadastro e autenticação de usuários, o armazenamento e gerenciamento de produtos, a criação de listas de favoritos, a realização de compras, o acompanhamento do status de entrega, além do controle de estoque, geração de relatórios de vendas e gestão de pedidos.

# 4. Modelagem de Dados

![Diagrama de Caso de Uso](img/dcu_modelagem.png "Diagrama de Caso de Uso")

# 4. Regras de negócio
- RN001.01 - Dados : Tamanho, cor, nome, preço, descrição, continente.
- RN002.01 - Dados : Nome, senha, cpf, email, telefone.
- RN005.01 - Dados : Nome, id.
- RN006.01 - Dados : Preço, data-venda, id cliente, tipo pagamento.
- RN006.02 - Configuração disponível somente para admin.
- RN007.01 - Dados : Nome, preço, endereço, tipo-pagamento.
- RN008.01 - Dados : Id roupa, Categoria, quantidade.
- RN009.01 - Dados : Localização, data-entrega.
- RN010.01 -  Dados : Vendas. 
- RN010.02 -  Configuração disponível somente para admin. 
- RN011.01 - Dados : Nome, id.

# 5. Requisitos funcionais
- RF001 - O sistema deve manter roupas 
- RF002 -  O sistema deve manter usuário 
- RF003 - O sistema deve permitir adicionar roupas e visualizar no carrinho de compra 
- RF004 -  O sistema deve permitir adicionar roupas e visualizar no  favoritos
- RF005 - O sistema deve manter Categoria
- RF006 - O sistema deve manter vendas
- RF007 - O sistema deve manter compras
- RF008 - O sistema deve manter estoque
- RF009 - O sistema deve manter status de entrega dos pedidos
- RF010 - O sistema deve manter relatórios de vendas
- RF011 - O sistema deve manter continentes 

# 6. Requisitos não funcionais
- RNF001 - O sistema deve possuir uma interface intuitiva e fácil uso
- RNF002 - O sistema deve ser responsivo
- RNF003 - O sistema deve apresentar feedback visual para ações do usuário (ex: confirmação de compra)
- RNF004 - O sistema deve ser desenvolvido de forma modular (separação entre Vue.js e Django)
- RNF005 - O sistema deve garantir autenticação segura de usuários (login com criptografia de senha)
- RNF006 - O sistema deve restringir o acesso às funcionalidades administrativas apenas a usuários autorizados
- RNF007 - O Frontend deve ser desenvolvido utilizando vue.js 
- RNF008 - O backend deve ser desenvolvido em django

  # FIZ ATÉ AQUI

# 7. Diagrama de Caso de Uso

**7.1 Introdução**

O diagrama de caso de uso é uma ferramenta de modelagem que descreve o comportamento de um sistema a partir da perspectiva do usuário. Ele é usado para capturar os requisitos funcionais de um sistema.

- Especificam a visão externa do sistema.
- Descrevem como o sistema é percebido por seus usuários.
- Descrevem as interações entre os usuários e o sistema.

![Diagrama de Caso de Uso](img/dcu1.png "Diagrama de Caso de Uso")

**Os casos de uso:**
- Descrevem como os **usuários interagem com o sistema** (as funcionalidades do sistema)
- Facilitam a **organização dos requisitos** de um sistema.
- Dão uma **visão externa** do sistema
- O conjunto de casos de uso deve ser capaz de comunicar a **funcionalidade** e o **comportamento** do sistema para o cliente.
- Descrevem **o que** o sistema faz, mas **não** especificam **como** isso deve ser feito.

**7.2 Elementos do diagrama de caso de uso**

7.2.1 **Atores**

- Representam os papéis desempenhados por **elementos externos** ao sistema
  - Ex: humano (usuário), dispositivo de hardware ou outro sistema (cliente)
- Elementos que **interagem** com o sistema

Notação:

![Atores Notação](img/dcu_atores_notacao.png "Atores Notação")

**Exemplo: Loja de CDs**

**Identificando os atores**
- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja.
- A loja possui um **atendente** cuja função é atender os clientes durante a venda dos discos. A loja também possui um **gerente** cuja função é administrar o estoque para que não faltem discos. Além disso é ele quem dá folga ao atendente, ou seja, ele também atende os clientes durante a venda dos discos.

![Identificando os atores](img/dcu_identificando_atores.png "Identificando os atores")

**E o cliente?**
- Não é ator pois ele **não interage** com o sistema!

**7.2.2 Casos de uso**

- Representam **funcionalidades** do sistema (requisitos funcionais).
- São iniciados por **atores** ou por outros casos de uso.

> **Dica**: nomeie os casos de uso com **verbos** no **infinitivo**.

Notação:

![Casos de uso Notação](img/dcu_casos_de_uso_notacao.png "Casos de uso Notação")

**Exemplo: Loja de CDs**

**Identificando os casos de uso**

- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja. A loja possui um atendente cuja função é atender os clientes durante a **venda dos discos**.
- A loja também possui um gerente cuja função é **administrar o estoque** para que não faltem discos. Além disso é ele quem dá folga ao atendente, ou seja, ele também atende os clientes durante a **venda dos discos**.

![Identificando os casos de uso](img/dcu_identificando_casos_de_uso.png "Identificando os casos de uso")

**7.2.3 Relacionamentos**

**7.2.3.1 Relacionamento de associação**

- Indica que um ator **participa** de um caso de uso, ou seja, o ator **interage** (comunica-se) com o caso de uso.
- É representado por uma **linha sólida**.
- Um ator pode se relacionar com **um ou mais casos de uso**.

> Dicas:
> - Não use setas nas linhas de associação.
> - Associações não representam fluxo de informação.

![Relacionamento de associação](img/dcu_relacionamento_de_associacao.png "Relacionamento de associação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de associação**

- Uma loja de CDs possui discos para venda. Um cliente pode comprar uma quantidade ilimitada de discos para isto ele deve se dirigir à loja. A loja possui um _atendente_ cuja função é atender os clientes durante a **venda dos discos**.
- A loja também possui um _gerente_ cuja função é **administrar o estoque** para que não faltem discos. Além disso é ele quem dá folga ao _atendente_, ou seja, ele também atende os clientes durante a **venda dos discos**.

![Identificando os relacionamentos de associação](img/dcu_identificando_relacionamentos_de_associacao.png "Identificando os relacionamentos de associação")

**7.2.3.2 Relacionamento de generalização/especialização**

**Generalização de atores**

- Quando dois ou mais atores podem se **comunicar com o mesmo conjunto de casos de uso**.
- Indica que um ator **herda** as características de outro ator.
– Um filho (herdeiro) pode se comunicar com todos os casos de uso que seu pai se comunica.

> **Dica:** coloque os herdeiros **embaixo**.

**Notação:**

![Relacionamento de generalização/especialização de atores - notação](img/dcu_relacionamento_de_generalizacao_especializacao_notacao_de_atores.png "Relacionamento de generalização/especialização de atores - notação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de generalização/especialização de atores**

![Identificando os relacionamentos de generalização/especialização de atores](img/dcu_identificando_relacionamentos_de_generalizacao_especializacao_de_atores.png "Identificando os relacionamentos de generalização/especialização de atores")

**Generalização de casos de uso**

– O caso de uso filho herda o comportamento e o significado do caso de uso pai.
– O caso de uso filho pode incluir ou sobrescrever o comportamento do caso de uso pai.
– O caso de uso filho pode substituir o caso de uso pai em qualquer lugar que ele apareça.

> **Dica:** deve ser aplicada quando uma condição resulta na definição de
diversos fluxos alternativos.

Notação:

![Relacionamento de generalização/especialização de casos de uso - notação](img/dcu_relacionamento_de_generalizacao_especializacao_notacao_de_casos_de_uso.png "Relacionamento de generalização/especialização de casos de uso - notação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de generalização/especialização de casos de uso**

**Novos requisitos:**

- As vendas podem ser **à vista** ou **a prazo**. Em ambos os casos o estoque é
atualizado e uma nota fiscal, entregue ao consumidor.
- No caso de uma **venda à vista**, clientes cadastrados na loja e que compram mais de 5 CDs de uma só vez ganham um desconto de 1% para cada ano de cadastro.
- No caso de uma **venda a prazo**, ela pode ser parcelada em 2 pagamentos com um
acréscimo de 20%. As vendas a prazo podem ser pagas no **cartão** ou no **boleto**.
  - Para pagamento com **boleto**, são gerados boletos bancários que são entregues ao cliente e armazenados no sistema para lançamento posterior no caixa.
  - Para pagamento com **cartão**, os clientes com mais de 10 anos de cadastro na loja ganham o mesmo desconto das compras à vista.

![Identificando os relacionamentos de generalização/especialização de casos de uso](img/dcu_identificando_relacionamentos_de_generalizacao_especializacao_de_casos_de_uso.png "Identificando os relacionamentos de generalização/especialização de casos de uso")

**Identificando mais relacionamentos de generalização/especialização de casos de uso**

![Identificando mais relacionamentos de generalização/especialização de casos de uso](img/dcu_identificando_mais_relacionamentos_de_generalizacao_especializacao_de_casos_de_uso.png "Identificando mais relacionamentos de generalização/especialização de casos de uso")

**7.2.3.3 Relacionamento de dependência**

**Extensão**

- Representa uma variação/extensão do comportamento do caso de uso base.
- O caso de uso estendido só é executado sob certas circunstâncias.
- Separa partes obrigatórias de partes opcionais.
  - Partes obrigatórias: caso de uso base.
  - Partes opcionais: caso de uso estendido.
- Fatorar comportamentos variantes do sistema (podendo reusar este comportamento
em outros casos de uso).

**Notação:**

![Relacionamento de dependência (extensão) - notação](img/dcu_relacionamento_de_dependencia_extensao_notacao.png "Relacionamento de dependência (extensão) - notação")

**Exemplo: Loja de CDs**

**Identificando os relacionamentos de dependência (extensão)**

**Novos requisitos:**
- No caso de uma venda à vista, clientes cadastrados na loja e que compram mais
de 5 CDs de uma só vez ganham um **desconto** de 1% para cada ano de cadastro.
- No caso de uma venda a prazo...
  - ...Para pagamento com cartão, os clientes com mais de 10 anos de cadastro na loja ganham o mesmo **desconto** das compras à vista.

![Identificando os relacionamentos de dependência (extensão)](img/dcu_identificando_relacionamentos_de_dependencia_extensao.png "Identificando os relacionamentos de dependência (extensão)")

**Inclusão**

- Evita repetição ao fatorar uma atividade
comum a dois ou mais casos de uso.
- Um caso de uso pode incluir vários casos de uso.

**Notação:**

![Relacionamento de dependência (inclusão) - notação](img/dcu_relacionamento_de_dependencia_inclusao_notacao.png "Relacionamento de dependência (inclusão) - notação")

**Exemplo: Loja de CDs**

**Novos requisitos:**
Para efetuar vendas ou administrar estoque, atendentes e gerentes terão que **validar** suas respectivas senhas de
acesso ao sistema.

![Identificando os relacionamentos de dependência (inclusão)](img/dcu_identificando_relacionamentos_de_dependencia_inclusao.png "Identificando os relacionamentos de dependência (inclusão)")

**7.2.4 Fronteira do sistema**

- Elemento opcional (mas essencial para um bom
entendimento).
- Serve para definir a área de atuação do sistema, ou seja, seus limites.

**Identificando a fronteira do sistema**

![Identificando a fronteira do sistema](img/dcu_identificando_a_fronteira_do_sistema.png "Identificando a fronteira do sistema")

---



