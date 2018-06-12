---
title: Configurando o ambiente de desenvolvimento de aplicativos do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: Saiba mais sobre como configurar seu ambiente de desenvolvimento para criar um aplicativo do EWS que se comunica com o Exchange.
ms.openlocfilehash: 0c7d4c6d37b28b6797bdb638930b8582f31ffc5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750951"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>Configurando o ambiente de desenvolvimento de aplicativos do Exchange

Saiba mais sobre como configurar seu ambiente de desenvolvimento para criar um aplicativo do EWS que se comunica com o Exchange.
  
Antes de começar a gravar seu aplicativo de serviços Web do Exchange (EWS), você precisará certificar-se de que seu ambiente de desenvolvimento atende aos requisitos mínimos de alguns. Você pode usar o EWS Managed API, o acesso do cliente padrão API para aplicativos do .NET Framework para desenvolver seu aplicativo, ou você pode usar o EWS por si só, com nossa sem um proxy gerada automaticamente. Em geral, é recomendável que você use o EWS Managed API; No entanto, você pode [explorar a diferença entre essas duas opções](ews-client-design-overview-for-exchange.md) em mais detalhes para encontrar check-out que um é ideal para você. 
  
> [!NOTE]
>  A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api). Você pode usar a biblioteca de fonte aberta: > correções e melhorias para a API de colaboração. > Obtenha correções e aprimoramentos antes que estejam disponíveis em um lançamento oficial. > Acesso a implementação mais abrangente e atualizado da API, para usar como uma referência ou para criar novas bibliotecas em plataformas novas. > Bem-vindos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub. 
  
## <a name="development-environment-for-the-ews-managed-api"></a>Ambiente de desenvolvimento para a API gerenciada de EWS
<a name="bk_EWSMA"> </a>

Para criar um aplicativo do EWS Managed API, você precisará ter acesso ao seguinte:
  
- A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme). 
    
    Você pode armazenar os arquivos de API gerenciada de EWS em qualquer lugar em seu computador; Por padrão, eles são instalados nos serviços de Files\Microsoft\Exchange\Web programa\\< número da versão\> pasta.
    
- Uma caixa de correio em um servidor do Exchange que está executando o Exchange Online, Exchange Online como parte do Office 365 ou uma versão do Exchange começando com o Exchange Server 2007. 
    
    Você pode obter um plano do Exchange Online para negócios, incluindo uma avaliação gratuita, do [site do Office 365](http://office.microsoft.com/en-us/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a). Para se conectar à caixa de correio, você deve ter o nome de usuário e as credenciais da conta associada a caixa de correio.
    
- Uma versão do Visual Studio, começando com o Visual Studio 2005. Se você ainda não tem o Visual Studio, você pode baixar a versão gratuita do [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).
    
- Uma versão do .NET Framework começando com o .NET Framework 3.5. Você pode baixar o .NET Framework 3.5 do [Centro de Download da Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).
    
Além disso, é útil se você tiver alguma familiaridade com c#. Embora o Visual Studio suporta outros idiomas além do c#, a maioria dos exemplos de código disponíveis para a API gerenciada de EWS é gravado em c#.
  
## <a name="development-environment-for-ews"></a>Ambiente de desenvolvimento para o EWS
<a name="bk_EWS"> </a>

Você pode usar o EWS para desenvolver seu aplicativo de duas maneiras diferentes. A maneira mais simples para usar o EWS é criar arquivos de texto que contenham suas solicitações XML e transmitir para o Exchange. Para fazer isso, aqui está o que você precisa: 
  
- Um editor de texto simples, como o bloco de notas, para editar sua solicitação XML. Qualquer editor de texto farão, embora você pode querer que ajudará com sua validação de sintaxe XML como XMetal.
    
- Uma ferramenta ou aplicativo que pode enviar e receber solicitações de SOAP XML e respostas, para se comunicar com o Exchange.
    
Quando você trabalha com o XML bruto, também é útil ter uma compreensão básica de formatação de XML.
  
A segunda maneira de usar o EWS é criar um proxy de gerada automaticamente que permitem que você trabalhe com as operações usando um idioma .NET como c#. Aqui está o que você precisa funcionar com um proxy gerada automaticamente:
  
- Uma versão do Visual Studio, começando com o Visual Studio 2005, para criar uma referência de proxy. Você pode baixar a versão gratuita do [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).
    
- Uma versão do .NET Framework começando com o .NET Framework 2.0. Você pode baixar o .NET Framework 3.5 do [Centro de Download da Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).
    
Se você usar um proxy gerado automaticamente, você vai querer tenha alguma familiaridade com programação em c#.
  
> [!NOTE]
> Se você for um desenvolvedor do .NET Framework, recomendamos que você usar a API gerenciada de EWS em vez de proxies gerado automaticamente para desenvolver contra EWS. O modelo de objeto do EWS Managed API é mais fácil de usar do que os modelos de objeto de proxy gerada automaticamente. Além disso, a API gerenciada de EWS implementa a [descoberta automática](autodiscover-for-exchange.md) e inclui a lógica do lado do cliente. 
  
## <a name="see-also"></a>Confira também


- [Configurando o ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    
- [Controlar o acesso a EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)
    
- [EWS gerado modelos de objeto para o Exchange](https://msdn.microsoft.com/en-us/library/jj190899)
    

