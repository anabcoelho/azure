# Security Services

Network Security Group

- Filtragem do tráfego entre recursos
- Entre subredes
- Firewall interno
- Regras podem ser criadas por especificações de:
    - Protocolo
    - Fonte / destino (ip, tags, application security groups)
    - Portas
    - Direção (inbound, outbound)
    - Prioridade

Application Security Group

- Agrupa servidores de forma lógica com características comuns, permitindo que as regras se segurança funcione de forma agrupada
- Reduz esforço de manutenção
- Evita o uso de IPs explícitos

User defined Routing

- Redirecionamento de conexões
- Selecionar um caminho de tráfego em uma ou entre múltiplas redes

Proteção contra DDoS

- Proteção contra a tentativa de sobrecarregar e esgotar os recursos
- Bloqueio do tráfego adicional
- Basic: automaticamente habilitada de modo gratuito em todos os recursos azure
- Standard: possui valor adicional, com recursos adicionais como Machine Learning p/ monitorar padrões de acessos.
- O mesmo plano protege todos os serviços

Firewall

PaaS

- Monitora e controla tráfego in/out
- Políticas de segurança
- Escalável e com alta disponibilidade
- Bloqueio / aceite de IPs

Azure Sentinel

- Detecção e resposta a ameaças
- Sistema de gerenciamento de evento e informações de segurança
- Agrega informações de on-prem, outras clouds e Azure
- Responde a incidentes
- Investiga ameaças

![Untitled](Security%20Services%206708ed4f10264255abf5c87f006d6071/Untitled.png)

![Untitled](Security%20Services%206708ed4f10264255abf5c87f006d6071/Untitled%201.png)

Host dedicado Azure

- Único cliente (assinatura) usando um computador físico
- Pago por Host
- Controle sobre Infra
- Não pode compartilhar o mesmo host entre assinaturas

Azure Security Center

PaaS

- Gerenciamento de segurança
- Visibilidade da postura de segurança em todos os serviços, tanto em nuvem quanto local
- Nativamente embutido
- Gratuito (sem defender)
- **Resource Security Hygiene:** Saúde dos recursos por uma perspectiva de segurança
- **Respond to security alerts:** visão centralizada de todos os alertas de segurança

- **Postura de Segurança:** Habilidade da organização sobre controles e políticas de cybersegurança bem como consegue prever, previnir e responder a ameaças de segurança.
- **Secure Score:** medida da postura de segurança,  baseado na porcentagem de controles de segurança que você satisfaz.
- Defender for Cloud: Paga pelo que habilita; segurança híbrida, scan de vulnerabilidade

- **Proteção contra ameaças:** Proteção avançada para VMs, segurança de rede e integridade de arquivos na nuvem.
    - Just in time acess: Bloqueia tráfego por padrão para portas de redes específicas das VMs, mas permite tráfego por um período de tempo quando um adm solicita.
    - Adaptative application controls: Quais aplicações podem rodar nas VMs
    - File integrity monitoring: detecta alterações em arquivos

Key Vault

PaaS

- Armazenamento seguro de chaves e certificados
- Centralizado, monitorado e nativo em muitos serviços azure

Defesa em camadas

![Untitled](Security%20Services%206708ed4f10264255abf5c87f006d6071/Untitled%202.png)

- Segurança Física: proteção de acesso aos hardwares
- Identidade e acesso
- Perímetro: proteção de ataques de rede
- Network: limita comunicação entre recursos
- Computação: segurança dos recursos
- Application: Apps seguros e livres de vulnerabilidade
- Dados: controla acesso aos dados
- PIPnCAD

Azure Information Protection

- Classificação e rotulagem de documentos e emails

![Untitled](Security%20Services%206708ed4f10264255abf5c87f006d6071/Untitled%203.png)