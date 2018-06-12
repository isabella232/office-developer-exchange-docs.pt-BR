---
title: Protocolo (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: O elemento de protocolo contém as especificações para conectar um cliente para o computador que está executando o Exchange Server que possui a função de servidor acesso para cliente instalada.
ms.openlocfilehash: e58ae82ea5ec9d39db0f9219f6019df7da24a343
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824926"
---
# <a name="protocol-pox"></a>Protocolo (POX)

O elemento de **protocolo** contém as especificações para conectar um cliente para o computador que está executando o Exchange Server que possui a função de servidor acesso para cliente instalada. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
```xml
<Protocol>
   <Type/>
   <Internal/>
   <External/>
   <TTL/>
   <Server/>
   <ServerDN/>
   <ServerVersion/>
   <MdbDN/>
   <PublicFolderServer/>
   <Port/>
   <DirectoryPort/>
   <ReferralPort/>
   <ASUrl/>
   <EwsUrl/>
   <EmwsUrl/>
   <SharingUrl/>
   <EcpUrl/>
   <EcpUrl-um/>
   <EcpUrl-aggr/>
   <EcpUrl-mt/>
   <EcpUrl-ret/>
   <EcpUrl-sms/>
   <EcpUrl-publish/>
   <EcpUrl-photo/>
   <EcpUrl-tm/>
   <EcpUrl-tmCreating/>
   <EcpUrl-tmHiding/>
   <EcpUrl-tmEditing/>
   <EcpUrl-extinstall/>
   <OOFUrl/>
   <OABUrl/>
   <UMUrl/>
   <EwsPartnerUrl/>
   <LoginName/>
   <DomainRequired/>
   <DomainName/>
   <SPA/>
   <AuthPackage/>
   <CertPrincipalName/>
   <SSL/>
   <AuthRequired/>
   <UsePOPAuth/>
   <SMTPLast/>
   <NetworkRequirements/>
   <AddressBook/>
   <MailStore/>
</Protocol>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Tipo  <br/> |Indica o tipo de protocolo descrito por esse elemento de **protocolo** . O único valor válido para este atributo é "mapiHttp". Este atributo é presente somente se a descoberta automática solicitar que corresponde a essa resposta [incluído um cabeçalho X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md). Este atributo é aplicável a clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, ou versões locais do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Versão  <br/> |Indica a versão do protocolo descrita por esse elemento de **protocolo** . O único valor válido para este atributo é "1". Este atributo só estará presente se a solicitação de descoberta automática que corresponde a essa resposta incluiu um cabeçalho **X-MapiHttpCapability** . Este atributo é aplicável a clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, ou versões locais do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Tipo (POX)](type-pox.md) <br/> |Identifica o tipo da conta de email configurada.  <br/> |
|[Interno (POX)](internal-pox.md) <br/> |Contém uma coleção de URLs que um cliente pode usar para se conectar ao Exchange de dentro da rede da organização.  <br/> |
|[Externo (POX)](external-pox.md) <br/> |Contém uma coleção de URLs que um cliente pode usar para se conectar ao Exchange de fora da rede da organização.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas.  <br/> |
|[Servidor (POX)](server-pox.md) <br/> |Especifica o nome do servidor de email.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Especifica o nome diferenciado do Exchange Server.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Representa o número de versão do Exchange Server.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Representa o nome diferenciado do banco de dados de caixa de correio.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Contém o nome de domínio totalmente qualificado (FQDN) do servidor de pasta pública para o usuário.  <br/> |
|[Porta (POX)](port-pox.md) <br/> |Especifica a porta que é usada para conexão com o repositório.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Especifica a porta usada para conectar ao diretório quando o protocolo de Interface de provedor de serviço de nome (NSPI) é usado.  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Especifica a porta usada para obter uma referência para um diretório.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Especifica a URL da instância recomendada dos serviços da Web do Exchange para um usuário habilitado para email.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Contém a URL do servidor de compartilhamento usado para entre organizações compartilhamento de calendários e contatos.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Especifica a URL do painel de controle do Exchange para um usuário habilitado para email.  <br/> |
|[EcpUrl-um POX)](ecpurl-um-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de caixa postal de um usuário habilitado para email.  <br/> |
|[EcpUrl-agregação (POX)](ecpurl-aggr-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de agregação de lista segura de email para um usuário habilitado para email.  <br/> |
|[EcpUrl-mt POX)](ecpurl-mt-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações para um usuário habilitado para email de acompanhamento de mensagens de email.  <br/> |
|[EcpUrl-resposta POX)](ecpurl-ret-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de marca de retenção para um usuário habilitado para email.  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações do serviço SMS (Short Message) para um usuário habilitado para email.  <br/> |
|[EcpUrl-publicar (POX)](ecpurl-publish-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de publicação de calendário de um usuário habilitado para email.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar um habilitados para email foto do usuário atual.  <br/> |
|[EcpUrl-tm POX)](ecpurl-tm-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site dos quais um usuário habilitado para email é membro atualmente.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para criar uma nova caixa de correio do site.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para cancelar o usuário a partir de uma caixa de correio do site.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para editar uma caixa de correio de site existentes.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email instalados atualmente na caixa de correio do usuário.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Especifica a URL da instância melhor do que o serviço de disponibilidade para um usuário habilitado para email.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Especifica a URL do servidor do catálogo de Endereços Offline configuração para uma topologia do Exchange.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Especifica a URL da instância do serviço Web Unificação de mensagens para um usuário habilitado para email recomendada.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[LoginName POX)](loginname-pox.md) <br/> |Especifica o nome de logon do usuário.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Indica se o domínio é necessário para autenticação.  <br/> |
|[DomainName POX)](domainname-pox.md) <br/> |Especifica o domínio do usuário.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Indica se a autenticação de senha segura é necessária.  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |Especifica o esquema de autenticação usado quando autenticar contra o computador do Exchange 2007 que possui a função de servidor de caixa de correio instalada.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Especifica o nome principal do certificado Secure Sockets Layer (SSL) que é necessária para conectar-se à organização do Microsoft Exchange usando SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Especifica se o logon seguro é necessária.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Especifica se a autenticação é necessária.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Indica se as informações de autenticação que são fornecidas para um tipo de POP3 da conta também são usadas para SMTP Simple Mail Transfer Protocol ().  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Especifica se o servidor SMTP exige que o email seja baixada antes de enviar email usando o servidor SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Contém os critérios que são usados para determinar se o computador cliente está em uma rede que atenda aos requisitos do provedor de serviços de Internet para se conectar ao servidor.  <br/> |
|[AddressBook POX)](addressbook-pox.md) <br/> |Contém as especificações para conectar-se um cliente para o servidor de catálogo de endereços usando o protocolo MAPI/HTTP. Esse elemento só estará presente se o atributo de **tipo** no elemento **protocolo** está presente e definida como "mapiHttp". O elemento **AddressBook** é aplicável a clientes que implementam o protocolo MAPI/HTTP e o Exchange Online de destino e a versões do Exchange, começando com 15.00.0847.032.  <br/> |
|[Armazenamento_de_email (POX)](mailstore-pox.md) <br/> |Contém as especificações para conectar um cliente de caixa de correio do usuário por meio do protocolo MAPI/HTTP. Esse elemento só estará presente se o atributo de **tipo** no elemento **protocolo** está presente e definida como "mapiHttp". O elemento **Armazenamento_de_email** é aplicável a clientes que implementam o protocolo MAPI/HTTP e o Exchange Online de destino e a versões do Exchange, começando com 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações da conta do usuário.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O elemento de **protocolo** está presente em uma resposta que possui um valor de [Ação POX ()](action-pox.md) é igual a **configurações**.
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

