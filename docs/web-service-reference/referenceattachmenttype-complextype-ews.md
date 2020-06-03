---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: 24f5a62eadd490b5b0000dfe048850c44540f266
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528731"
---
# <a name="referenceattachmenttype-complextype-ews"></a>ReferenceAttachmentType complexType (EWS)

## <a name="type-information"></a>Informação de tipo

|||
|:-----|:-----|
|**Namespace** <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|**Arquivo de esquema** <br/> |Types. xsd  <br/> |
|**Base da extensão** <br/> |t:AttachmentType  <br/> |
   
## <a name="definition"></a>Definição

```XML
<xs:complexType name="ReferenceAttachmentType">
    <xs:complexContent>
        <xs:extension base="t:AttachmentType">
            <xs:sequence>
                <xs:element name="AttachLongPathName" type="xs:string" maxOccurs="1" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>

```

## <a name="elements-and-attributes"></a>Elementos e atributos

Se o esquema definir requisitos específicos, como **sequence**, **minOccurs**,**maxOccurs** e **choice**, confira a seção de definição. 
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|[AttachLongPathName](attachlongpathname.md) <br/> |xs:string  <br/> ||
   
### <a name="attributes"></a>Atributos

Nenhum
  

