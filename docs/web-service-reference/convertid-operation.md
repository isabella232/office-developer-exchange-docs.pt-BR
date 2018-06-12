---
title: Operação ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Encontre informações sobre o EWS ConvertId operação.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751536"
---
# <a name="convertid-operation"></a><span data-ttu-id="ae9ec-103">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-103">ConvertId operation</span></span>

<span data-ttu-id="ae9ec-104">Encontre informações sobre a operação de EWS **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="ae9ec-105">A operação de serviços Web do Exchange (EWS) **ConvertId** converte identificadores de item e pasta entre formatos que são aceitos pelo Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange Server no local 2013.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="ae9ec-106">Usando a operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-106">Using the ConvertId operation</span></span>
<span data-ttu-id="ae9ec-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-107"></span></span>

<span data-ttu-id="ae9ec-108">Você pode converter os seguintes identificadores usando a operação **ConvertId** :</span><span class="sxs-lookup"><span data-stu-id="ae9ec-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="ae9ec-109">O formato do identificador de EWS na versão inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="ae9ec-110">Isso é representado pelo `EwsLegacyId` valor de enumeração na enumeração [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="ae9ec-111">O formato do identificador de EWS no Exchange 2007 SP1 ou Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="ae9ec-112">Isso é representado pelo `EwsId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ae9ec-112">This is represented by the  `EwsId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="ae9ec-113">O identificador MAPI, como a propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="ae9ec-114">Isso é representado pelo `EntryId` valor de enumeração na enumeração [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="ae9ec-115">O identificador de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-115">The availability calendar event identifier.</span></span> <span data-ttu-id="ae9ec-116">Esta é uma representação hexadecimal codificado da propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="ae9ec-117">Isso é representado pelo `HexEntryId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ae9ec-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="ae9ec-118">O identificador de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-118">The Exchange store identifier.</span></span> <span data-ttu-id="ae9ec-119">Isso é representado pelo `StoreId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ae9ec-119">This is represented by the  `StoreId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="ae9ec-120">A operação **ConvertId** não converte os identificadores de pasta pública do identificador EWS para o identificador do repositório.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="ae9ec-121">O identificador do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="ae9ec-122">Isso é representado pelo `OwaId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae9ec-122">This is represented by the  `OwaId` enumeration value in [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="ae9ec-123">Não há suporte para a passagem de URLs que são criados a partir esse identificador para o Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="ae9ec-124">O identificador do Outlook Web App é aplicável para o Exchange 2007 e Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="ae9ec-125">Outlook Web App para Exchange Online e versões do Exchange, começando com o Exchange Server 2013 usa identificadores EWS.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="ae9ec-126">A operação **ConvertId** não funciona conforme o esperado, ao converter identificadores de pasta pública o identificador do EWS para o identificador de repositório no Exchange Online e Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="ae9ec-127">Você pode atualizar manualmente o identificador retornado como uma solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="ae9ec-128">Para atualizar manualmente o identificador:</span><span class="sxs-lookup"><span data-stu-id="ae9ec-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="ae9ec-129">Em seu código de aplicativo, determine se o item/pasta de destino está em uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="ae9ec-130">Decodificar a sequência identifier codificado na Base64.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="ae9ec-131">Verificar se o byte tipo (21 de byte) tem o valor 7.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="ae9ec-132">O valor 7 indica que o identificador está no formato incorreto.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="ae9ec-133">Ignore os primeiros quatro bytes.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-133">Skip the first four bytes.</span></span> <span data-ttu-id="ae9ec-134">Eles devem ser definidos como zero.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="ae9ec-135">Atualizar o próximo de 16 bytes com a seguinte GUID: 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="ae9ec-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="ae9ec-136">Atualize o próximo byte (tipo byte) com um valor de 9.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="ae9ec-137">Altere o identificador para uma cadeia de caracteres codificado na Base64.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="ae9ec-138">A operação **ConvertId** valida que um determinado endereço SMTP tem um formato válido.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="ae9ec-139">A operação não determinará se um endereço SMTP representa uma caixa de correio válida.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="ae9ec-140">A operação **ConvertId** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="ae9ec-141">**Tabela 1. Cabeçalhos SOAP ConvertId operação**</span><span class="sxs-lookup"><span data-stu-id="ae9ec-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="ae9ec-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="ae9ec-142">**Header**</span></span>|<span data-ttu-id="ae9ec-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae9ec-143">**Element**</span></span>|<span data-ttu-id="ae9ec-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae9ec-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ae9ec-145">Representação</span><span class="sxs-lookup"><span data-stu-id="ae9ec-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="ae9ec-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ae9ec-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ae9ec-147">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="ae9ec-148">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ae9ec-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ae9ec-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ae9ec-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ae9ec-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ae9ec-151">Identifica a versão do esquema para a solicitação de operação, que isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ae9ec-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ae9ec-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ae9ec-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ae9ec-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ae9ec-154">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ae9ec-155">Isso é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="ae9ec-156">Exemplo de solicitação de operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-156">ConvertId operation request example</span></span>
<span data-ttu-id="ae9ec-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-157"></span></span>

<span data-ttu-id="ae9ec-158">O exemplo a seguir de uma solicitação de **ConvertId** mostra como converter a partir de um identificador do EWS e um identificador do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="ae9ec-159">O elemento [RequestServerVersion](requestserverversion.md) no cabeçalho SOAP deve ser definido como Exchange2007_SP1 ou posterior para esta operação trabalhar.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ae9ec-160">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-160">The item identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a><span data-ttu-id="ae9ec-161">Exemplo de resposta da operação de ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-161">ConvertId operation response example</span></span>
<span data-ttu-id="ae9ec-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-162"></span></span>

<span data-ttu-id="ae9ec-163">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="ae9ec-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="ae9ec-164">Este exemplo resposta contém um identificador do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ae9ec-165">O identificador do Outlook Web App foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="ae9ec-166">Exemplo de resposta de erro de operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-166">ConvertId operation error response example</span></span>
<span data-ttu-id="ae9ec-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-167"></span></span>

<span data-ttu-id="ae9ec-168">O exemplo a seguir mostra a resposta a uma solicitação que contém o tipo de formato de identificador incorreto.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="ae9ec-169">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="ae9ec-169">Version differences</span></span>
<span data-ttu-id="ae9ec-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-170"></span></span>

<span data-ttu-id="ae9ec-171">O formato de identificador do EWS alterado entre a versão de lançamento inicial do Exchange 2007 e Exchange 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ae9ec-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="ae9ec-172">Exchange Online como parte do Office 365, Exchange Online e a versões locais do Exchange, começando com o Exchange 2010 usam o mesmo formato de identificador que usa o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="ae9ec-173">A operação **ConvertId** converte os identificadores de pasta pública do identificador do EWS para o identificador de repositório no Exchange 2007 e Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="ae9ec-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ae9ec-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="ae9ec-174">See also</span></span>
<span data-ttu-id="ae9ec-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="ae9ec-175"></span></span>

- [<span data-ttu-id="ae9ec-176">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="ae9ec-176">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="ae9ec-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="ae9ec-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="ae9ec-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ae9ec-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

