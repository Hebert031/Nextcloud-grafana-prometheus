# Nextcloud + grafana + prometheus
## Playbook do Ansible para Configuração do Ambiente Nextcloud
Este playbook do Ansible automatiza a configuração do ambiente Nextcloud, bem como a instalação e configuração do Grafana e Prometheus para monitoramento adicional.

O playbook inclui as seguintes tarefas:

    Criação de diretórios e configuração do ambiente Nextcloud.
    Cópia de arquivos de configuração necessários para o Nextcloud, Grafana e Prometheus.
    Instalação do Docker e Docker Compose para gerenciar os contêineres.
    Configuração e implantação do Grafana para visualização dos dados de monitoramento.
    Implantação do Prometheus para coletar e armazenar métricas do ambiente.

Essa solução permite configurar facilmente um ambiente completo para o Nextcloud, além de fornecer as ferramentas de monitoramento Grafana e Prometheus para acompanhar o desempenho e a saúde do sistema.
### Pré-requisitos

Certifique-se de ter o Ansible instalado no sistema antes de executar este playbook.

### Como Usar

1. Clone o repositório do GitHub: `git@github.com:Hebert031/Nextcloud-grafana-prometheus.git`
2. Acesse o diretório do projeto:
3. Abra o arquivo `hosts` e defina o endereço do host alvo sob o grupo `[cloud01-hstech]`.
4. Edite o arquivo `play_docker.yml` e ajuste os caminhos dos arquivos que deseja copiar no diretório `/h/nexcloud`. Certifique-se de ter os arquivos `docker-compose-nextcloud.yml` e `prometheus.yml` disponíveis.
5. Execute o playbook do Ansible: 
6. Aguarde até que o playbook seja executado com sucesso e verifique se o ambiente Nextcloud foi configurado corretamente.

### Funcionalidades

- Criação do diretório `/h/nexcloud`.
- Cópia dos arquivos `docker-compose-nextcloud.yml` e `prometheus.yml` para o diretório `/h/nexcloud`.
- Instalação do Docker e Docker Compose no host.

### Contribuição

Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novas funcionalidades para este playbook. Basta abrir uma pull request no repositório.

### Licença

Este playbook é licenciado sob a licença [MIT](https://opensource.org/licenses/MIT).
