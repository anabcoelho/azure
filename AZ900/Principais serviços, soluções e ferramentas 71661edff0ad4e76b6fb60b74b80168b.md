# Principais serviços, soluções e ferramentas

Azure Marketplace: Apps e serviços de centenas de provedores.

- Computação
    
    Virtual machines
    
    - IaaS
    - Emula computadores físicos, que incluem um processador virtual, memória, armazenamento e recursos de rede
    - controle total sobre o sistema operacional
    - VM scale sets: Usado pra implementar um conjunto de VMs idênticas com suporte a escalabilidade (manual, automática ou ambos) (apenas linux e Windows)
    - Spot VM: VMs com desconto, para vida curta
    - VM reservada: pagamento antecipado para um período longo
    - Azure Batch: Escala muitas VMs p/ computação de alta performance (HPC) e jobs paralelos em larga escala
    - HyperV: mais potente
    - When an Azure virtual machine is stopped, you don't pay for the virtual machine. However, you do still pay for the storage costs associated to the virtual machine.
    
    Container
    
    - Ambiente de virtualização
    - Não gerencia o Sistema Operacional
    - Projetados para serem criados, dimensionados e interrompidos dinamicamente
    - Não é altamente escalável
    
    Kubernetes
    
    - Orquestração de containeres open-source, feito para rodar praticamente qualquer coisa, altamente escalável e customizável.
    
    Functions
    
    - Execução de um código
    - Pago pelo tempo que o código é executado
    - Não mantém estado por padrão
    
    Logic apps
    
    - Orquestra tasks, workflows
    - Executados somente em nuvem
    - Drag and Drop - executa workflows
    - Gatilho e fluxos de trabalho
    
    Serviço de app
    
    - PaaS
    - Construir, implantar e escalar rapidamente aplicativos de nível empresarial, sendo web, móveis e API, executados em qualquer plataforma
    - Alcança rigorosa performance, escalabilidade, segurança e requerimentos de conformidade
    
    Free = 1 GB 
    
    Shared = 1 GB
    
     Basic = 10 GB 
    
    Standard = 50 GB 
    
    Premium = 250 GB 
    
    Isolated = 1 TB
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled.png)
    
    Área de trabalho virtual Azure
    
    - Serviço de virtualização de área de trabalho e aplicativos que é executado na nuvem, que permite que os usuários usem uma versão do windows hospedada na nuvem em qualquer localização
    - Funciona em Windows, IoS, Mac, android, linux
    - Gerenciamento simplificado:
    - Usuários devem existir no AD
    - Free no MS 365
    
    Event grid
    
    - Recebe e encaminha mensagens baseadas em eventos
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%201.png)
    
