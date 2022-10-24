# Principais Conceitos Azure

Vantagens de uso de Cloud

- Alta disponibilidade
- Escalabilidade fácil (vertical: + computação, horizontal: + recursos)
- Elasticidade (dimensionamento automático)
- Alcance global
- Recuperação de desastre (backup, replicação de dados e distribuição geográfica)
- Custo preditivo
- Agilidade (implementação e configuração rápida)
- Segurança
- Economia de escala (reduz custos e aumenta eficiência)

Despesas de Capital

CapEx:

- Investimento enorme inicial e pequenos posteriores
- comprar a própria infraestrutura
- Custo de manutenção total

OpEx:

- Aluguel de infraestrutura
- Pay per use (baseado em consumo)
- Manutenção sem gastos adicionais

Diferentes modelos de Nuvem

Public Cloud

- Contrata-se provedor
- Acessada via internet
- OpEx
- Pay as you go
- Sem necessidade de manutenção de hardware
- Nenhuma habilidade técnica aprofundada necessária

Hybrid Cloud 

- Mistura da pública com a privada
- + flexível
- Dados e apps compartilhados entre elas
- Alta flexibilidade
- + caro
- + complicado de administrar
- You could start with a public cloud and then combine that with an on-premise infrastructure to implement a hybrid cloud.
- You can extend a private cloud by deploying virtual servers in a public cloud.

Private Cloud  

- Próprio datacenter
- Hardware mantido pelo cliente
- Grande CapEx
- Baixa agilidade
- Habilidade e expertise mandatória
- infra em rede privada
- Único locatário

IaaS, PaaS, SaaS

![Untitled](Principais%20Conceitos%20Azure%207406dc37227e46b6bf6d3c988bbb6ffa/Untitled.png)

IaaS

![Untitled](Principais%20Conceitos%20Azure%207406dc37227e46b6bf6d3c988bbb6ffa/Untitled%201.png)

Infraestrutura física

Datacenter

- Instalações físicas que armazenam servidores interligados por rede
- Onde é rodado serviços que o provedor disponibiliza

Availability set

- update domains
- Separação física
- Mantêm aplicações online caso haja falha de hardwares
- SLA: 99,95%

Availability Zone 

- Conexão por fibra optica privada
- Datacenters fisicamente separados
- SLA: 99,99%
- Energia / resfriamento independentes
- Azure data center failure

![Untitled](Principais%20Conceitos%20Azure%207406dc37227e46b6bf6d3c988bbb6ffa/Untitled%202.png)

Geography > Regions > Zones > Datacenters > Availbility Sets

Regiões 

- Áreas geográficas no planeta compostas por um ou mais datacenters fisicamente separados porém conectados por rede de internet de baixa latência
- Nem todo serviço ou feature está disponível em todas as regiões
- SLA independe da região
- Regiões especiais: Regiões governamentais EUA e [21Vianet](https://en.wikipedia.org/wiki/21Vianet) China , onde a Microsoft providencia os serviços mas não mantém nem administra as regiões diretamente

Pares de regiões:

- Cada região possui um par conectada a ela com distância física de 483 km, para cobrir desastres naturais

Geografias

- Teórica
- 2 ou + regiões onde seu propósito é garantir que todos os níveis de requerimentos sejam preservados
- Cada região contem uma única geografia

![Untitled](Principais%20Conceitos%20Azure%207406dc37227e46b6bf6d3c988bbb6ffa/Untitled%203.png)

Níveis de gerenciamento

Azure Resource Manager

- Camada de gerenciamento centralizado que governa todos recursos e grupos de recursos azure
- O responsável por criar cada serviço Azure
- Controla o acesso e administração de recursos
- Independente do meio utilizado para compra de serviços, todas interfaces se conectam no ARM
- Checa privilégios antes de criar, modificar ou deletar recursos.
- ARM model (Json) permite a criação de grupos de recursos
- Cria recursos de forma consistente

Conta do Azure

- Endereço de email que fornece ao criar uma assinatura Azure
- Você pode usar a mesma conta do azure para várias assinaturas, que servem como diferentes modelos de cobrança e que pode aplicar diferentes políticas de acesso.

Administrador da conta

- Parte associada ao email usado para criar uma assinatura.
- Responsável por pagar todos os custos que incorrem pelos recursos da assinatura

Grupos de gerenciamento

- Ajuda a gerenciar o acesso, a política e a conformidade de várias assinaturas
- Todas as assinaturas em um grupo herdam automaticamente as condições aplicadas ao grupo de gerenciamento
- Possui até 6 camadas

![Untitled](Principais%20Conceitos%20Azure%207406dc37227e46b6bf6d3c988bbb6ffa/Untitled%204.png)

Subscription 

- Unidade lógica dos serviços: associa as contas de usuário e os recursos que elas criam.
- Fornece acesso autenticado e autorizado à recursos e serviços
- Cada recurso é associado a apenas 1 assinatura
- Limite de faturamento
- Limite de controle de acesso
- Pode separar: ambientes de testes, estruturas organizacionais e billing.
- Sempre terá um locatário

Grupo de recurso

- Agrupamento de recursos
- Nenhum recurso pode ser criado sem um grupo de recurso
- É possível mudar o recurso de grupo
- Agrupamento de forma logica
- administra recursos
- Localização indicada ao criar serve apenas para metadados
- Não é possível ter hierarquia

Suporte Azure

Basic

- Free
- Sem suporte técnico

Developer

- p/ ambientes de teste e não produção
- suporte via email em horário comercial
- $29

Standard

- p/ ambientes de carga de trabalho de produção
- 24/7 por email e telefone
- $100

Profissional

- p/ dependência crítica
- 24/7 email e telefone
- $1000

Premier

- + completa
- Consultoria de ajuda personalizada
- partir de 1º de julho de 2022, a Microsoft não oferecerá mais contratos de suporte Premier para clientes em renovação.

**Balanceamento de carga:** é a prática de distribuir **cargas**  de trabalho computacionais entre dois ou mais computadores