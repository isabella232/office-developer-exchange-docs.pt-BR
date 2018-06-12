---
title: EWS no Exchange e anexos
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Saiba mais sobre como sua API gerenciada de EWS ou EWS no Exchange client representa-los e anexos.
ms.openlocfilehash: e4a97873798b8252e6fc14003519ce8a0eab7ec8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750647"
---
# <a name="attachments-and-ews-in-exchange"></a>EWS no Exchange e anexos

Saiba mais sobre como sua API gerenciada de EWS ou EWS no Exchange client representa-los e anexos.
  
Geralmente, os anexos estão associados a itens de email, mas na verdade, todos os itens do EWS — mensagens, itens de calendário, contatos, tarefas de email — pode incluir anexos.
  
## <a name="types-of-attachments"></a>Tipos de anexos

EWS categoriza anexos em dois grupos: anexos de item e anexos de arquivo.
  
- **Item anexos:** Fortemente tipadas [itens EWS](folders-and-items-in-ews-in-exchange.md), como mensagens de email e itens de calendário, que estejam anexados a outro item do EWS fortemente tipadas. Qualquer item fortemente tipadas que pode ser criado usando o EWS Managed API ou o EWS pode ser usado como um anexo do item. O conteúdo de um anexo do item é o item fortemente tipadas, que fornece acesso fácil a todas as suas propriedades. Anexos de item podem ter seus próprios anexos de item, portanto, uma hierarquia de anexos de item (ou aninhamento de anexos) é possível.
    
- **Anexos de arquivo:** Qualquer arquivo, como. txt,. jpg,. zip,. PDF, ou até mesmo um arquivo. msg. Um anexo de arquivo tem apenas algumas propriedades, uma delas é o conteúdo do arquivo codificado base 64. 
    
- **Referência anexos:** Qualquer anexo que é referenciado por um provedor de arquivo, como um arquivo localizado na nuvem. Um anexo pode ter entre vários provedores. 
    
Quando você adiciona ou recuperar anexos de um item, você vai fazer forma diferente dependendo se é um anexo de arquivo ou item. Por exemplo, para adicionar um anexo de arquivo a um item, você pode apenas passar no local do arquivo. Para adicionar um item existente como um anexo do item, você realmente precisa copie as propriedades ou o conteúdo MIME do item existente para um novo anexo do item; Você não pode vincular-se apenas ao item existente. É importante tão distinguir entre os dois tipos de anexos. Para obter mais detalhes sobre as diferenças entre os anexos de item e anexos de arquivo são abordadas nos artigos [nesta seção](#bk_inthissection).
  
## <a name="how-are-attachments-represented-programmatically"></a>Como são anexos representados programaticamente?

Anexos são armazenados em uma coleção no item EWS. Coleção attachments é formada pelo anexos de arquivo e/ou anexos do item. Metadados sobre a coleção de anexos estão disponíveis quando você obter um item usando o método API gerenciada de EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou a operação de EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , mas chamadas adicionais são necessários para recuperar o conteúdo dos anexos. 
  
**Tabela 1. Metadados de item sobre anexos**

|**Entidade de metadados**|**Propriedade API gerenciada de EWS**|**Elemento EWS**|
|:-----|:-----|:-----|
|Indicador de anexo (não sinalizará anexos embutidos)  <br/> |[Item.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Coleção de anexos  <br/> |[Item.Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Anexos](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|ID do anexo  <br/> |[Attachment.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**Tabela 2. Entidades de anexo**

|**Tipo de anexo**|**Classe de API gerenciada de EWS**|**Elemento EWS**|
|:-----|:-----|:-----|
|Anexo de arquivo  <br/> |[FileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Anexo do item  <br/> |[ItemAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](http://msdn.microsoft.com/en-us/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Anexo de referência  <br/> |[ReferenceAttachmentType complexType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Anexos embutidos

Anexos embutidos são um melhores especial de anexo. Ambos os anexos de arquivo e anexos de item podem ser anexos embutidos. Um anexo em linha aparece como parte do conteúdo do corpo e mantém sua posição em relação ao restante do conteúdo no item. 
  
Um anexo é um anexo em linha, se a propriedade de API gerenciada de EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) ou o elemento do EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) for definido como true. Anexos embutidos usam os elementos e as seguintes propriedades opcionais para identificar o local de um anexo em linha: 
  
- API gerenciada de EWS — [ContentId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) ou [ContentLocation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) propriedades. 
    
- EWS — Elemento [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) ou [ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) . 
    
Observe que a propriedade de API gerenciada de EWS [HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) e o elemento do EWS [HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) não refletem a existência dos anexos embutidos e que tem por que anexos embutidos também são chamados oculto anexos. Portanto, se você definir a propriedade de API gerenciada de EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) ou o elemento do EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) como true e o item não tem nenhuma outros anexos, **HasAttachments** será definida como false. Se seu cliente usa **HasAttachments** para preencher um indicador de anexo ou um ícone em um email, lembre-se de que o ícone não aparecerá para e-mails com anexos embutidos. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Adicionar anexos usando o EWS no Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Obter anexos usando o EWS no Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Excluir anexos usando o EWS no Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também
<a name="bk_additionalresources"> </a>

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    