- Rede
    
    Azure Virtual Network
    
    - Permite que recursos do Azure comuniquem-se uns com os outros, com usuários na internet e com computadores locais.
    - Além de comunicação as Vnets podem isolar e segmentar, rotear e filtrar o trafego de rede
    - pode ser seccionada em subredes, melhor para gerenciar a localização de IP, além de agrupar recursos relacionados
    - Pertence a apenas uma região
    - Vnet Peering: 2 ou mais Vnets se comportando como se fosse uma. (conectando vnets em regiões e permitindo transferência de dados entre locatários)
    - Ponto de extremidade privado: usa IP privado da Vnet e se comunica com serviços
    - 
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%202.png)
    
    Express route
    
    - Estende redes locais p/ azure por conexão privada que é facilitada por um provedor de conectividade
    
    Azure Load Balancer 
    
    - Responsável por distribuir tráfego non-web igualmente entre recursos
    
    Application Gateway
    
    - Distribui tráfego web (e non-web, para múltiplos tiers)
    - Ferramentas de firewall, URL routing ou ssl termination
    
    Gateway de VPN 
    
    - Dados criptografados em tunel privado à medida que atravessam a internet
    - Pode ser baseado em política (ip específico) ou em rota.
    - Site a site: datacenter local p/ azure
    - Point to site: dispositivo individual p/ azure
    - rede a rede: vnet p/ vnet
    - A Local Network Gateway is an object in Azure that represents your on-premise VPN device. A Virtual Network Gateway is the VPN object at the Azure end of the VPN. A 'connection' is what connects the Local Network Gateway and the Virtual Network Gateway to bring up the VPN. The **local network** gateway typically refers to your **on-premises location**. You give the site a name by which Azure can refer to it, then specify the IP address of the on-premises VPN device to which you will create a connection. You also specify the IP address prefixes that will be routed through the VPN gateway to the VPN device.
    
    Content delivery network 
    
    - entrega rápida de conteúdos.
    - Economize largura de banda e melhore a capacidade de resposta na codificação e distribuição de softwares de jogos, atualizações de firmware e pontos de extremidade IoT. Reduza o tempo de carregamento de sites, aplicativos móveis e mídia de streaming para aumentar a satisfação do usuário globalmente.
    - ideal para dados que não mudam com frequência
    
    DNS do Azure
    
    - **hospedagem para domínios DNS**
    - Ao hospedar seus domínios no Azure, você pode gerenciar seus registros DNS usando as mesmas credenciais, APIs, ferramentas e faturamento que os outros serviços do Azure.
    - não é possível comprar um nome de domínio (pode usar o serviço de app para isso, além de sites de venda de dominios)
- Armazenamento
    
    Storage Account (IaaS)
    
    - Grupos de serviços menores
    - Serviço altamente escalável e durável
    - Armazenamento de grande quantidade de dados por preços baixíssimos
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%203.png)
    
    - Blob Storage
        - Armazenados em containeres (pastas)
        - Ideal para dados não estruturados
        - Acesso em qualquer lugar via internet
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%204.png)
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%205.png)
        
    - File Storage
        - Shares (pastas) e files
        - Acesso via protocolo SMB (server message block) e network file system
        - ideal p/ migração de onprem e manter estado de uma aplicação
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%206.png)
        
    
    - Queue Storage
        - entrega de mensagens em filas
        - utilizado pra casos específicos (em pequenas partes de dados sequenciais)
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%207.png)
        
    - Table Storage
        - Modelo chave/valor, dados semiestruturados
        - Acesso rápido e possui diversas interfaces
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%208.png)
        
    - Disk Storage
        - Emulação de discos na nuvem, permitindo que os clientes anexem discos persistentes às VM tanto para o sistema operacional como para dados de apps
        - HD e SSD
        - Diferentes tamanhos
        - Managed - Cliente responsável
        - Unmanaged - provedor responsável
- Database
    
    Azure SQL Database
    
    - PaaS
    - Versão + recente e estável do SQL server
    - Datasets estruturados
    - Migração facil do on-prem
    
    Azure SQL Managed Instance
    
    - todos os recursos do SQL server, porém mais caro
    - PaaS
    - Migração facil do on-prem
    - Melhor opção para migração de on prem p/ cloud
    
    SQL em VM
    
    - Controle do S.O.
    - IaaS
    - recursos interessantes como segurança, backup, monitoramento, replicação e atualização automática do S.O.
    
     
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%209.png)
    
    Database for MySQL 
    
    - Usa mySQL community edition
    - Banco relacional
    - Alta disponibilidade e segurança
    - Desempenho previsível, totalmente gerenciável
    
    Postgre SQL 
    
    - PaaS
    - Baseado no mecanismo de banco de dados postgres
    - Banco de dados relacional
    - Criptografia de dados em disco e ssl
    - Servidor único:
        
        ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%2010.png)
        
    - Hiperescala: ideal pra bigdata (+1tb), escala horizontal de consultas e análise em tempo real
    
    Cosmos DB
    
    - Não relacional
    - Totalmente gerenciado e sem servidor
    - Globalmente distribuido
    - Os dados são então abstraídos e projetados como uma API que é especificada ao criar o banco de dados - Pode escolher API que mais satisfaz
    - Fácil de migrar do table storage
    
    ![Untitled](Principais%20servic%CC%A7os,%20soluc%CC%A7o%CC%83es%20e%20ferramentas%2071661edff0ad4e76b6fb60b74b80168b/Untitled%2011.png)
    
