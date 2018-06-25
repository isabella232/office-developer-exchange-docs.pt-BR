---
title: Configuração (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: O elemento Setting representa uma definição de configuração a ser retornado.
ms.openlocfilehash: cb5b1d6ab2109b48810b96221b76c6b8fc9803ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825472"
---
# <a name="setting-soap"></a>Configuração (SOAP)

O elemento **Setting** representa uma definição de configuração a ser retornado. 
  
```XML
<Setting/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das definições de configuração solicitada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto para esse elemento é a definição de configuração. A tabela a seguir lista as configurações possíveis.
  
|**Definição de configuração**|**Descrição**|
|:-----|:-----|
|UserDisplayName  <br/> |O nome de exibição do usuário.  <br/> |
|NDUsuário  <br/> |O nome distinto herdado do usuário.  <br/> |
|UserDeploymentId  <br/> |O identificador de implantação do usuário.  <br/> |
|InternalMailboxServer  <br/> |O nome de domínio totalmente qualificado (FQDN) do servidor de caixa de correio.  <br/> |
|InternalRpcClientServer  <br/> |O nome de domínio totalmente qualificado do servidor de cliente RPC.  <br/> |
|InternalMailboxServerDN  <br/> |O nome distinto herdado do servidor de caixa de correio.  <br/> |
|InternalEcpUrl  <br/> |A URL interna do painel de controle do Exchange.  <br/> |
|InternalEcpVoicemailUrl  <br/> |A URL interna do painel de controle do Exchange para personalização de caixa postal.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |A URL interna do painel de controle do Exchange para assinaturas de Email.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |A URL interna do painel de controle do Exchange para mensagens de texto.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |A URL interna do painel de controle do Exchange para relatórios de entrega.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |A URL interna do painel de controle do Exchange para marcas de política de retenção.  <br/> |
|InternalEcpPublishingUrl  <br/> |A URL interna do painel de controle do Exchange para publicação.  <br/> |
|InternalEwsUrl  <br/> |A URL do Exchange serviços Web internos.  <br/> |
|InternalOABUrl  <br/> |A URL interna do catálogo de endereços offline (OAB).  <br/> |
|InternalUMUrl  <br/> |A URL interna dos serviços de Unificação de mensagens.  <br/> |
|InternalWebClientUrls  <br/> |As URLs internas do cliente da Web do Exchange.  <br/> |
|MailboxDN  <br/> |O nome distinto do banco de dados de caixa de correio da caixa de correio do usuário.  <br/> |
|PublicFolderServer  <br/> |O nome do servidor de pastas públicas.  <br/> |
|ActiveDirectoryServer  <br/> |O nome do servidor do Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |O nome do RPC sobre servidores HTTP.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |O indicador para o RPC sobre servidores HTTP requer o SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Os métodos de autenticação que são compatíveis com o RPC sobre servidores HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |O fragmento de URL do painel de controle do Exchange para personalização de caixa postal.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para assinaturas de Email.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para mensagens de texto.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para relatórios de entrega.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para marcas de política de retenção.  <br/> |
|EcpPublishingUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para publicação.  <br/> |
|ExternalEcpUrl  <br/> |A URL externa do painel de controle do Exchange.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |A URL externa do painel de controle do Exchange para personalização de caixa postal.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |A URL externa do painel de controle do Exchange para assinaturas de Email.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |A URL externa do painel de controle do Exchange para mensagens de texto.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |A URL externa do painel de controle do Exchange para relatórios de entrega.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |A URL externa do painel de controle do Exchange para marcas de política de retenção.  <br/> |
|ExternalEcpPublishingUrl  <br/> |A URL externa do painel de controle do Exchange para publicação.  <br/> |
|ExternalEwsUrl  <br/> |A URL externa dos serviços da Web do Exchange.  <br/> |
|ExternalOABUrl  <br/> |A URL externa do OAB.  <br/> |
|ExternalUMUrl  <br/> |A URL externa dos serviços de Unificação de mensagens.  <br/> |
|ExternalWebClientUrls  <br/> |As URLs externas do cliente da Web do Exchange.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indica que o compartilhamento entre organizações está habilitada.  <br/> |
|AlternateMailboxes  <br/> |Coleção de caixas de correio alternativas.  <br/> |
|CasVersion  <br/> |A versão do servidor acesso para cliente que está servindo a solicitação (por exemplo, 14.XX. YYYY. ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Uma lista separada por vírgulas de versões de esquema suportadas pelo Exchange Web Services. Os valores de versão do esquema será o mesmo que os valores da enumeração **ExchangeServerVersion** .  <br/> |
|InternalPop3Connections  <br/> |A lista de configurações de conexão interna para conexões de protocolo POP3.  <br/> |
|ExternalPop3Connections  <br/> |A lista de configurações de conexão externo para conexões de protocolo POP3.  <br/> |
|InternalImap4Connections  <br/> |A lista de configurações de conexão interna para conexões do protocolo IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |A lista de configurações de conexão externo para conexões do protocolo IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |A lista de configurações de conexão interna para conexões SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |A lista de configurações de conexão externo para conexões SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |O servidor interno exclusivo conectar sinalizador. Se definido como "Desativado", em seguida, clientes deve conectar via esse protocolo.  <br/> |
|ExternalServerExclusiveConnect  <br/> |O servidor externo exclusive conectar sinalizador. Se definido como "Ligado", em seguida, clientes deve se conectar via esse protocolo.  <br/> |
|ExchangeRpcUrl  <br/> |A URL que é usado para chamadas de procedimento remoto. Essa URL para o servidor interno e não deve ser usado pelos clientes.  <br/> |
|ShowGalAsDefaultView  <br/> |Especifica um valor Boolean que indica se a GAL deve ser exibida como o catálogo de endereços. Um valor de texto "true" indica que o GAL é a serem mostradas por padrão. Um valor de texto de "false" indica que a lista de contatos está a ser mostrado.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |O endereço SMTP principal descoberta automática para o usuário. Esse é o endereço de proxy em vez de eliminar o endereço de email do usuário, se houver um endereço de proxy.  <br/> |
|InteropExternalEwsUrl  <br/> |A URL externa do ponto de extremidade do serviço do servidor Web. Esta é a URL para um servidor que pode atender a caixas de correio hospedadas em um servidor que não tem os serviços Web.  <br/> |
|ExternalEwsVersion  <br/> |A versão do servidor de serviços da Web que está fornecendo a solicitação especificada.  <br/> |
|InteropExternalEwsVersion  <br/> |A versão do servidor InteropExternalEwsUrl está apontando para.  <br/> |
|MobileMailboxPolicyInterop  <br/> |As configurações de diretiva de caixa de correio móvel.  <br/> |
|GroupingInformation  <br/> |Um valor usado em conjunto com a configuração de ExternalEwsUrl para agrupar várias caixas de correio juntos para [manter a afinidade](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) quando a assinatura de notificações.  <br/> |
|UserMSOnline  <br/> |Um valor Boolean que indica se caixas de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Um valor Boolean que indica se a caixa de correio do usuário é acessível através do protocolo MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

