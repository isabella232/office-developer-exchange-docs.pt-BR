---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: O elemento de QueryString contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824943"
---
# <a name="querystring-querystringtype"></a>QueryString (QueryStringType)

O elemento de **QueryString** contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS). 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|ResetCache  <br/> |Indica que o cache deve ser redefinido.  <br/> |
|ReturnDeletedItems  <br/> |Indica que os itens excluídos devem ser retornados.  <br/> |
|ReturnHighlightTerms  <br/> |Indica que os termos realçados devem ser retornados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> A seguir é a expressão XPath para esse elemento: /FindItem.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **QueryString** representa uma consulta de caixa de correio que será feita usando um subconjunto da [Sintaxe de consulta avançada (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Consulte a seção de comentários para obter informações sobre as opções de sintaxe com suporte para cadeias de caracteres de consulta.
  
## <a name="remarks"></a>Comentários

No Exchange Server 2010, esse elemento é um tipo de cadeia de caracteres de esquema XML. Nas versões do Exchange, começando com o Exchange Server 2013, incluindo o Exchange Online, o tipo deste elemento é **QueryStringType**. Essa alteração não quebrará quaisquer clientes existentes, pois adiciona três novos atributos opcionais. 
  
O elemento **QueryString** exclui o uso das restrições do EWS. AQS no EWS oferece suporte a três tipos de restrições: restrição de fase, a restrição de intervalo de data e a restrição de tipo de mensagem do word. As tabelas a seguir listam as propriedades de pesquisa com suporte para cada tipo de restrição. 
  
**Restrição de fase do Word**

|**Property**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|from  <br/> |De: Dean  <br/> De: "Dean Halstead"  <br/> |Pesquisar os itens enviados do Dean.  <br/> Pesquisar os itens enviados do Dean Halstead. O remetente deve ser exatamente "Dean Halstead".  <br/> |
|para  <br/> |Como: Dean  <br/> |Pesquisar os itens enviados para Dean.  <br/> |
|cc  <br/> |Cc:Dean  <br/> |Procurar itens com Dean na linha Cc.  <br/> |
|bcc  <br/> |BCC:Dean  <br/> |Procurar itens com Dean na linha Cco.  <br/> |
|Participantes  <br/> |Participantes: Dean  <br/> |Pesquisar itens com Dean para, Cc ou Cco, campos.  <br/> |
|Assunto  <br/> |Assunto: produto  <br/> Assunto:(product development)  <br/> Assunto: "desenvolvimento do produto"  <br/> |Procurar itens com o produto no assunto.  <br/> Procurar itens com o produto e desenvolvimento no assunto.  <br/> |
|Body  <br/> Conteúdo  <br/> |Corpo: progresso  <br/> Progresso de conteúdo:  <br/> |Procurar itens cujo andamento no corpo.  <br/> |
|Anexo  <br/> |Anexo: relatório  <br/> |Procurar itens com o relatório no corpo de arquivo ou nome de arquivo do anexo.  <br/> |
|(a propriedade não for especificada)  <br/> |Desenvolvimento do produto  <br/> |Procurar itens que contenham o produto e desenvolvimento em todas as propriedades de fase do word.  <br/> |
   
Correspondência de restrição do Word fase sempre diferencia maiusculas de minúsculas. Restrição de fase do Word suporta dois tipos de correspondência: correspondência de prefixo ou correspondência exata. Correspondência de prefixo é o comportamento padrão de correspondência. Se você quiser correspondência exata, use aspas duplas. Por exemplo, subject: corresponde a "product" 'produto', mas não 'produção' no assunto. Várias palavras em aspas duplas restringem fases do word e sua ordem. Por exemplo "win produto" corresponde a única 'win produto', não 'win95 produto' ou 'produto do win'. Você pode usar um asterisco (\*) para definir uma correspondência de prefixo com ordem restringido. Por exemplo, "win produto"\* corresponde 'win95 produto', 'linha de produção do windows', mas não 'windows novo produto' ou 'produto do win'. Você pode pesquisar todas as mensagens enviadas de ou para um domínio. Por exemplo, from:"@hotmail.com" retorna todas as mensagens enviadas de hotmail.com.
  
A tabela a seguir descreve as restrições de intervalo de data.
  
**Restrição de intervalo de data**

|**Property**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|Enviado  <br/> |Enviados: última semana  <br/> Enviados: 01/01/2001  <br/> Sent:01/01/2001..01/15/2001  <br/> |Pesquisar itens enviados a última semana.  <br/> Pesquisar os itens enviados em 1º de janeiro de 2001.  <br/> Pesquisar os itens enviados entre 1º de janeiro de 2001 e 15 de janeiro de 2001.  <br/> |
|Received  <br/> |Recebidos: hoje  <br/> Recebidos: 01/01/2001  <br/> |Pesquisar os itens recebidas hoje.  <br/> Pesquisar itens recebidos em 1º de janeiro de 2001.  <br/> |
   
Os dois pontos (.) é um operador de intervalo. Ele pode ser usado para definir um intervalo com um início e uma data de término. Para especificar uma data, você pode usar datas relativas. Há suporte para as seguintes datas relativas:
  
- Datas relativas: hoje, amanhã, ontem
    
- Datas relativas multiword: esta semana, mês seguinte, última semana, passou do mês ou ano seguinte
    
- Dias: Domingo, segunda-feira, terça-feira, quarta-feira, quinta-feira, sexta-feira, sábado
    
- Janeiro, fevereiro e março, abril, maio, junho, julho, agosto, setembro, outubro, novembro, dezembro
    
A tabela a seguir descreve as restrições de tipo de mensagem. 
  
**Restrição de tipo de mensagem**

|**Property**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|Tipo  <br/> |Tipo: tarefas  <br/> |Pesquise todos os itens de tarefa.  <br/> |
   
AQS no EWS usa a propriedade **Kind** para especificar o tipo de mensagem. A propriedade Kind pode ser usada com os seguintes tipos de item: 
  
- email
    
- reuniões
    
- tarefas
    
- Observações
    
- documentos
    
- diários
    
- contatos
    
- mensagens instantâneas
    
A tabela a seguir descreve o agrupamento lógicos conectores.
  
**Conectores de lógica de agrupamento**

|**Conector**|**Exemplo**|**Function**|
|:-----|:-----|:-----|
|E  <br/> |Assunto: produto e assunto: desenvolvimento  <br/> Assunto:(product AND development)  <br/> Assunto:(product development)  <br/> |Pesquisar os itens com o produto e desenvolvimento no assunto.  <br/> |
|OU  <br/> |Corpo: projeto ou corpo: proposta  <br/> Corpo:(project OR proposal)  <br/> |Pesquisar os itens com o produto ou desenvolvimento no corpo.  <br/> |
|NÃO  <br/> |NÃO corpo: proposta  <br/> Corpo:(NOT proposal)  <br/> |Pesquisar mensagens sem proposta no corpo.  <br/> |
   
E é sempre o conector padrão. Por exemplo, o assunto: projeto e corpo: proposta é o mesmo assunto: project corpo: proposta. Conectores lógicas diferenciam maiusculas de minúsculas. Por exemplo, do corpo:(project Or proposal) procura mensagens com 'projeto', 'ou' e proposta no corpo, em vez de 'projeto' ou 'proposta'. O símbolo de adição (+) é equivalente à and. O símbolo de hífen (-) é equivalente à não. Por exemplo, do corpo:(project-proposal) procura mensagens com 'projeto', mas sem 'proposta' no corpo. 
  
A cadeia de caracteres de consulta também pode conter as propriedades não-indexadas para pesquisa. Se a cadeia de caracteres de consulta contém propriedades não-indexadas, a pesquisa pode executar uma pesquisa do Exchange sobre as propriedades indexadas e uma pesquisa de repositório de propriedades não-indexado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação para pesquisar mensagens na caixa de entrada com a descoberta automática no assunto.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)
  
[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