- Big Data
    
    Azure Synapse Analytics
    
    - PaaS
    - Plataforma de big data e analytics que permite os usuários a fazer análise e transformação de dados com datasets muito grandes
    - Workspace p/ werehousing e análise de ponta a ponta com diversas ferramentas integradas
    - Spark embutido
    - Synapse Studio: gerencia as ferramentas e fazer toda a transformação dos dados em um único lugar
    - Synapse SQL: Clusters de banco de dados massivo de processamento paralelo baseado em SQL
    - Azure DataFactory: Ferramenta que permite aos desenvolvedores injetar e transformar seus dados usando workflows visuais.
    
    Azure HDInsights
    
    - PaaS flexível de multipropósito
    - Big data Open Source
    - Ampla gama de cenários
    - Cluster gerenciado pela Microsoft
    
    Databricks
    
    - Ambiente spark
    - PaaS
    - Suporte a Python, Scala, R, Java e SQL
    
    Datalake analytics:
    
    - Análise sob demanda
    - ETL
- IoT
    
    Azure IoT hub (PaaS)
    
    - Plataforma para desenvolvimento de soluções
    - Conexão bidirecional entre a nuvem e os dispositivos IoT
    - Integração com serviços azure e diversas linguagens de programação
    - Suporte a muitos protocolos de comunicação (HTTP, AMQP, MQTT)
    - IoT edge: Permite que os modelos de análise de dados sejam enviados por push diretamente a dispositivos IoT, possibilitando a reação desses dispositivos sem necessidade de consultar modelos de IA baseados em nuvem
    
    Azure IoT central (SaaS) 
    
    - Templates para construir modelos personalizados c/ interface
    - Segura, escalável e confiável
    
     Azure Sphere
    
    - Não é um serviço em si
    - Set de componentes que permitem a criação de apps de IoT seguras e de ponta a ponta
    - Do hardware, sistema operacional, segurança a um método seguro de envio de mensagens
- AI
    
    Azure Machine Learning
    
    - Recursos para construir e testar um modelo de ML
    - Drag and Drop
    
    Serviços Cognitivos
    
    - ML pré criados que permitem ver, ouvir, falar, entender e até mesmo raciocinar
    - Personalizer: ‘Observa’ as ações de usuários em uma aplicação e utiliza essas infos p/ prever suas ações e oferecer experiências relevantes.
    
     
    
    Azure bot service
    
    - Criação de agente virtual (IA) p/ interagir com humanos via linguagem natural
- DevOps
    - Conjuntos de práticas de desenvolvimento e operações
    
    Azure DevOps
    
    - + 1000 serviços
    - Boards: rastreio de progresso via quadros / kanban
    - Repos: repositório e versionamento via git
    - Pipelines:  compila e testa automaticamente seus projetos de código. Combina a CI (integração contínua) e a CD (entrega contínua) para testar e compilar seu código e enviá-lo para qualquer destino.
    - Artifact: os desenvolvedores podem criar, hospedar e publicar pacotes em seus feeds e compartilhá-los na mesma equipe, entre organizações e até publicamente.
    - Test plans: uso de testes de código, garantindo a qualidade antes da liberação.
    
    Github e Github actions
    
    - Repositório de códigos e gerenciador de versões
    - Actions se assemelha a pipelines
    
    Azure DevTest Labs
    
    - Ambientes (que estão disponíveis no ARM) rapidamente provisionados, feitos para teste e exclusão rápida
    - grande número de máquinas virtuais personalizadas semanalmente