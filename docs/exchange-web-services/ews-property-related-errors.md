---
title: Erros relacionados a propriedade do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1c4c5969-7bdd-4021-be0e-cae99e86cf2c
description: Descubra como lidar com erros relacionados a propriedade em seu aplicativo do EWS.
ms.openlocfilehash: f214ab40c3717178c6957a9da93bdf89999fc1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750660"
---
# <a name="ews-property-related-errors"></a>Erros relacionados a propriedade do EWS

Descubra como lidar com erros relacionados a propriedade em seu aplicativo do EWS.
  
A maioria dos aplicativos de cliente do EWS usará propriedades, que significa que você terá que lidar com erros relacionados a propriedade. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.
  
**Tabela 1: Erros relacionados a propriedade e como lidar com eles**

|**Erro**|**Causado por uma tentativa de …**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorDataSizeLimitExceeded  <br/> |Definir uma propriedade com um valor que exceda o tamanho máximo da propriedade ou a propriedade não tem suporte para o fluxo de mídia, como as propriedades de pasta.  <br/> |Limitar o tamanho de dados definido na propriedade.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Obtenha uma propriedade que não puderam ser recuperada.  <br/> |Indicando que a propriedade não pode ser recuperada.  <br/> |
|ErrorInvalidExtendedProperty  <br/> |Defina uma combinação de valores de propriedade estendida ou resultados inválida em uma propriedade identificador de recurso uniforme (URI) estendida de inválida.  <br/> |Verificando o valor da propriedade estendida.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Definir um valor da propriedade estendidas que não corresponde ao tipo especificado  <br/> |Atualizando o seu código para verificar se há tipos correspondentes.  <br/> |
|ErrorInvalidFolderId  <br/> |Defina a estrutura de um identificador de pasta para um formulário inválido.  <br/> |Apenas usando identificadores retornado por EWS.  <br/> |
|ErrorInvalidId  <br/> |Definir a estrutura de um identificador e/ou alterar chave para um formato inválido.  <br/> |Apenas usando identificadores retornado por EWS.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Defina um identificador de um vazio.  <br/> |Definindo o identificador com um identificador de item ou de pasta válido.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Definir a estrutura de um identificador e/ou alterar chave para um formato inválido.  <br/> |Apenas usando identificadores retornado por EWS.  <br/> |
|ErrorInvalidPropertyAppend  <br/> |Acrescente uma propriedade que não oferece suporte a anexar.  <br/> |Atualizando o seu código para que ele tenta acrescentar valores para as propriedades da coleção destinatários (para, Cc, Cco), as propriedades de conjunto de participante (obrigatório, opcional, recursos), propriedade Body e a propriedade ReplyTo.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Exclua uma propriedade que não oferece suporte a exclusão.  <br/> |Atualizando o seu código para não tentar excluir a propriedade. Por exemplo, a pasta e os identificadores de item não podem ser excluídos.  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Defina uma restrição de existential de pesquisa com base em uma propriedade de sinalizador.  <br/> |Atualizando o seu código para não usar propriedades com base no sinalizador em uma restrição de pesquisa com base existential. Com base no sinalizador propriedades são IsDraft, IsSubmitted, IsUnmodified, IsResend e IsFromMe.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Atuar em uma propriedade de um item ou a pasta que não é compatível com a operação.  <br/> |Atualizando o seu código para não acessar a propriedade com a operação que causou o erro.  <br/> |
|ErrorInvalidPropertyRequest  <br/> |Especifique uma propriedade na solicitação de que não há suporte para o tipo de item.  <br/> |Atualizando o seu código para não tente acessar a propriedade com a operação.  <br/> |
|ErrorInvalidPropertySet  <br/> |Defina uma propriedade somente leitura.  <br/> |Atualizando o seu código para não tentar definir a propriedade.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Compare um valor de propriedade em uma restrição de pesquisa onde o valor de comparação não coincide com o tipo de propriedade.  <br/> |Atualizando o seu código para verificar se há incompatibilidade de tipo de propriedade.  <br/> |
|ErrorItemSavePropertyError  <br/> |Salve um item ou pasta com valores de propriedade inválido.  <br/> |Verificando os valores de propriedade e tipos antes de enviá-los em uma solicitação.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Defina a classe de pasta em uma nova pasta que não seja o tipo da pasta base.  <br/> |Usando um tipo de pasta genérico para definir a classe de pasta.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Referência a uma propriedade estendida personalizada por marca de sua propriedade.  <br/> |Atualizar seu código para referenciar o sinalizador estendido identificador de conjunto de propriedade por propriedade e o nome da propriedade ou identificador de expedição de propriedade.  <br/> |
|ErrorObjectTypeChanged  <br/> |Definir ou atualizar a classe de item em um item que não corresponda com seu tipo de esquema.  <br/> |Atualizando o seu código para que o item classe corresponde ao tipo de esquema do item.  <br/> |
|ErrorPropertyUpdate  <br/> |Atualize uma propriedade com um valor de propriedade inválido.  <br/> |Verificando o valor da propriedade antes de enviá-la em uma solicitação de [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) .  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Envie uma solicitação de CreateAttachment que está faltando uma propriedade necessária.  <br/> |Atualizando o seu código para definir a propriedade ausente conforme especificado pelo caminho de propriedade retornado na resposta.  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Use a propriedade estendida tipos de objeto do tipo, matriz de objeto, erro ou nulo.  <br/> |Atualizando o código para não usar os tipos de propriedade estendida restritos.  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Use um caminho de propriedade não suportado em uma restrição de pesquisa.  <br/> |Alterando a restrição de pesquisa para excluir o caminho de propriedade não suportado.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Use um caminho de propriedade não suportado em uma solicitação de pesquisa classificados ou agrupada.  <br/> |Alterando a restrição de pesquisa para excluir o caminho de propriedade não suportado.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Solicite um tipo de propriedade que não pode ser convertido para XML para o EWS retornar em uma resposta.  <br/> |Atualizando o seu código para não solicitar a propriedade sem suporte.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Atualize um item ou pasta para a descrição de alteração para o qual não corresponde à propriedade que é especificada para ser atualizado.  <br/> |Alterando seu código para que a descrição da alteração corresponde ao tipo de item ou a pasta que está sendo atualizado.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Propriedades e as propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

