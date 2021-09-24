---
title: Estrutura CChkSGFiles.PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: f324ec9aca6f94911041c227ce039139292a10aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516255"
---
# <a name="cchksgfilespage_info-struct"></a>Estrutura CChkSGFiles.PAGE_INFO

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Contém informações para uma página Exchange banco de dados. Essa estrutura é usada com a **função ErrCheckDbPages.** 
  
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

## <a name="members"></a>Members

### <a name="ulpgno"></a>ulPgNo
  
Long não assinado. Número de página lógica da página do banco de dados a ser verificada. Esse valor deve ser definido antes de **chamar ErrCheckDbPages**. Se o aplicativo estiver lendo o arquivo com base em deslocamentos de arquivo e, portanto, deve mapear esses deslocamentos de arquivo para números de página lógicas, você encontrará o **método PgnoFromFileOffset** útil para determinar o valor desse campo. **ErrCheckDbPages** não modifica esse valor. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Boolean. Um valor TRUE indica que a página do banco de dados contém dados. Um valor FALSE indica que a página contém apenas zeros. **ErrCheckDbPages** define esse valor. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Boolean. Um valor TRUE indica que houve uma incompatibilidade de verificação detectada na página do banco de dados, mas que é um erro corrigível. **ErrCheckDbPages** define esse valor. 
    
### <a name="checksumactual"></a>checksumActual
  
Inteiro de 64 bits não assinado. Indica o valor de checksum armazenado no banco de dados para esta página lógica. **ErrCheckDbPages** define esse valor. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Inteiro de 64 bits não assinado. Esse é o valor de verificação esperado calculado para a página de banco de dados; é definido por **ErrCheckDbPages**. Se esse valor for diferente do armazenado na página do banco de dados (ou seja, o valor retornado em **checksumActual**), **ErrCheckDbPages** indicará que um erro foi encontrado nesta página de banco de dados. 
    
### <a name="dbtime"></a>dbTime
  
Inteiro de 64 bits não assinado. **ErrCheckDbPages** define esse membro como o data/hora na página do banco de dados. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Inteiro de 64 bt não assinados. **ErrCheckDbPages** define esse membro como o valor de checksum calculado do conteúdo da página que exclui dados desnecessários ao determinar a equivalência de página lógica. Por exemplo, não é necessário considerar os valores de dados no espaço de página do banco de dados nãoutilado. Esse membro só será válido se **os valores checksumActual**  e  **checksumExpected**  são iguais uns aos outros. 
    
### <a name="ulflags"></a>ulFlags
  
Inteiro de 64 bits não assinado. Reserved for future use. O valor deste campo deve ser definido como 0 (zero) antes de chamar **ErrCheckDbPages**.
    
## <a name="remarks"></a>Comentários

Ao chamar a **função ErrCheckDbPages,** o **parâmetro rgPageInfo** é uma matriz de **estruturas PAGE \_ INFO.** Deve haver uma estrutura **DE \_ INFORMAÇÕES de PÁGINA** para cada página do banco de dados a ser verificada. 
  
O aplicativo deve definir o **membro ulPgno**  como o valor adequado e também deve definir o membro  **ulFlags**  como 0 (zero) antes de chamar **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Requisitos

Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

