---
title: Referência de classe função cchksgfiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Encontre informações de referência para a API do CHKSGFILES no Exchange 2013.
ms.openlocfilehash: 38b1f2c900767c22594636f0c6ddf4855961aec4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526729"
---
# <a name="cchksgfiles-class-reference"></a>Referência de classe função cchksgfiles

Encontre informações de referência para a API do CHKSGFILES no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
A API CHKSGFILES permite que aplicativos de backup e restauração verifiquem a integridade dos arquivos de log de transações e bancos de dados do Exchange Server 2013 programaticamente. Você pode usar essa API em aplicativos de backup e restauração que usam o serviço de cópias de sombra de volume (VSS).
  
> [!NOTE]
> Os grupos de armazenamento não estão disponíveis no Exchange 2013. O suporte para grupos de armazenamento foi removido de versões do Exchange a partir do Exchange Server 2010. Para compatibilidade com versões anteriores com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange 2010, a API CHKSGFILES permite que você especifique grupos de armazenamento. Ao executar o CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento para uma cadeia de caracteres vazia. 
  
## <a name="file-location"></a>Local do arquivo
<a name="bk_fileslocation"> </a>

A API do CHKSGFILES é fornecida como parte do Exchange 2013. Você pode usar essa API em um computador que tenha a função de servidor caixa de Correio instalada. 
  
Por padrão, a DLL CHKSGFILES é instalada no diretório C:\Arquivos de Files\Microsoft\Exchange\V15\Bin.
  
O Exchange 2013 inclui apenas uma versão de 64 bits (amd64) da API CHKSGFILES. 
  
Você pode baixar um arquivo. zip que inclui a biblioteca CHKSGFILE. lib e os arquivos de cabeçalho CHKSGFILES. hXX para uso no seu aplicativo personalizado no [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Linguagens de desenvolvimento
<a name="bk_developmentlanguages"> </a>

A API CHKSGFILES deve ser usada com versões do Visual Studio que começam com o Visual Studio 2005 no C/C++ nativo. A API CHKSGFILES não se destina ao uso em código gerenciado. Embora você possa criar um assembly de interoperabilidade com com o CHKSGFILES, não enviamos um assembly de interoperabilidade COM com o Exchange 2013.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Função função cchksgfiles. CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Função função cchksgfiles. Delete](cchksgfiles-delete-function.md)
    
- [Enumeração função cchksgfiles. ERR](cchksgfiles-err-enumeration.md)
    
- [Função função cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Função função cchksgfiles. ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Função função cchksgfiles. ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Função função cchksgfiles. ErrGetHeader (reservado)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Função função cchksgfiles. ErrInit](cchksgfiles-errinit-function.md)
    
- [Função função cchksgfiles. ErrTerm](cchksgfiles-errterm-function.md)
    
- [Enumeração função cchksgfiles. iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Função função cchksgfiles. New](cchksgfiles-new-function.md)
    
- [Enumeração função cchksgfiles. NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Struct função cchksgfiles. PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Função função cchksgfiles. PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Confira também

- [Desenvolvimento do Exchange Online e do Exchange](../exchange-server-development.md)
- [Backup, restauração e recuperação de desastre](https://technet.microsoft.com/library/dd876874)
    

