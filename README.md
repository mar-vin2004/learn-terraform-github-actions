# Relatório: Automação do Terraform com GitHub Actions

Neste relatório, descreverei minha experiência ao seguir o tutorial "Automate Terraform with GitHub Actions". Explorarei os conceitos aprendidos, o passo a passo do artigo e os resultados obtidos.

## Tecnologia e Conceitos

Aprendi sobre a integração do Terraform com o GitHub Actions para automatizar o processo de provisionamento de infraestrutura. O Terraform é uma ferramenta de infraestrutura como código (IaC) da HashiCorp, enquanto o GitHub Actions é uma plataforma de automação para repositórios do GitHub.

Os principais conceitos incluem:

- Integração do GitHub Actions com a API do Terraform Cloud.
- Utilização de fluxos de trabalho do GitHub Actions para criar planos e aplicar configurações do Terraform.
- Configuração de webhooks no Terraform Cloud para receber notificações de eventos do GitHub.

## Passo a Passo

1. **Configuração do Terraform Cloud**: Criei um workspace no Terraform Cloud e configurei variáveis de ambiente para autenticar-me com a AWS. Também gerei um token de API do Terraform Cloud para autenticação no GitHub Actions.

   ![Configuração do Terraform Cloud](/assets/Captura de tela de 2024-04-10 10-52-42.png)

2. **Configuração do Repositório GitHub**: Criei um novo repositório a partir do template fornecido no artigo e configurei as secrets necessárias para autenticar-me com o Terraform Cloud.

3. **Revisão dos Fluxos de Trabalho do Actions**: Analisei os arquivos de configuração dos fluxos de trabalho do GitHub Actions fornecidos no repositório. Esses fluxos de trabalho são responsáveis por realizar ações como planificação e aplicação de configurações do Terraform.

4. **Criação de Pull Request e Mesclagem**: Criei um novo branch, fiz alterações nos arquivos de configuração e abri um pull request. Isso acionou automaticamente o fluxo de trabalho do GitHub Actions para planificação da infraestrutura.

   ![Criação de Pull Request](link_para_a_imagem)

5. **Verificação da Implantação**: Após mesclar o pull request, verifiquei a execução do fluxo de trabalho do GitHub Actions para aplicação da infraestrutura. Verifiquei também no Terraform Cloud a correta criação dos recursos.

   ![Verificação da Implantação](link_para_a_imagem)

6. **Teste de Acesso à Instância EC2**: Por fim, verifiquei se a instância EC2 provisionada estava acessível publicamente, utilizando o endereço web fornecido pelo Terraform Cloud.

   ![Teste de Acesso à Instância EC2](link_para_a_imagem)

## Resultados

- Concluí com sucesso a configuração de um workflow de CI/CD para automação do Terraform com GitHub Actions.
- Aprendi a integrar o Terraform Cloud com o GitHub Actions para automatizar o processo de provisionamento e implantação de infraestrutura.
- Verifiquei a correta execução dos fluxos de trabalho, desde a planificação até a aplicação da infraestrutura.
- Confirmei que a instância EC2 provisionada estava acessível publicamente, demonstrando a eficácia da automação.

## Conclusão

A automação do Terraform com GitHub Actions é uma abordagem poderosa para gerenciar infraestrutura de forma eficiente e escalável. Este tutorial proporcionou uma compreensão prática de como configurar e utilizar essas ferramentas em conjunto. Com essa base, posso criar pipelines de CI/CD robustos para automatizar completamente o ciclo de vida da infraestrutura.
