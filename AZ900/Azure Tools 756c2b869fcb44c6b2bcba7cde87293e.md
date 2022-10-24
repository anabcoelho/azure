# Azure Tools

Portal Azure

- Interface baseada em web, acessada via browser
- Self-service
- Ideal para tarefas simples

App Móvel do Azure 

- monitora integridade e o status de seus recursos do Azure
- Verificar se há alertas, diagnosticar e corrigir problemas rapidamente e reiniciar app web ou vm.

Azure PowerShell 

- Command-lets
- Uso de terminal, que funciona no linux, windows, macOS
- Baseado em PowerShell
- Automatizar tarefas, de forma mais simples
- Código imperativo: detalha cada etapa individual que deve ser executada para alcançar um resultado desejado
- Uso da API rest para executar toda tarefa de gerenciamento azure
- Comandos:
    - Connect - AzAccount-login,
    - Get - AzResourceGroup,
    - New - AzResourceGroup,
    - New - AzVm

Azure CLI 

- Familiaridade com Linux
- Baseado em python
- Comandos
    - az login
    - az grouplist
    - az groupcreate
    - az vmcreate

Azure CloudShell

- Acesso via navegador, Portal Azure ou App Mobile
- Ambiente atualizado onde módulos e ferramentas já estão pré-instaladas
- Pode utilizar CLI, PowerShell
- Expira com 20min de inatividade