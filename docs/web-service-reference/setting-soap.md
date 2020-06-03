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
description: O elemento Setting representa uma definição de configuração a ser retornada.
ms.openlocfilehash: df3b55fe7ba2c5ae92f8c31ec0643dbe100fa072
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466742"
---
# <a name="setting-soap"></a>Configuração (SOAP)

O elemento **Setting** representa uma definição de configuração a ser retornada. 
  
```XML
<Setting/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das definições de configuração solicitadas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é a definição de configuração. A tabela a seguir lista as definições de configuração possíveis.
  
|**Definição de configuração**|**Descrição**|
|:-----|:-----|
|NomeParaExibiçãoDoUsuário  <br/> |O nome de exibição do usuário.  <br/> |
|UserDN  <br/> |O nome diferenciado herdado do usuário.  <br/> |
|Userdeploymentid  <br/> |O identificador de implantação do usuário.  <br/> |
|InternalMailboxServer  <br/> |O FQDN (nome de domínio totalmente qualificado) do servidor de caixa de correio.  <br/> |
|InternalRpcClientServer  <br/> |O nome de domínio totalmente qualificado do servidor cliente RPC.  <br/> |
|InternalMailboxServerDN  <br/> |O nome diferenciado herdado do servidor de caixa de correio.  <br/> |
|InternalEcpUrl  <br/> |A URL interna do painel de controle do Exchange.  <br/> |
|InternalEcpVoicemailUrl  <br/> |A URL interna do painel de controle do Exchange para a personalização de caixa postal.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |A URL interna do painel de controle do Exchange para assinaturas de email.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |A URL interna do painel de controle do Exchange para mensagens de texto.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |A URL interna do painel de controle do Exchange para relatórios de entrega.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |A URL interna do painel de controle do Exchange para marcas RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |A URL interna do painel de controle do Exchange para publicação.  <br/> |
|InternalEwsUrl  <br/> |A URL interna dos serviços Web do Exchange.  <br/> |
|InternalOABUrl  <br/> |A URL interna do catálogo de endereços offline (OAB).  <br/> |
|InternalUMUrl  <br/> |A URL interna dos serviços de Unificação de mensagens.  <br/> |
|InternalWebClientUrls  <br/> |As URLs internas do cliente Web do Exchange.  <br/> |
|MailboxDN  <br/> |O nome distinto do banco de dados de caixa de correio da caixa de correio do usuário.  <br/> |
|PublicFolderServer  <br/> |O nome do servidor de pastas públicas.  <br/> |
|ActiveDirectoryServer  <br/> |O nome do servidor do Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |O nome do servidor RPC sobre HTTP.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |O indicador para saber se o servidor RPC sobre HTTP exige SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Os métodos de autenticação suportados pelo servidor RPC sobre HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |O fragmento de URL do painel de controle do Exchange para a personalização de caixa postal.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para assinaturas de email.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para mensagens de texto.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para relatórios de entrega.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para marcas RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |O fragmento de URL do painel de controle do Exchange para publicação.  <br/> |
|ExternalEcpUrl  <br/> |A URL externa do painel de controle do Exchange.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |A URL externa do painel de controle do Exchange para a personalização de caixa postal.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |A URL externa do painel de controle do Exchange para assinaturas de email.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |A URL externa do painel de controle do Exchange para mensagens de texto.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |A URL externa do painel de controle do Exchange para relatórios de entrega.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |A URL externa do painel de controle do Exchange para marcas RetentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |A URL externa do painel de controle do Exchange para publicação.  <br/> |
|ExternalEwsUrl  <br/> |A URL externa dos serviços Web do Exchange.  <br/> |
|ExternalOABUrl  <br/> |A URL externa do OAB.  <br/> |
|ExternalUMUrl  <br/> |A URL externa dos serviços de Unificação de mensagens.  <br/> |
|ExternalWebClientUrls  <br/> |As URLs externas do cliente Web do Exchange.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indica que o compartilhamento entre organizações está habilitado.  <br/> |
|AlternateMailboxes  <br/> |Conjunto de caixas de correio alternadas.  <br/> |
|CasVersion  <br/> |A versão do servidor de acesso para cliente que está servindo a solicitação (por exemplo, 14. XX. DD. ZZZ  <br/> |
|EwsSupportedSchemas  <br/> |Uma lista separada por vírgulas de versões de esquema compatíveis com os serviços Web do Exchange. Os valores de versão do esquema serão os mesmos dos valores da enumeração **ExchangeServerVersion** .  <br/> |
|InternalPop3Connections  <br/> |A lista de configurações de conexão interna para conexões do protocolo POP3.  <br/> |
|ExternalPop3Connections  <br/> |A lista de configurações de conexão externa para conexões do protocolo POP3.  <br/> |
|InternalImap4Connections  <br/> |A lista de configurações de conexão interna para conexões de protocolo IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |A lista de configurações de conexão externa para conexões de protocolo IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |A lista de configurações de conexão interna para conexões SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |A lista de configurações de conexão externa para conexões SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |O sinalizador de conexão exclusivo do servidor interno. Se for definido como "desativado", os clientes não deverão se conectar por meio desse protocolo.  <br/> |
|ExternalServerExclusiveConnect  <br/> |O sinalizador de conexão exclusivo do servidor externo. Se definido como "ativado", os clientes devem se conectar por meio desse protocolo.  <br/> |
|ExchangeRpcUrl  <br/> |A URL usada para chamadas de procedimento remoto. Esta URL é interna ao servidor e não deve ser usada por clientes.  <br/> |
|ShowGalAsDefaultView  <br/> |Especifica um valor Boolean que indica se a GAL deve ser mostrada como o catálogo de endereços. Um valor de texto "true" indica que a GAL deve ser mostrada por padrão. Um valor de texto "false" indica que a lista de contatos deve ser mostrada.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |O endereço SMTP principal do autodiscover para o usuário. Este é o endereço de proxy em vez do endereço de email do usuário, se houver um endereço de proxy.  <br/> |
|InteropExternalEwsUrl  <br/> |A URL externa do ponto de extremidade do serviço Web do servidor. Esta é a URL para um servidor que pode servir caixas de correio hospedadas em um servidor que não tenha os serviços Web.  <br/> |
|ExternalEwsVersion  <br/> |A versão do servidor de serviços Web que está fornecendo a solicitação especificada.  <br/> |
|InteropExternalEwsVersion  <br/> |A versão do servidor InteropExternalEwsUrl está apontando para.  <br/> |
|MobileMailboxPolicyInterop  <br/> |As configurações da política de caixa de correio móvel.  <br/> |
|GroupingInformation  <br/> |Um valor usado em conjunto com a configuração ExternalEwsUrl para agrupar várias caixas de correio juntas para [manter a afinidade](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) ao assinar notificações.  <br/> |
|UserMSOnline  <br/> |Um valor booliano que indica se a caixa de correio do usuário está hospedada no Exchange Online ou no Exchange Online como parte do Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Um valor Boolean que indica se a caixa de correio do usuário pode ser acessada por meio do protocolo MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

