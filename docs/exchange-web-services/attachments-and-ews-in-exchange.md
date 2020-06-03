---
title: Anexos e EWS no Exchange
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Saiba mais sobre os anexos e como a API gerenciada do EWS ou o EWS no cliente do Exchange os representa.
localization_priority: Priority
ms.openlocfilehash: d37fef9ea14a3b42a0eed0240724fe69c8531c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528486"
---
# <a name="attachments-and-ews-in-exchange"></a>Anexos e EWS no Exchange

Saiba mais sobre os anexos e como a API gerenciada do EWS ou o EWS no cliente do Exchange os representa.
  
Normalmente, os anexos são associados a itens de email, mas, na verdade, todos os itens do EWS — mensagens de email, itens de calendário, contatos, tarefas — podem incluir anexos.
  
## <a name="types-of-attachments"></a>Tipos de anexos

O EWS categoriza os anexos em dois grupos: anexos de arquivo e anexos de item.
  
- **Anexos de item:** [Itens de EWS](folders-and-items-in-ews-in-exchange.md)fortemente tipados, como mensagens de email e itens de calendário, que estão anexados a outro item de EWS de tipo de alta segurança. Qualquer item fortemente tipado que possa ser criado usando a API gerenciada do EWS ou o EWS pode ser usado como um anexo de item. O conteúdo de um anexo de item é o item fortemente tipado, que fornece acesso fácil a todas as suas propriedades. Anexos de item podem ter seus próprios anexos de item, portanto, uma hierarquia de anexos de item (ou aninhamento de anexos) é possível.
    
- **Anexos de arquivo:** Qualquer arquivo, como. txt,. jpg,. zip,. pdf ou até mesmo um arquivo. msg. Um anexo de arquivo tem apenas algumas propriedades, uma das quais é o conteúdo codificado em base 64 do arquivo. 
    
- **Anexos de referência:** Qualquer anexo que é referenciado por um provedor de arquivos, como um arquivo localizado na nuvem. Um anexo pode ser de vários provedores. 
    
Ao adicionar ou recuperar anexos de um item, você fará isso de forma diferente, dependendo se é um anexo de arquivo ou um anexo de item. Por exemplo, para adicionar um anexo de arquivo a um item, você pode apenas passar o local do arquivo. Para adicionar um item existente como um anexo de item, você realmente precisa copiar as propriedades ou o conteúdo MIME do item existente para um novo anexo de item; Você não pode apenas associar ao item existente. Portanto, distinguir entre os dois tipos de anexos é importante. Mais detalhes sobre as diferenças entre anexos de item e anexos de arquivo são discutidos nos artigos [desta seção](#bk_inthissection).
  
## <a name="how-are-attachments-represented-programmatically"></a>Como os anexos são representados programaticamente?

Os anexos são armazenados em uma coleção no item EWS. A coleção Attachments é composta por anexos de arquivo e/ou anexos de item. Os metadados sobre a coleção de anexos estão disponíveis quando você recebe um item usando o item de API gerenciada do EWS. o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou a operação do EWS [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , mas são necessárias chamadas adicionais para recuperar o conteúdo dos anexos. 
  
**Tabela 1. Metadados de item sobre anexos**

|**Entidade de metadados**|**Propriedade da API gerenciada do EWS**|**Elemento do EWS**|
|:-----|:-----|:-----|
|Indicador de anexo (não sinaliza anexos embutidos)  <br/> |[Item. HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](https://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Coleção Attachment  <br/> |[Item. Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Anexos](https://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|ID do anexo  <br/> |[Attachment.Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[Attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**Tabela 2. Entidades de anexo**

|**Tipo de anexo**|**Classe de API gerenciada do EWS**|**Elemento do EWS**|
|:-----|:-----|:-----|
|Anexo de arquivo  <br/> |[FileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](https://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Anexo de item  <br/> |[ItemAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](https://msdn.microsoft.com/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](https://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Anexo de referência  <br/> |[ReferenceAttachmentType complexType (EWS)](https://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](https://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Anexos embutidos

Os anexos embutidos são uma espécie especial de anexo. Os anexos de arquivo e anexos de item podem ser anexos embutidos. Um anexo embutido aparece como parte do conteúdo do corpo e mantém sua posição relativa ao restante do conteúdo do item. 
  
Um anexo é um anexo embutido se a propriedade [IsInline](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) da API gerenciada do EWS ou o elemento [myinline](https://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) do EWS estiver definido como true. Anexos embutidos usam as seguintes propriedades e elementos opcionais para identificar o local de um anexo embutido: 
  
- API gerenciada do EWS — propriedades [ContentId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) ou [ContentLocation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) . 
    
- EWS — elemento [ContentId](https://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) ou [ContentLocation](https://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) . 
    
Observe que a propriedade [HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) da API gerenciada do EWS e o elemento EWS [HasAttachments](https://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) não refletem a existência de anexos embutidos e é por isso que os anexos embutidos também são chamados de anexos ocultos. Portanto, se você definir a propriedade [IsInline](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) da API gerenciada do EWS ou o elemento [IsInline](https://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) do EWS como true e o item não tiver outros anexos, **HasAttachments** será definido como false. Se o cliente usar **HasAttachments** para preencher um indicador ou ícone de anexo em um email, lembre-se de que o ícone não aparecerá para emails com anexos embutidos. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Adicionar anexos usando o EWS no Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Obter anexos usando o EWS no Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Excluir anexos usando EWS no Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também
<a name="bk_additionalresources"> </a>

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    

