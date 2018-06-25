---
title: CChkSGFiles.PAGE_INFO struct
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751569"
---
# <a name="cchksgfilespageinfo-struct"></a>CChkSGFiles.PAGE_INFO struct

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Contém informações para uma página de banco de dados do Exchange. Essa estrutura é usada com a função **ErrCheckDbPages** . 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a>Membros

### <a name="ulpgno"></a>ulPgNo
  
Unsigned Long. Número da página lógica da página banco de dados a ser verificado. Este valor deve ser definido antes de chamar **ErrCheckDbPages**. Se o aplicativo está lendo o arquivo com base em arquivo deslocamentos e, portanto, deve ser mapeados esses deslocamentos de arquivo aos números de página lógicos, você encontrará o método **PgnoFromFileOffset** útil para determinar o valor para esse campo. **ErrCheckDbPages** não modifique esse valor. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Boolean. Um valor TRUE indica que a página de banco de dados contém dados. Um valor FALSE indica que a página contém somente zeros. **ErrCheckDbPages** define esse valor. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Boolean. Um valor TRUE indica que houve uma incompatibilidade de soma de verificação detectada na página banco de dados, mas que é um erro pode ser corrigido. **ErrCheckDbPages** define esse valor. 
    
### <a name="checksumactual"></a>checksumActual
  
Inteiro não assinado de 64 bits. Indica o valor de soma de verificação armazenado no banco de dados para esta página lógica. **ErrCheckDbPages** define esse valor. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Inteiro não assinado de 64 bits. Esse é o valor de soma de verificação esperada é calculado para a página de banco de dados; ele é definido por **ErrCheckDbPages**. Se esse valor é diferente daquele armazenadas na página banco de dados (ou seja, o valor retornado em **checksumActual**), **ErrCheckDbPages** indicará que um erro foi localizado nesta página de banco de dados. 
    
### <a name="dbtime"></a>dbTime
  
Inteiro não assinado de 64 bits. **ErrCheckDbPages** define este membro para o carimbo de hora na página banco de dados. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Inteiro não assinado de 64-bt. **ErrCheckDbPages** define este membro para o valor calculado de soma de verificação do conteúdo da página excluindo dados que é desnecessários ao determinar a equivalência lógica de página. Por exemplo, é desnecessário considerar os valores de dados no espaço de página do banco de dados não utilizados. Este membro só será válido se os valores de **checksumActual** e **checksumExpected** são iguais uns aos outros. 
    
### <a name="ulflags"></a>ulFlags
  
Inteiro não assinado de 64 bits. Reservado para uso futuro. O valor desse campo deve ser definido como 0 (zero) antes de chamar **ErrCheckDbPages**.
    
## <a name="remarks"></a>Comentários

Ao chamar a função **ErrCheckDbPages** , o parâmetro **rgPageInfo** é uma matriz de **página\_INFO** estruturas. Deve haver um **página\_INFO** estrutura para cada página de banco de dados a ser verificado. 
  
O aplicativo deve definir o membro **ulPgno** com o valor apropriado e também deve definir o membro **ulFlags** como 0 (zero) antes de chamar **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Requisitos

Exchange Server 2013 apenas inclui uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

