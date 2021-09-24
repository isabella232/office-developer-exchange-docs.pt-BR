---
title: Protocol (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: O elemento Protocol contém as especificações para conectar um cliente ao computador que está executando Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
ms.openlocfilehash: 4f308951c74612936755e6d4c16620e38277aecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516395"
---
# <a name="protocol-pox"></a>Protocol (POX)

O **elemento Protocol** contém as especificações para conectar um cliente ao computador que está executando Exchange Server que tem a função de servidor de Acesso para Cliente instalada. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Tipo  <br/> |Indica o tipo de protocolo descrito por este **elemento Protocol.** O único valor válido para esse atributo é "mapiHttp". Esse atributo só estará presente se a solicitação de Descoberta Automática que corresponde a essa resposta incluir um [header X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md). Esse atributo é aplicável aos clientes que implementam o protocolo MAPI/HTTP e o Exchange Online de destino, Exchange Online como parte do Office 365 ou versões locais do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Versão  <br/> |Indica a versão do protocolo descrito por este **elemento Protocol.** O único valor válido para esse atributo é "1". Esse atributo só estará presente se a solicitação de Descoberta Automática que corresponde a essa resposta incluir um header **X-MapiHttpCapability.** Esse atributo é aplicável aos clientes que implementam o protocolo MAPI/HTTP e o Exchange Online de destino, Exchange Online como parte do Office 365 ou versões locais do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |Identifica o tipo da conta de email configurada.  <br/> |
|[Internal (POX)](internal-pox.md) <br/> |Contém uma coleção de URLs que um cliente pode usar para se conectar Exchange de dentro da rede da organização.  <br/> |
|[External (POX)](external-pox.md) <br/> |Contém uma coleção de URLs que um cliente pode usar para se conectar Exchange de fora da rede da organização.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Especifica a hora de vida, em horas, durante a qual as configurações permanecem válidas.  <br/> |
|[Server (POX)](server-pox.md) <br/> |Especifica o nome do servidor de email.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Especifica o nome Exchange Server distinto.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Representa o Exchange Server de versão.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Representa o nome diferenciado do banco de dados de caixa de correio.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Contém o FQDN (nome de domínio totalmente qualificado) do servidor de pasta pública do usuário.  <br/> |
|[Port (POX)](port-pox.md) <br/> |Especifica a porta usada para se conectar ao armazenamento.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Especifica a porta usada para se conectar ao diretório quando o protocolo NSPI (Name Service Provider Interface) é usado.  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Especifica a porta usada para obter uma referência para um diretório.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Especifica a URL da melhor instância do Exchange Web para um usuário habilitado para email.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Especifica a URL da melhor instância de ponto de extremidade para Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Especifica a URL da melhor instância de ponto de extremidade para Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Contém a URL do servidor de compartilhamento usado para compartilhamento entre organizações de calendários e contatos.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Especifica a URL do painel de controle Exchange para um usuário habilitado para email.  <br/> |
|[EcpUrl-um (POX)](ecpurl-um-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar configurações de caixa postal para um usuário habilitado para email.  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar configurações de agregação de email para um usuário habilitado para email.  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de controle de mensagens de email para um usuário habilitado para email.  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de marca de retenção para um usuário habilitado para email.  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar configurações de SMS (Serviço de Mensagem Curta) para um usuário habilitado para email.  <br/> |
|[EcpUrl-publish (POX)](ecpurl-publish-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar configurações de publicação de calendário para um usuário habilitado para email.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar a foto atual de um usuário habilitado para email.  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site das quais um usuário habilitado para email é membro no momento.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para criar uma nova caixa de correio de site.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para cancelar a assinatura do usuário de uma caixa de correio de site.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para editar uma caixa de correio de site existente.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email atualmente instalados na caixa de correio do usuário.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Especifica a URL da melhor instância do serviço de disponibilidade para um usuário habilitado para email.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Especifica a URL do servidor de configuração do Livro de Endereços Offline para Exchange topologia.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Especifica a URL da melhor instância do serviço Web de Unificação de Mensagens para um usuário habilitado para email.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Especifica a URL da melhor instância de ponto de extremidade para Exchange Web Services (EWS) para um usuário habilitado para email.  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |Especifica o nome de logon do usuário.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Indica se o domínio é necessário para autenticação.  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |Especifica o domínio do usuário.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Indica se a autenticação de senha segura é necessária.  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |Especifica o esquema de autenticação usado ao autenticar no computador Exchange 2007 que tem a função de servidor de Caixa de Correio instalada.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização do Microsoft Exchange usando SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Especifica se o logon seguro é necessário.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Especifica se a autenticação é necessária.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Indica se as informações de autenticação fornecidas para um tipo pop3 de conta também são usadas para o SMTP (Simple Mail Transfer Protocol).  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Especifica se o servidor SMTP exige que o email seja baixado antes de enviar emails usando o servidor SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Contém os critérios usados para determinar se o computador cliente está em uma rede que atende aos requisitos do Provedor de Serviços da Internet para se conectar ao servidor.  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP. Esse elemento só estará presente se o atributo **Type** no elemento **Protocol** estiver presente e definido como "mapiHttp". O elemento **AddressBook** é aplicável aos clientes que implementam o protocolo MAPI/HTTP e Exchange Online e versões do Exchange começando com 15.00.0847.032.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP. Esse elemento só estará presente se o atributo **Type** no elemento **Protocol** estiver presente e definido como "mapiHttp". O **elemento MailStore** é aplicável aos clientes que implementam o protocolo MAPI/HTTP e Exchange Online e versões do Exchange começando com 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Especifica as configurações da conta para o usuário.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento Protocol** está presente em uma resposta que tem um valor Action [(POX)](action-pox.md) igual a **configurações**.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

