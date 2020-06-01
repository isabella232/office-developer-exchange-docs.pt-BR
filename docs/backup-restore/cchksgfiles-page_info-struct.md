---
title: Struct função cchksgfiles. PAGE_INFO
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456336"
---
# <a name="cchksgfilespage_info-struct"></a>Struct função cchksgfiles. PAGE_INFO

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Armazena informações de uma página de banco de dados do Exchange. Essa estrutura é usada com a função **ErrCheckDbPages** . 
  
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
  
Longo não assinado. Número de página lógica da página do banco de dados a ser verificado. Esse valor deve ser definido antes de chamar **ErrCheckDbPages**. Se o aplicativo estiver lendo o arquivo com base nos deslocamentos de arquivo e, portanto, mapear esses deslocamentos de arquivo para números de página lógicos, você encontrará o método **PgnoFromFileOffset** útil para determinar o valor desse campo. **ErrCheckDbPages** não modifica esse valor. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Valor. Um valor TRUE indica que a página do banco de dados contém dados. Um valor FALSE indica que a página contém apenas zeros. **ErrCheckDbPages** define este valor. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Valor. Um valor TRUE indica que houve uma incompatibilidade de checksum detectada na página do banco de dados, mas é um erro corrigível. **ErrCheckDbPages** define este valor. 
    
### <a name="checksumactual"></a>checksumActual
  
Inteiro de 64 bits não assinado. Indica o valor de checksum armazenado no banco de dados para essa página lógica. **ErrCheckDbPages** define este valor. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Inteiro de 64 bits não assinado. Este é o valor de soma de verificação esperado que é calculado para a página do banco de dados; é definido pelo **ErrCheckDbPages**. Se esse valor for diferente daquele armazenado na página de banco de dados (ou seja, o valor retornado em **checksumActual**), **ErrCheckDbPages** indicará que um erro foi encontrado nesta página de banco de dados. 
    
### <a name="dbtime"></a>dbTime
  
Inteiro de 64 bits não assinado. **ErrCheckDbPages** define este membro para o carimbo de data/hora na página do banco de dados. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Inteiro de 64-BT não assinado. **ErrCheckDbPages** define este membro como o valor de soma de verificação calculado do conteúdo da página, excluindo dados desnecessários ao determinar a equivalência de página lógica. Por exemplo, não é necessário considerar os valores de dados no espaço de página de banco de dados não usado. Este membro só será válido se os valores **checksumActual** e **checksumExpected** forem iguais. 
    
### <a name="ulflags"></a>ulFlags
  
Inteiro de 64 bits não assinado. Reserved for future use. O valor deste campo deve ser definido como 0 (zero) antes de chamar **ErrCheckDbPages**.
    
## <a name="remarks"></a>Comentários

Ao chamar a função **ErrCheckDbPages** , o parâmetro **rgPageInfo** é uma matriz de estruturas de ** \_ informações da página** . Deve haver uma estrutura **de \_ informações da página** para cada página de banco de dados a ser verificada. 
  
O aplicativo deve definir o membro **ulPgno** para o valor apropriado e também deve definir o membro **parâmetroulflags** como 0 (zero) antes de chamar **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Requirements

O Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

