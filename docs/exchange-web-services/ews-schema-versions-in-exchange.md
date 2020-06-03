---
title: Versões de esquema do EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d1ab6f9c-ea91-4022-830d-7f7b759e3935
description: Saiba mais sobre o esquema do EWS e como projetar seu aplicativo para trabalhar com ele, bem como os recursos disponíveis em cada versão do esquema e como o esquema se relaciona com a versão do serviço do Exchange.
localization_priority: Priority
ms.openlocfilehash: 6afef658e747b11d9aa5fb7d7a88ba8f5c57ac82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456007"
---
# <a name="ews-schema-versions-in-exchange"></a>Versões de esquema do EWS no Exchange

Saiba mais sobre o esquema do EWS e como projetar seu aplicativo para trabalhar com ele, bem como os recursos disponíveis em cada versão do esquema e como o esquema se relaciona com a versão do serviço do Exchange.
  
O esquema do EWS define as estruturas de dados que podem ser enviadas e retornadas pelo Exchange. Cada nova versão do Exchange que contenha uma alteração significativa na funcionalidade do EWS conterá um novo esquema. O EWS e o esquema do EWS estão atrás e, em alguns casos, os aplicativos compatíveis com o recurso de encaminhamento de versões anteriores do EWS funcionarão, na maioria dos casos, com versões posteriores do EWS, e os aplicativos direcionados a versões posteriores do EWS funcionarão se a mesma funcionalidade tiver sido incluída em uma versão anterior. Este artigo ajudará você a entender a função do esquema do EWS, como a versão do esquema funciona, a relação entre a versão do esquema e a versão do serviço e como projetar seu aplicativo para trabalhar com o esquema do EWS. 
  
## <a name="role-of-the-ews-schema"></a>Função do esquema do EWS

O esquema EWS faz o seguinte:
  
