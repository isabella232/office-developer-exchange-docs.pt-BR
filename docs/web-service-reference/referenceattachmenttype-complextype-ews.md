---
title: ReferenceAttachmentType complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: da9ff2b73f86bba3003c31dec009ea11a9b26b32
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825030"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="a5a6a-102">ReferenceAttachmentType complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="a5a6a-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="a5a6a-103">Informações de tipo</span><span class="sxs-lookup"><span data-stu-id="a5a6a-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5a6a-104">**Namespace**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5a6a-105">**Arquivo de esquema**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-105">**Schema file**</span></span> <br/> |<span data-ttu-id="a5a6a-106">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a5a6a-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5a6a-107">**Extensão de base**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-107">**Extension base**</span></span> <br/> |<span data-ttu-id="a5a6a-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="a5a6a-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="a5a6a-109">Definição</span><span class="sxs-lookup"><span data-stu-id="a5a6a-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="a5a6a-110">Elementos e atributos</span><span class="sxs-lookup"><span data-stu-id="a5a6a-110">Elements and attributes</span></span>

<span data-ttu-id="a5a6a-111">Se o esquema define os requisitos específicos, como a **sequência**, **minOccurs**, **maxOccurs**e **Escolha**, consulte a seção de definição.</span><span class="sxs-lookup"><span data-stu-id="a5a6a-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="a5a6a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a5a6a-112">Child elements</span></span>

|<span data-ttu-id="a5a6a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-113">**Element**</span></span>|<span data-ttu-id="a5a6a-114">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-114">**Type**</span></span>|<span data-ttu-id="a5a6a-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a5a6a-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="a5a6a-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="a5a6a-116">AttachLongPathName</span></span>](http://msdn.microsoft.com/library/98464422-2c13-8d33-0fe3-b1978f2d5b4a%28Office.15%29.aspx) <br/> |<span data-ttu-id="a5a6a-117">xs: String</span><span class="sxs-lookup"><span data-stu-id="a5a6a-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="a5a6a-118">Atributos</span><span class="sxs-lookup"><span data-stu-id="a5a6a-118">Attributes</span></span>

<span data-ttu-id="a5a6a-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5a6a-119">None.</span></span>
  

