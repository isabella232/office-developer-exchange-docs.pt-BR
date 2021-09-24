---
title: Namespaces do agente de transporte Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Saiba mais sobre as .NET Framework e membros que você pode usar para criar agentes de transporte personalizados para Exchange 2013.
ms.openlocfilehash: 076ddb8e2ccbdfa195a68aca6b296337a2876b55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537127"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Namespaces do agente de transporte Exchange 2013

Saiba mais sobre as .NET Framework e membros que você pode usar para criar agentes de transporte personalizados para Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os namespaces que contêm informações de referência que você pode usar para criar agentes de transporte para Exchange Server 2013. Ele também descreve as classes que seus agentes de transporte podem usar para ler e modificar mensagens de email que passam pelo pipeline de transporte.
  
## <a name="transport-agent-class-library"></a>Biblioteca de classes de agente de transporte

Os namespaces a seguir contêm tipos que você pode usar para criar e estender agentes de transporte.

**Tabela 1. .NET Framework namespaces**

|**Namespace**|**Descrição**|
|:-----|:-----|
|[Microsoft. Exchange. Dados](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contém tipos que especificam exceções de dados e configuração.  <br/> |
|[Microsoft. Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contém tipos que suportam a localização e o tratamento de erros.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contém tipos que permitem ler e gravar dados iCalendar.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contém tipos que permitem que você leia e escreva dados TNEF.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contém tipos que permitem ler e gravar dados vCard.  <br/> |
|[Microsoft. Exchange. Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contém tipos que permitem que você trabalhe com culturas e conjuntos de caracteres para produzir conteúdo localizado.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contém tipos que permitem que você leia e escreva dados MIME.  <br/> |
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contém tipos que permitem codificar e decodificar dados MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contém tipos que permitem ler e gravar dados com diferentes formatos de texto e converter dados para e para esses formatos.  <br/> |
|[Microsoft. Exchange. Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contém tipos que permitem que você acesse informações de roteamento, host e domínio sobre o pipeline de transporte.  <br/> |
|[Microsoft. Exchange. Data.Transport.Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contém tipos que suportam a extensão de Exchange de entrega 2013.  <br/> |
|[Microsoft. Exchange. Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contém tipos que suportam a criação, leitura, escrita e modificação de mensagens de email.  <br/> |
|[Microsoft. Exchange. Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contém tipos que suportam a extensão do comportamento de roteamento de transporte Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contém tipos que suportam a extensão do comportamento SMTP de transporte Exchange 2013.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)   
- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Referência de API de servidor para Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Elementos de arquivo de configuração de agentes para Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