- Define o conjunto de recursos que está disponível para um cliente. Um cliente pode obter a lista de versões de esquema com suporte usando o [serviço de descoberta automática](autodiscover-for-exchange.md)SOAP. O cliente pode então determinar quais recursos ele pode acessar, pois cada versão do esquema representa um [conjunto de recursos do EWS](ews-schema-versions-in-exchange.md#bk_features). Cada novo esquema lançado para EWS contém as entidades de esquema da versão anterior mais as definições de esquema para qualquer nova funcionalidade. Dessa forma, o EWS oferece suporte a aplicativos direcionados para uma versão anterior do EWS.
    
- Fornece uma descrição geral do contrato de API. Você pode usar este contrato para determinar as estruturas de dados que podem ser enviadas e recebidas do Exchange.
    
- Fornece um mecanismo de controle de versão para solicitações de envio. O servidor do Exchange contém todas as versões de esquema do EWS com suporte em seu diretório virtual. 
    
## <a name="designing-your-application-with-schema-version-in-mind"></a>Criando seu aplicativo com a versão do esquema em mente

Tenha em mente os seguintes pontos ao projetar seu aplicativo para trabalhar com versões diferentes do esquema do EWS:
  
- Ativar/desativar a funcionalidade com base na versão do esquema. Convém mapear a funcionalidade do cliente para a versão do esquema e, em alguns casos, para a versão do serviço. O exemplo a seguir retornará um [PropertySet](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) com base na versão do esquema e no serviço. 
    
  ```cs
  private static PropertySet InitPropertySetByVersion(ExchangeService service)
  {
      PropertySet props;
      // The schema version to target to access the NormalizedBody property 
      // is Exchange2013 or later. The server version to target to access the 
      // NormalizedBody property on an email is 15 or later, which 
      // equates to Exchange 2013.
      if (service.RequestedServerVersion >= ExchangeVersion.Exchange2013 &amp;&amp;
          service.ServerInfo.MajorVersion >= 15)
      {
          props = new PropertySet(EmailMessageSchema.NormalizedBody);
      }
      else
      {
          props = new PropertySet(EmailMessageSchema.Body);
      }
      return props;
  }
  ```

- Versão suas solicitações com a versão anterior do esquema do EWS que oferece suporte à funcionalidade que você deseja usar. Isso fará com que seu cliente se aplique a um número maior de possíveis servidores do Exchange. Isso é menos importante se você estiver desenvolvendo um aplicativo de linha de negócios para direcionar os servidores de sua organização apenas, mas é muito importante se você estiver criando um aplicativo para um público Exchange mais amplo.
    
## <a name="features-by-schema-version"></a>Recursos por versão de esquema
<a name="bk_features"> </a>

As versões de esquema que estão disponíveis para um cliente são identificadas no tipo simples **ExchangeVersionType** localizado no esquema Types. xsd. O **ExchangeVersionType** é implementado pelo elemento [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) . O elemento **RequestServerVersion** é enviado em todas as solicitações EWS para indicar ao servidor qual versão do esquema o cliente está direcionado. Isso, por sua vez, identifica o conjunto de recursos que está disponível para o cliente. 
  
**Tabela 1: recursos do EWS por produto e versão de esquema**

|**Versão do produto**|**Versão de esquema associada**|**Recursos**|
|:-----|:-----|:-----|
|Exchange Online  |A versão mais recente do esquema.  |Inclui todos os recursos da versão atual do Exchange além de qualquer novo recurso adicionado para clientes online. |
|Exchange 2013 SP1 |Exchange2013_SP1 | Inclui todos os recursos do Exchange 2013.<br/><br/>Os seguintes recursos foram introduzidos no Exchange 2013 SP1: <ul><li>[Política de retenção de caixa de correio](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) </li><li> [Propor novo horário](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) </li><li>  Ler atualizações de confirmação para [atualização](https://msdn.microsoft.com/library/office/dn600559%28v=exchg.80%29.aspx) e [exclusão](https://msdn.microsoft.com/library/office/dn600557%28v=exchg.80%29.aspx) de itens  </li><li> Atualização de [informações do IRM](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.conversation.hasirm%28v=exchg.80%29.aspx) para conversas  </li></ul> |
|Exchange 2013   |Exchange2013   | Inclui todos os recursos introduzidos no Exchange 2007 e no Exchange 2010. <br/><br/>Os seguintes recursos foram introduzidos no Exchange 2013:<ul><li>Arquivamento  </li><li>  Descoberta eletrônica  </li><li>  Personas  </li><li>  Políticas de retenção  </li><li>  Armazenamento de Contato Unificado  </li><li>  Fotos do usuário  </li></ul> |
|Exchange 2010 SP3   |Exchange2010_SP2 | Inclui todos os recursos introduzidos no Exchange 2010 SP1. <br/><br/>Os seguintes recursos foram introduzidos no Exchange 2010 SP2:<ul><li>Obter expiração de senha  </li><li>  Precisão DateTime  </li><li>  Identificadores de propriedade atualizados para contatos  </li><li>  Novos cenários de representação  </li></ul> |
|Exchange 2010 SP1  |Exchange2010_SP1   | Inclui todos os recursos introduzidos no Exchange 2010. <br/><br/>Os seguintes recursos foram introduzidos no Exchange 2010 SP1:<ul><li>Criar, recuperar e modificar regras de caixa de entrada  </li><li>  Acesso programático à caixa de correio de arquivo morto  </li><li>  Ações de conversas  </li><li>  Notificações de passagem de firewall  </li><li>  Recursos de administração aprimorados  </li><li>  Suporte aprimorado à versão mista  </li><li>  Suporte à proteção contra limitação  </li><li>  Controle do acesso de aplicativos ao EWS  </li><li>  Suporte a autenticação de certificado de cliente  </li></ul> |
|Exchange 2010  |Exchange2010   | Inclui todos os recursos introduzidos no Exchange 2007 SP1. <br/><br/>Os seguintes recursos foram introduzidos na versão inicial de lançamento do Exchange 2010:<ul><li>Lista de distribuição privada completa  </li><li>  Objetos de configuração do usuário  </li><li>  Itens associados da pasta  </li><li>  Controle de mensagens  </li><li>  Unificação de Mensagens  </li><li>  Descoberta Automática SOAP  </li><li>  Suporte avançado a fuso horário  </li><li>  Informações de disponibilidade do recurso de sala  </li><li>  Pesquisa indexada  </li><li>  Acesso de dumpster  </li><li>  Informações de dicas de dados  </li></ul> |
|Exchange 2007 SP1   |Exchange2007_SP1  | Inclui todos os recursos introduzidos no Exchange 2007. <br/><br/>Os seguintes recursos foram introduzidos no Exchange 2007 SP1:<ul><li>Gerenciamento de representante  </li><li>  Permissões de pastas  </li><li>  Pastas públicas  </li><li>  Itens post  </li><li>  Conversão de ID  </li></ul>|
|Exchange 2007  |Exchange2007 | Os seguintes recursos foram introduzidos na versão inicial de lançamento do Exchange 2007:<ul><li>Acesso completo a itens, pastas e anexos (criar, obter, atualizar, excluir)  </li><li>  Disponibilidade  </li><li>  Configurações de ausência temporária  </li><li>  Notificações  </li><li>  Sincronização  </li><li>  Resolução do nome  </li><li>  Expansão da lista de distribuição (DL)  </li><li>  Pesquisar  </li></ul> |
   
## <a name="relationship-between-the-ews-schema-and-the-service-version"></a>Relação entre o esquema do EWS e a versão do serviço
<a name="bk_features"> </a>

A versão do esquema do EWS está relacionada à versão do serviço EWS que o servidor está executando. O padrão de nomenclatura para o esquema do EWS está relacionado às versões locais do Exchange. Por exemplo, a versão inicial do Exchange 2013 tem uma versão de serviço do 15.00.0516.032 e o nome do esquema **Exchange2013**. Como o esquema foi atualizado para o Exchange 2013, o Exchange 2013 e o Exchange Online com uma versão de serviço do 15.00.0516.032 e posterior têm o mesmo nome de versão para o esquema mais recente. Nas versões anteriores do Exchange, o esquema do EWS não foi atualizado com as atualizações cumulativas (anteriormente chamadas de rollups). Mas como o Exchange é atualizado com mais frequência para oferecer suporte ao Exchange Online, as atualizações cumulativas agora contêm atualizações de esquema para o EWS. Os nomes de arquivo de esquema e o nome da versão do esquema associado são atualizados apenas com Service Packs ou versões principais do Exchange no local.
  
Enquanto o esquema do EWS define o contrato, em alguns cenários, a versão do serviço é a única maneira de um cliente determinar como ele deve interagir com o serviço. As alterações de comportamento de serviço que não são refletidas no esquema só podem ser determinadas pela versão de serviço retornada em todas as respostas do EWS. Por exemplo, quando as [pastas públicas](public-folder-access-with-ews-in-exchange.md) foram reprojetadas no Exchange 2013, as operações usadas para mover e copiar pastas públicas foram alteradas. Se você tiver criado um cliente para copiar pastas públicas no Exchange 2010, será necessário atualizá-lo para usar operações diferentes para obter o mesmo resultado no Exchange 2013. 
  
## <a name="how-the-ews-schema-is-updated"></a>Como o esquema do EWS é atualizado
<a name="bk_features"> </a>

Os servidores do Exchange que executam versões do Exchange a partir do Exchange 2007 incluem o esquema do EWS no diretório virtual que hospeda o serviço do EWS. A versão atual do esquema é sempre representada pelos arquivos Types. xsd e messages. xsd. A Figura 1 mostra como o esquema messages. xsd é bifurcado quando uma nova versão do esquema é desenvolvida. Antes da adição da nova funcionalidade, uma cópia do esquema messages. xsd original é incluída e renomeada para representar a versão anterior do esquema. O arquivo messages. xsd é atualizado com a descrição de serviço para a nova versão.
  
**Figura 1. Como o esquema do EWS é atualizado**

![Uma ilustração que mostra como o esquema EWS é atualizado. A última versão do esquema é bifurcada e renomeada para representar a versão anterior, e o nome do arquivo mais recente representa a versão atual.](media/Ex15_EWS_Schema_Update1.png)
  
Antes do esquema do EWS ser atualizado para uma nova versão, a versão atual do esquema é bifurcada e renomeada usando a seguinte convenção:
  
`<schemaname>-<majorserverversion><servicepack>.xsd`
  
O nome do arquivo original representa o esquema mais recente. Todos os novos recursos são adicionados ao esquema mais recente, com a exceção de atualizações e correções para as versões anteriores do esquema. 
  
## <a name="see-also"></a>Confira também

- [Versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md) 
- [Descoberta Automática do Exchange](autodiscover-for-exchange.md) 
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

