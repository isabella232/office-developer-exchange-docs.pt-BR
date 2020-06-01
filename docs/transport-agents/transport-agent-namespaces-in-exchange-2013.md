---
title: Namespaces do agente de transporte no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Saiba mais sobre as classes e membros do .NET Framework que você pode usar para criar agentes de transporte personalizados para o Exchange 2013.
ms.openlocfilehash: fc2d9108c910a730bb48c5be028797f0f15ad4ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461790"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Namespaces do agente de transporte no Exchange 2013

Saiba mais sobre as classes e membros do .NET Framework que você pode usar para criar agentes de transporte personalizados para o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os namespaces que contêm informações de referência que você pode usar para criar agentes de transporte para o Exchange Server 2013. Também descreve as classes que seus agentes de transporte podem usar para ler e modificar mensagens de email que passam pelo pipeline de transporte.
  
## <a name="transport-agent-class-library"></a>Biblioteca de classes de agente de transporte

Os namespaces a seguir contêm tipos que você pode usar para criar e estender agentes de transporte.

**Tabela 1. Namespaces do .NET Framework**

|**Namespace**|**Descrição**|
|:-----|:-----|
|[Microsoft. Exchange. Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contém tipos que especificam exceções de dados e de configuração.  <br/> |
|[Microsoft. Exchange. Data. Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contém tipos que dão suporte à localização e tratamento de erros.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contém tipos que permitem que você leia e grave dados do iCalendar.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. TNEF](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contém tipos que permitem que você leia e grave dados TNEF.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contém tipos que permitem que você leia e grave dados de vCard.  <br/> |
|[Microsoft. Exchange. Data. Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contém tipos que permitem que você trabalhe com culturas e conjuntos de caracteres para produzir conteúdo localizado.  <br/> |
|[Microsoft. Exchange. Data. MIME](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contém tipos que permitem que você leia e grave dados MIME.  <br/> |
|[Microsoft. Exchange. Data. MIME. decodificadores](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contém tipos que permitem codificar e decodificar dados MIME.  <br/> |
|[Conversores Microsoft. Exchange. Data.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contém tipos que permitem que você leia e grave dados com formatos de texto diferentes e converta os dados nesses formatos.  <br/> |
|[Microsoft. Exchange. Data. Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contém tipos que permitem acessar informações de roteamento, host e domínio sobre o pipeline de transporte.  <br/> |
|[Microsoft. Exchange. Data. Transport. Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contém tipos que oferecem suporte à extensão de agentes de entrega do Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. Transport. email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contém tipos que oferecem suporte à criação, leitura, gravação e modificação de mensagens de email.  <br/> |
|[Microsoft. Exchange. Data. Transport. Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contém tipos que oferecem suporte à extensão do comportamento de roteamento de transporte do Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. Transport. SMTP](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contém tipos que oferecem suporte à extensão do comportamento SMTP de transporte do Exchange 2013.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)   
- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Referência de API de servidor para Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

