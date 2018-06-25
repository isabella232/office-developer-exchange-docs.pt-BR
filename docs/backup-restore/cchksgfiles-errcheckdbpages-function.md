---
title: Função CChkSGFiles.ErrCheckDbPages
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750629"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>Função CChkSGFiles.ErrCheckDbPages

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valida um intervalo de páginas em um banco de dados especificado. 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Par�metros

### <a name="idb"></a>iDb
  
Parâmetro de entrada. Um índice na matriz de bancos de dados especificado no parâmetro **[] de rgwszDb** para a função **ErrInit** . O banco de dados indexado por esse parâmetro será verificado. 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
Parâmetro de entrada. Um ponteiro para um buffer que contém uma ou mais páginas de banco de dados a ser verificado. O tamanho do buffer deve ser um múltiplo do tamanho de página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** . O aplicativo de chamada deve espaço em buffer com o conteúdo de página do banco de dados antes de chamar **ErrCheckDbPages**.
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
Parâmetro de entrada. O tamanho do parâmetro **pvPageBuffer** , em bytes. Este valor deve ser um múltiplo do tamanho de página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** . 
    
### <a name="rgpageinfo"></a>[] de rgPageInfo 
  
Parâmetro de entrada/saída. Uma matriz de **página\_INFO** detalhada de estruturas **ErrCheckDbPages** preenche com resultados de cada página de banco de dados que está marcada. A matriz deve ter um elemento para cada página de banco de dados passado para o parâmetro **pvPageBuffer** e o campo **ulPgno** em cada **página\_INFO** estrutura deve ser definida como o número de página lógica que corresponde à página de banco de dados. Para obter mais informações, consulte "Comentários" mais adiante neste tópico. 
    
### <a name="cpageinfo"></a>cPageInfo
  
Parâmetro de entrada. O número de entradas na matriz **[] de rgPageInfo** . Este valor deve ser igual ao número de páginas de banco de dados passada no parâmetro **pvPageBuffer** . 
    
### <a name="ulflags"></a>ulFlags 
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado neste parâmetro deve ser de 0 (zero).
    
## <a name="return-value"></a>Valor retornado

Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Comentários

Observe que você precisa especificar o banco de dados na matriz de bancos de dados passado para a função **ErrInit** . Além disso, **ErrCheckDbHeaders** deve ser chamado antes de **ErrCheckDbPages**.
  
O aplicativo de chamada deve alocar um buffer de memória que é grande o suficiente para armazenar as páginas do banco de dados a ser verificado. O aplicativo é responsável por preencher o buffer com o conteúdo de uma ou mais dessas páginas de banco de dados. 
  
O aplicativo de chamada deve chamar **ErrCheckDbHeaders** antes de chamar **ErrCheckDbPages**. Esta função pode ser chamada quantas vezes forem necessárias para cobrir todas as páginas em todos os arquivos de banco de dados que devem ser verificado.
  
No parâmetro **[] de rgPageInfo** , cada elemento retornado contém informações sobre a página de banco de dados em um **página\_INFO** estrutura. Se a função de **ErrCheckDbPages** retornará um erro, o aplicativo deve verificar cada **página\_INFO** estrutura para determinar em qual página o erro foi encontrado. Por exemplo, comparar os valores **checksumActual** e **checksumExpected** indicará se foi detectado um erro de soma de verificação nessa página de banco de dados. 
  
Se **ErrCheckDbPages** detecta quaisquer erros no conteúdo do banco de dados, ele cria uma entrada de log de eventos de erro do Windows. 
  
O objeto **CChkSGFiles** determina se todos os bancos de dados registrados com a função **ErrInit** realmente marcados. Especificamente, **CChkSGFiles** usa a função **ErrCheckDbPages** para determinar se o mesmo número de páginas de banco de dados indicado pelo **ErrCheckDbHeaders** realmente foram verificado. Se o número correto das páginas em cada banco de dados não foram verificado com êxito, a função de **ErrTerm** retornará um erro. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você pode chamar a função **ErrCheckDbPages** na parte multithread do aplicativo. Observe que **ErrCheckDbPages** é geralmente chamado várias vezes para cada banco de dados está marcado. 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

