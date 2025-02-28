---
title: About GitHub Enterprise Server
intro: '{% data variables.product.product_name %} is a software development platform that you can host in a private environment.'
versions:
  ghes: '*'
type: overview
topics:
  - Enterprise
  - Fundamentals
---

## About {% data variables.product.product_name %}

{% data reusables.enterprise.ghes-is-a-self-hosted-platform %} Your team can use {% data variables.product.product_name %} to build and ship software using Git version control, powerful APIs, productivity and collaboration tools, and integrations. Developers familiar with {% data variables.product.prodname_dotcom_the_website %} can onboard and contribute seamlessly using familiar features and workflows.

{% data reusables.enterprise.ghes-runs-on-your-infrastructure %}

{% data reusables.enterprise.github-distributes-ghes %} For more information, see "[System overview](/admin/overview/system-overview)."

You can choose to deploy {% data variables.product.product_name %} on premises, or to a supported cloud environment.

## Supported environments for deployment

You can deploy {% data variables.product.product_name %} to a virtualization hypervisor within your on-premises datacenter, or to a public cloud service.

{% data variables.product.company_short %} supports the following virtualization hypervisors for on-premises deployment.

- Microsoft Hyper-V
- OpenStack KVM
- VMware ESXi

{% data variables.product.company_short %} supports the following services for cloud deployment.

- Amazon Web Services (AWS)
- Google Cloud Platform (GCP)
- Microsoft Azure

Para obtener más información, consulta "[Configurar una instancia del {% data variables.product.prodname_ghe_server %}](/admin/installation/setting-up-a-github-enterprise-server-instance)."

## About releases and upgrades

{% data reusables.enterprise.constantly-improving %} You are responsible for upgrades to your instance. For more information, see "[{% data variables.product.product_name %} releases](/admin/all-releases)."

## About administration

You can configure and monitor {% data variables.product.product_name %} via browser, administrative SSH access, and REST or GraphQL APIs. {% data variables.product.company_short %} has found that people with Linux administration experience are more successful with the deployment and maintainance of {% data variables.product.product_name %}.

You can give certain employees administrative access to {% data variables.product.product_name %}, so they can set up external authentication, configure the instance to meet developer needs, and monitor the instance's activity and performance. To ensure compliance with business rules or regulatory restrictions, administrators can configure policies that control how people use {% data variables.product.product_location %}. Para obtener más información, consulta los siguientes artículos.

- "[About authentication for your enterprise](/admin/identity-and-access-management/managing-iam-for-your-enterprise/about-authentication-for-your-enterprise)"
- "[Configuring your enterprise](/admin/configuration/configuring-your-enterprise)"
- "[About the {% data variables.product.prodname_enterprise %} API](/admin/overview/about-the-github-enterprise-api)"
- "[Monitoring your appliance](/admin/enterprise-management/monitoring-your-appliance)"
- "[Monitoring activity in your enterprise](/admin/monitoring-activity-in-your-enterprise)"
- "[About enterprise policies](/admin/policies/enforcing-policies-for-your-enterprise/about-enterprise-policies)"

## About optional features

You can configure optional features for {% data variables.product.product_name %} that improve the software development lifecycle for your enterprise.

| Característica                                               | Descripción                                                                                          | Más información                                                                                                                                                                               |
|:------------------------------------------------------------ |:---------------------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| {% data variables.product.prodname_actions %}                | Automate CI/CD and development workflows                                                             | "[Acerca de {% data variables.product.prodname_actions %} para empresas](/admin/github-actions/getting-started-with-github-actions-for-your-enterprise/about-github-actions-for-enterprises)" |
| {% data variables.product.prodname_github_connect %}       | Benefit from the power of {% data variables.product.prodname_dotcom_the_website %} in limited ways | "[Acerca de {% data variables.product.prodname_github_connect %}](/admin/configuration/configuring-github-connect/about-github-connect)"                                                    |
| {% data variables.product.prodname_GH_advanced_security %} | Improve code security and quality                                                                    | "[Acerca de {% data variables.product.prodname_GH_advanced_security %}](/get-started/learning-about-github/about-github-advanced-security)"                                                 |
| {% data variables.product.prodname_registry %}               | Host software packages for your enterprise                                                           | "[Introduction to {% data variables.product.prodname_registry %}](/packages/learn-github-packages/introduction-to-github-packages)"                                                           |

## About deployment topologies

By default, {% data variables.product.product_name %} runs as a standalone instance. You can increase the reliability and performance of {% data variables.product.product_name %} by using a different topology for your deployment.

- To mitigate the impact of system or network failures, you can deploy a passive replica instance. During an outage that affects your primary instance, you can manually fail over to the replica instance. Para obtener más información, consulta "[Acerca de la configuración de alta disponibilidad](/admin/enterprise-management/configuring-high-availability/about-high-availability-configuration)."
- You can configure multiple active replicas to improve performance for developers who are geographically distant from your primary instance. Para obtener más información, consulta la sección "[Acerca de la geo-replicación](/admin/enterprise-management/configuring-high-availability/about-geo-replication)".
- Some enterprises with tens of thousands of developers may benefit from a cluster configuration that scales horizontally instead of vertically. Para obtener más información, consulta "[Acerca de las agrupaciones](/admin/enterprise-management/configuring-clustering/about-clustering)."

## About backups and disaster recovery

To safeguard against data loss or service disruptions for your developers, {% data variables.product.company_short %} strongly recommends that you establish a plan for disaster recovery. You can back up your instance's configuration and user data by deploying and configuring a Linux or Unix host system with {% data variables.product.prodname_enterprise_backup_utilities %}. Para obtener más información, consulta "[Configurar copias de seguridad en tu aparato](/admin/configuration/configuring-your-enterprise/configuring-backups-on-your-appliance)"

Additionally, you can configure a passive replica instance to fail over to in the event of a system or network failure. For more information, see "[About deployment topologies](#about-deployment-topologies)."

## About documentation

Documentation for both administrators and users of {% data variables.product.product_name %} is available on this site, {% data variables.product.prodname_docs %}.

- [Documentación para administradores empresariales](/admin)
- [User documentation](/)

Different versions of {% data variables.product.product_name %} are reflected separately in the documentation on {% data variables.product.prodname_docs %}. Para obtener más información, consulta la sección "[Acerca de las versiones de {% data variables.product.prodname_docs %}](/get-started/learning-about-github/about-versions-of-github-docs)".

## Trying {% data variables.product.product_name %}

You can sign up for a free, 45-day trial of {% data variables.product.product_name %}. Para obtener más información, consulta "[Configurar una prueba de {% data variables.product.prodname_ghe_server %}](/get-started/signing-up-for-github/setting-up-a-trial-of-github-enterprise-server)".

## Leer más

- "[Iniciar con {% data variables.product.product_name %}](/get-started/onboarding/getting-started-with-github-enterprise-server)"
- "[Acerca de {% data variables.contact.github_support %}](/support/learning-about-github-support/about-github-support)"
- [ {% data variables.product.prodname_roadmap %} ]({% data variables.product.prodname_roadmap_link %}) en el repositorio `github/roadmap`
