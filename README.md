
# EventWave

O EventWave é uma aplicação de gerenciamento de eventos e ingressos, que utiliza a tecnologia de microserviços para fornecer um ambiente escalável e seguro para a gestão de eventos.

A aplicação é construída com o uso de diferentes tecnologias, incluindo Flyway, MongoDB e Postgres para o gerenciamento de dados, Kafka para a comunicação entre microserviços, Border Gateway para garantir o acesso seguro aos serviços e Discovery para garantir que cada serviço possa ser descoberto e acessado pelos demais serviços de forma segura e escalável.

## Microserviços

A aplicação EventWave é composta por diferentes microserviços, cada um com sua própria responsabilidade e funcionalidade:

* Serviço de autenticação
* Serviço de gerenciamento de eventos
* Serviço de gerenciamento de ingressos
* Serviço de gerenciamento de reservas
* Serviço de processamento de pagamentos
* Serviço de notificação
* Serviço de análise de vendas

Cada microserviço é implantado em um contêiner Docker, o que facilita o gerenciamento e a implantação em diferentes ambientes. Os contêineres podem ser facilmente escalados horizontalmente de acordo com a demanda.
## Tabelas e collections
Abaixo estão algumas das tabelas e coleções utilizadas pela aplicação EventWave, juntamente com seus relacionamentos:

**Usuários:** tabela para armazenar informações dos usuários que acessam a aplicação, incluindo nome, endereço de e-mail, senha criptografada, data de criação e atualização.

**Eventos:** coleção para armazenar informações dos eventos cadastrados na plataforma, incluindo nome, descrição, localização, data, hora, capacidade, imagem, categoria e detalhes adicionais do evento.

**Ingressos:** tabela para armazenar informações dos ingressos disponíveis para venda em cada evento, incluindo o evento ao qual ele pertence, o nome, o preço, a quantidade disponível e as datas de criação e atualização.

**Reservas:** tabela para armazenar informações das reservas de ingressos feitas pelos usuários, incluindo o usuário que fez a reserva, o ingresso reservado, a quantidade, o status (pendente, confirmado ou cancelado) e as datas de criação e atualização.

Além dessas tabelas e coleções, a aplicação EventWave também utiliza outras tabelas e coleções para armazenar informações adicionais sobre os usuários, eventos e reservas.
## Utilização do Docker
Para implantar e executar a aplicação EventWave, é necessário configurar e iniciar cada microserviço individualmente, garantindo que todos estejam se comunicando corretamente. Cada microserviço possui sua própria configuração e conjunto de dependências, que devem ser gerenciados separadamente.

Para facilitar o gerenciamento e a implantação em diferentes ambientes, cada microserviço é implantado em um cont
