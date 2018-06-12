---
title: Transporte namespaces de agente no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Saiba mais sobre as classes do .NET Framework e os membros que você pode usar para criar os agentes de transporte personalizado para o Exchange 2013.
ms.openlocfilehash: a8189ca9915312b64fefda3091f8f81e51271ad6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751030"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Transporte namespaces de agente no Exchange 2013

Saiba mais sobre as classes do .NET Framework e os membros que você pode usar para criar os agentes de transporte personalizado para o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os namespaces que contêm informações de referência que você pode usar para criar os agentes de transporte do Exchange Server 2013. Também descreve as classes que seus agentes de transporte podem usar para ler e modificar as mensagens de email que passam pelo pipeline de transporte.
  
## <a name="transport-agent-class-library"></a>Biblioteca de classes do agente de transporte

Os seguintes namespaces contêm tipos que você pode usar para criar e estender os agentes de transporte.

**Tabela 1. Namespaces do .NET framework**

|**Namespace**|**Descrição**|
|:-----|:-----|
|[Microsoft.Exchange.Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contém os tipos que especificam exceções de dados e a configuração.  <br/> |
|[Microsoft.Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contém os tipos que oferecem suporte a localização e tratamento de erros.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contém os tipos que permitem que você possa ler e gravar dados iCalendar.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contém os tipos que permitem que você possa ler e gravar dados TNEF.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contém os tipos que permitem que você possa ler e gravar dados vCard.  <br/> |
|[Microsoft.Exchange.Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contém os tipos que permitem que você trabalhe com culturas e caractere conjuntos para produzir o conteúdo localizado.  <br/> |
|[Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contém os tipos que permitem que você possa ler e gravar dados MIME.  <br/> |
|[Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contém os tipos que permitem codificar e decodificar dados MIME.  <br/> |
|[Microsoft.Exchange.Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contém os tipos que permitem que você possa ler e gravar dados com diferentes formatos de texto e converter os dados de e para empregar esses formatos.  <br/> |
|[Microsoft.Exchange.Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contém os tipos que permitem que você acesse o roteamento, host e informações sobre o pipeline de transporte de domínio.  <br/> |
|[Deliveryhttp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contém os tipos que oferecem suporte a extensão dos agentes de entrega do Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contém os tipos que oferecem suporte a criação, leitura, gravação e modificando mensagens de email.  <br/> |
|[Microsoft.Exchange.Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contém os tipos que oferecem suporte a extensão do comportamento de roteamento de transporte do Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contém os tipos que oferecem suporte a extensão do comportamento de SMTP de transporte do Exchange 2013.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)   
- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- [Referência de API do servidor do Exchange](http://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

