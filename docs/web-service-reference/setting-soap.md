---
title: Setting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: O elemento Setting representa uma configuração a ser retornada.
ms.openlocfilehash: 2e03bfacaf36676ee4687c148f3b08732a9f17b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539140"
---
# <a name="setting-soap"></a>Setting (SOAP)

O **elemento Setting** representa uma configuração a ser retornada. 
  
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
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das configurações solicitadas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é a configuração. A tabela a seguir lista as configurações possíveis.
  
|**Definição de configuração**|**Descrição**|
|:-----|:-----|
|NomeParaExibiçãoDoUsuário  <br/> |O nome de exibição do usuário.  <br/> |
|UserDN  <br/> |O nome diferenciado herddo do usuário.  <br/> |
|UserDeploymentId  <br/> |O identificador de implantação do usuário.  <br/> |
|InternalMailboxServer  <br/> |O FQDN (nome de domínio totalmente qualificado) do servidor de caixa de correio.  <br/> |
|InternalRpcClientServer  <br/> |O nome de domínio totalmente qualificado do servidor cliente RPC.  <br/> |
|InternalMailboxServerDN  <br/> |O nome diferenciado herddo do servidor de caixa de correio.  <br/> |
|InternalEcpUrl  <br/> |A URL interna do painel de Exchange de controle.  <br/> |
|InternalEcpVoicemailUrl  <br/> |A URL interna do painel de controle Exchange para Personalização do VoiceMail.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |A URL interna do painel de controle Exchange para assinaturas de email.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |A URL interna do painel de controle Exchange para Mensagens de Texto.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |A URL interna do painel de controle Exchange para relatórios de entrega.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |A URL interna do painel de controle Exchange para marcas RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |A URL interna do painel de controle Exchange para publicação.  <br/> |
|InternalEwsUrl  <br/> |A URL interna dos Exchange Web.  <br/> |
|InternalOABUrl  <br/> |A URL interna do OAB (lista de endereços offline).  <br/> |
|InternalUMUrl  <br/> |A URL interna dos serviços de Unificação de Mensagens.  <br/> |
|InternalWebClientUrls  <br/> |As URLs internas do cliente Exchange Web.  <br/> |
|MailboxDN  <br/> |O nome diferenciado do banco de dados de caixa de correio da caixa de correio do usuário.  <br/> |
|PublicFolderServer  <br/> |O nome do servidor de pastas públicas.  <br/> |
|ActiveDirectoryServer  <br/> |O nome do servidor do Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |O nome do servidor RPC sobre HTTP.  <br/> |
|ExternalMailboxServerRequiresSL  <br/> |O indicador para se o servidor RPC sobre HTTP requer SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Os métodos de autenticação suportados pelo servidor RPC sobre HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |O fragmento de URL do painel Exchange controle para personalização do VoiceMail.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |O fragmento de URL do painel de controle Exchange para assinaturas de email.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |O fragmento de URL do painel Exchange de controle para mensagens de texto.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |O fragmento de URL do painel de controle Exchange para relatórios de entrega.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |O fragmento de URL do painel de controle Exchange para marcas RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |O fragmento de URL do painel de controle Exchange para publicação.  <br/> |
|ExternalEcpUrl  <br/> |A URL externa do painel Exchange Controle.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |A URL externa do painel de controle Exchange para Personalização do VoiceMail.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |A URL externa do painel de controle Exchange para assinaturas de email.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |A URL externa do painel de controle Exchange de mensagens de texto.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |A URL externa do painel de controle Exchange para relatórios de entrega.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |A URL externa do painel de controle Exchange para marcas RetentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |A URL externa do painel Exchange controle para publicação.  <br/> |
|ExternalEwsUrl  <br/> |A URL externa do Exchange Web.  <br/> |
|ExternalOABUrl  <br/> |A URL externa do OAB.  <br/> |
|ExternalUMUrl  <br/> |A URL externa dos serviços de Unificação de Mensagens.  <br/> |
|ExternalWebClientUrls  <br/> |As URLs externas do cliente Exchange Web.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indica que o compartilhamento entre organizações está habilitado.  <br/> |
|AlternateMailboxes  <br/> |Coleção de caixas de correio alternativas.  <br/> |
|CasVersion  <br/> |A versão do servidor de Acesso para Cliente que está atendendo à solicitação (por exemplo, 14.XX.YYYY. ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Uma lista separada por vírgulas de versões de esquema com suporte Exchange Web Services. Os valores de versão do esquema serão os mesmos da enumeração **ExchangeServerVersion.**  <br/> |
|InternalPop3Connections  <br/> |A lista de configurações de conexão interna para conexões de protocolo POP3.  <br/> |
|ExternalPop3Connections  <br/> |A lista de configurações de conexão externa para conexões de protocolo POP3.  <br/> |
|InternalImap4Connections  <br/> |A lista de configurações de conexão interna para conexões de protocolo IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |A lista de configurações de conexão externa para conexões de protocolo IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |A lista de configurações de conexão interna para conexões SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |A lista de configurações de conexão externa para conexões SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |O sinalizador de conexão exclusiva do servidor interno. Se definido como "Desligado", os clientes não devem se conectar por meio desse protocolo.  <br/> |
|ExternalServerExclusiveConnect  <br/> |O sinalizador de conexão exclusiva do servidor externo. Se definido como "Ligado", os clientes devem se conectar por meio desse protocolo.  <br/> |
|ExchangeRpcUrl  <br/> |A URL usada para Chamadas de Procedimento Remoto. Essa URL é interna para o servidor e não deve ser usada pelos clientes.  <br/> |
|ShowGalAsDefaultView  <br/> |Especifica um valor Boolean que indica se a GAL deve ser mostrada como o livro de endereços. Um valor de texto "true" indica que a GAL deve ser mostrada por padrão. Um valor de texto "false" indica que a lista de contatos deve ser mostrada.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |O Endereço SMTP Primário de Descoberta Automática para o usuário. Esse é o endereço proxy em vez do endereço de email do usuário, se houver um endereço proxy.  <br/> |
|InteropExternalEwsUrl  <br/> |A URL externa do ponto de extremidade do serviço Web do servidor. Essa é a URL de um servidor que pode atender caixas de correio hospedadas em um servidor que não tem os serviços Web.  <br/> |
|ExternalEwsVersion  <br/> |A versão do servidor de serviços Web que está entregando a solicitação especificada.  <br/> |
|InteropExternalEwsVersion  <br/> |A versão do servidor InteropExternalEwsUrl está apontando para.  <br/> |
|MobileMailboxPolicyInterop  <br/> |As configurações de política de caixa de correio móvel.  <br/> |
|GroupingInformation  <br/> |Um valor usado em conjunto com a configuração ExternalEwsUrl para agrupar várias caixas de correio para manter [a](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) afinidade ao assinar notificações.  <br/> |
|UserMSOnline  <br/> |Um valor Boolean que indica se a caixa de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Um valor Boolean que indica se a caixa de correio do usuário está acessível por meio do protocolo MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

