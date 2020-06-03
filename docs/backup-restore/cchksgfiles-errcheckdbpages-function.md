---
title: Função função cchksgfiles. ErrCheckDbPages
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526722"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>Função função cchksgfiles. ErrCheckDbPages

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

## <a name="parameters"></a>Parâmetros

### <a name="idb"></a>iDb
  
Parâmetro de entrada. Um índice na matriz de bancos de dados especificado no parâmetro **rgwszDb []** para a função **ErrInit** . O banco de dados indexado por esse parâmetro será verificado. 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
Parâmetro de entrada. Um ponteiro para um buffer contendo uma ou mais páginas de banco de dados a serem verificadas. O tamanho do buffer deve ser um múltiplo do tamanho da página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** . O aplicativo de chamada deve preencher o buffer com o conteúdo da página do banco de dados antes de chamar **ErrCheckDbPages**.
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
Parâmetro de entrada. O tamanho do parâmetro **pvPageBuffer** , em bytes. Esse valor deve ser um múltiplo do tamanho da página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** . 
    
### <a name="rgpageinfo"></a>rgPageInfo[] 
  
Parâmetro de entrada/saída. Uma matriz de estruturas de ** \_ informações de página** que **ErrCheckDbPages** preenche com resultados detalhados de cada página de banco de dados verificada. A matriz deve ter um elemento para cada página de banco de dados aprovada no parâmetro **pvPageBuffer** , e o campo **ulPgno** em cada estrutura de ** \_ informações de página** deve ser definido como o número de página lógica que corresponde à página do banco de dados. Para obter mais informações, consulte "Comentários", mais adiante neste tópico. 
    
### <a name="cpageinfo"></a>cPageInfo
  
Parâmetro de entrada. O número de entradas na matriz **rgPageInfo []** . Esse valor deve ser igual ao número de páginas de banco de dados passadas no parâmetro **pvPageBuffer** . 
    
### <a name="ulflags"></a>ulFlags 
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado nesse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Comentários

Observe que você precisa ter especificado o banco de dados na matriz de bancos de dados passada para a função **ErrInit** . Além disso, **ErrCheckDbHeaders** deve ser chamado antes de **ErrCheckDbPages**.
  
O aplicativo de chamada deve alocar um buffer de memória grande o suficiente para armazenar as páginas do banco de dados a serem verificadas. O aplicativo é responsável por preencher o buffer com o conteúdo de uma ou mais dessas páginas de banco de dados. 
  
O aplicativo de chamada deve chamar **ErrCheckDbHeaders** antes de chamar **ErrCheckDbPages**. Essa função pode ser chamada quantas vezes forem necessárias para abranger todas as páginas em todos os arquivos de banco de dados que devem ser verificados.
  
No parâmetro **rgPageInfo []** , cada elemento retornado contém informações sobre a página do banco de dados em uma estrutura de ** \_ informações da página** . Se a função **ErrCheckDbPages** retornar um erro, o aplicativo deve verificar cada estrutura de ** \_ informações da página** para determinar em qual página o erro foi encontrado. Por exemplo, comparar os valores **checksumActual** e **checksumExpected** indicará se um erro de checksum foi detectado na página do banco de dados. 
  
Se o **ErrCheckDbPages** detectar qualquer erro no conteúdo do banco de dados, ele criará uma entrada do log de eventos de erro do Windows. 
  
O objeto **função cchksgfiles** determina se todos os bancos de dados registrados com a função **ErrInit** foram realmente verificados. Especificamente, **função cchksgfiles** usa a função **ErrCheckDbPages** para determinar se o mesmo número de páginas de banco de dados indicadas por **ErrCheckDbHeaders** foram realmente verificadas. Se o número correto de páginas em cada banco de dados não foi verificado com êxito, a função **ErrTerm** retornará um erro. 
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, poderá chamar a função **ErrCheckDbPages** na parte multithread do aplicativo. Observe que **ErrCheckDbPages** normalmente é chamado várias vezes para cada banco de dados selecionado. 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

