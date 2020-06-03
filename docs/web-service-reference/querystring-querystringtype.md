---
title: QueryString (QueryStringtype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: O elemento QueryString contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459185"
---
# <a name="querystring-querystringtype"></a>QueryString (QueryStringtype)

O elemento **QueryString** contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS). 
  
```XML
<QueryString/>
```

 **QueryStringtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|ResetCache  <br/> |Indica que o cache deve ser redefinido.  <br/> |
|ReturnDeletedItems  <br/> |Indica que os itens excluídos devem ser retornados.  <br/> |
|ReturnHighlightTerms  <br/> |Indica que os termos realçados devem ser retornados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:/FindItem.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **QueryString** representa uma consulta de caixa de correio que é feita usando um subconjunto de [sintaxe de consulta avançada (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). Consulte a seção comentários para obter informações sobre as opções de sintaxe suportadas para cadeias de caracteres de consulta.
  
## <a name="remarks"></a>Comentários

No Exchange Server 2010, esse elemento é um tipo de cadeia de caracteres de esquema XML. Nas versões do Exchange a partir do Exchange Server 2013, incluindo o Exchange Online, o tipo desse elemento é **querystringtype**. Essa alteração não quebra clientes existentes porque adiciona três novos atributos opcionais. 
  
O elemento **QueryString** exclui o uso de restrições do EWS. AQS no EWS dá suporte a três tipos de restrições: restrição de fase de palavra, restrição de intervalo de datas e restrição de tipo de mensagem. As tabelas a seguir listam as propriedades de pesquisa suportadas para cada tipo de restrição. 
  
**Restrição de fase do Word**

|**Propriedade**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|from  <br/> |De: diretora  <br/> De: "Halstead"  <br/> |Itens de pesquisa enviados pelo diretor.  <br/> Itens de pesquisa enviados por Halstead. O remetente deve ser exatamente "Halstead".  <br/> |
|para  <br/> |Para: diretora  <br/> |Itens de pesquisa enviados para a diretora.  <br/> |
|cc  <br/> |CC: diretora  <br/> |Pesquise itens com o diretor na linha CC.  <br/> |
|bcc  <br/> |CCO: diretora  <br/> |Pesquisar itens com a linha de um na linha Cco.  <br/> |
|Participante  <br/> |Participantes: diretora  <br/> |Pesquisar itens com o diretor nos campos para, CC ou Cco.  <br/> |
|Assunto  <br/> |Assunto: produto  <br/> Assunto: (desenvolvimento de produtos)  <br/> Assunto: "desenvolvimento de produtos"  <br/> |Pesquisar itens com o produto no assunto.  <br/> Pesquisar itens com produtos e desenvolvimento no assunto.  <br/> |
|Corpo  <br/> Conteúdo  <br/> |Corpo: Progress  <br/> Conteúdo: progresso  <br/> |Pesquisar itens com progresso no corpo.  <br/> |
|Anexo  <br/> |Anexo: relatório  <br/> |Pesquisar itens com o relatório no nome do arquivo de anexo ou no corpo do arquivo.  <br/> |
|(Propriedade não especificada)  <br/> |Desenvolvimento de produtos  <br/> |Pesquisar itens que contenham produtos e desenvolvimento em todas as propriedades da fase do Word.  <br/> |
   
A correspondência de restrição de fase de palavra sempre diferencia maiúsculas de minúsculas. A restrição de fase do Word dá suporte a dois tipos de correspondência: correspondência de prefixo ou correspondência exata. O prefixo correspondente é o comportamento padrão de correspondência. Se quiser correspondência exata, use aspas duplas. Por exemplo, Subject: "Product" corresponde a "Product", mas não a "Production" no assunto. Várias palavras em aspas duplas restringem ambas as fases da palavra e sua ordem. Por exemplo, "produto de vitória" corresponde somente a "produto Win", não ' produto do Win95 ' ou "produto de vitória". Você pode usar um asterisco ( \* ) para definir uma correspondência de prefixo com ordem restrita. Por exemplo, "produto do Win" corresponde a " \* produto do Win95", "linha de produção do Windows", mas não "novo produto do Windows" ou "produto de vitória". Você pode pesquisar todas as mensagens enviadas de ou para um domínio. Por exemplo, de: "@hotmail. com" retorna todas as mensagens enviadas de hotmail.com.
  
A tabela a seguir descreve as restrições de intervalo de datas.
  
**Restrição de intervalo de datas**

|**Propriedade**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|Sent  <br/> |Enviado: última semana  <br/> Enviado: 01/01/2001  <br/> Enviado: 01/01/2001.. 01/15/2001  <br/> |Itens de pesquisa enviados na semana passada.  <br/> Itens de pesquisa enviados no dia 1º de janeiro de 2001.  <br/> Itens de pesquisa enviados entre 1º de janeiro de 2001 e 15 de janeiro de 2001.  <br/> |
|Received  <br/> |Recebido: hoje  <br/> Recebido: 01/01/2001  <br/> |Itens de pesquisa recebidos hoje.  <br/> Itens de pesquisa recebidos no dia 1º de janeiro de 2001.  <br/> |
   
Os dois pontos (..) são um operador de intervalo. Pode ser usado para definir um intervalo com um início e uma data de término. Para especificar uma data, você pode usar datas relativas. As seguintes datas relativas têm suporte:
  
- Datas relativas: hoje, amanhã, ontem
    
- Datas relativas de MultiWord: esta semana, mês seguinte, semana passada, mês ou ano que vem
    
- Dias: domingo, segunda-feira, terça-feira, quarta-feira, quinta-feira, sábado
    
- Janeiro, fevereiro, março, abril, maio, junho de julho, agosto, setembro, outubro, novembro de dezembro
    
A tabela a seguir descreve as restrições de tipo de mensagem. 
  
**Restrição de tipo de mensagem**

|**Propriedade**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|Tipo  <br/> |Tipo: tarefas  <br/> |Pesquisar todos os itens de tarefa.  <br/> |
   
AQS no EWS usa a propriedade **Kind** para especificar o tipo de mensagem. A propriedade Kind pode ser usada com os seguintes tipos de item: 
  
- email
    
- treinamento
    
- tarefas
    
- notes
    
- docs
    
- diários
    
- contacts
    
- respectiva
    
A tabela a seguir descreve o agrupamento de conectores lógicos.
  
**Agrupando conectores lógicos**

|**Connector**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|E  <br/> |Assunto: produto e assunto: desenvolvimento  <br/> Assunto: (produto e desenvolvimento)  <br/> Assunto: (desenvolvimento de produtos)  <br/> |Pesquisar itens com produtos e desenvolvimento no assunto.  <br/> |
|OU  <br/> |Corpo: projeto ou corpo: proposta  <br/> Corpo: (projeto ou proposta)  <br/> |Pesquisar itens com o produto ou o desenvolvimento no corpo.  <br/> |
|NÃO  <br/> |Não corpo: proposta  <br/> Corpo: (não proposta)  <br/> |Pesquisar mensagens sem proposta no corpo.  <br/> |
   
E é sempre o conector padrão. Por exemplo, Subject: Project e Body: proposta é o mesmo que o assunto: corpo do projeto: proposta. Conectores lógicos diferenciam maiúsculas de minúsculas. Por exemplo, corpo: (projeto ou proposta) pesquisa mensagens com "projeto", "ou" e "proposta" no corpo em vez de "projeto" ou "proposta". O símbolo de adição (+) equivale a e. O símbolo de hífen (-) é equivalente a não. Por exemplo, Body: (Project-propostas) pesquisa mensagens com "Project", mas sem "proposta" no corpo. 
  
A cadeia de caracteres de consulta também pode conter Propriedades não indexadas para pesquisa. Se a cadeia de caracteres de consulta contiver Propriedades não indexadas, a pesquisa poderá realizar uma pesquisa do Exchange nas propriedades indexadas e uma pesquisa de armazenamento nas propriedades não indexadas. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação de pesquisa de mensagens na caixa de entrada com descoberta automática no assunto.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)
  
[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

