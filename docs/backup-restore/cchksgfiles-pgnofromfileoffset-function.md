---
title: Função CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750637"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Função CChkSGFiles.PgnoFromFileOffset

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Retorna o número de página do banco de dados lógico que corresponde ao índice de bytes especificado no arquivo de banco de dados físico. Se o deslocamento de arquivo é inválido, ou se a função **ErrCheckDbHeaders** não tiver sido chamada para os bancos de dados, essa função retornará 0 (zero). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Par�metros

### <a name="ibfileoffset"></a>ibFileOffset
  
Parâmetro de entrada. O deslocamento em um arquivo de banco de dados, em bytes.
    
## <a name="return-value"></a>Valor retornado

Número de página lógica do arquivo de banco de dados que inclui o deslocamento especificado.
  
## <a name="remarks"></a>Comentários

Se o parâmetro **ibFileOffset** for inválido, a função de **PgnoFromFileOffset** retornará 0 (zero). 
  
**PgnoFromFileOffset** também retornará 0 (zero) se você ainda não chamado a função **ErrCheckDbHeaders** na instância do **CCheckSGFiles** . Você deve chamar **ErrCheckDbHeaders** para inicializar o tamanho de página do banco de dados e o número de páginas alocadas aos cabeçalhos de banco de dados. 
  
Você deve usar **PgnoFromFileOffset** para preencher o **página\_INFO** estruturar elementos em preparação para chamar **ErrCheckDbPages**. O parâmetro **rgPageInfo** para **ErrCheckDbPages** exige que cada elemento da matriz uma estrutura **PAGE_INFO** , com os valores de membro **ulPgno** inicializado corretamente. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você pode chamar a função **PgnoFromFileOffset** na parte multithread do aplicativo. Observe que você normalmente chamaria essa função várias vezes para cada banco de dados que está sendo verificado. 
  
## <a name="requirements"></a>Requisitos

Exchange Server 2013 apenas inclui uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissão de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

