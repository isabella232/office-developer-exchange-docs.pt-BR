---
title: Configurando seu ambiente de desenvolvimento de aplicativos do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: Saiba como configurar seu ambiente de desenvolvimento para criar um aplicativo EWS que se comunica com o Exchange.
localization_priority: Priority
ms.openlocfilehash: 01a106817f29bd696991b8a0c5d7d9b7dd420b94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463759"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>Configurando seu ambiente de desenvolvimento de aplicativos do Exchange

Saiba como configurar seu ambiente de desenvolvimento para criar um aplicativo EWS que se comunica com o Exchange.
  
Antes de começar a escrever seu aplicativo de serviços Web do Exchange (EWS), você precisará certificar-se de que seu ambiente de desenvolvimento atende a alguns requisitos mínimos. Você pode usar a API gerenciada do EWS, a API de acesso para cliente padrão para aplicativos do .NET Framework, para desenvolver seu aplicativo, ou você pode usar o EWS sozinho, com nosso sem um proxy autogerado. Em geral, recomendamos que você use a API gerenciada do EWS; no entanto, você pode [explorar a diferença entre essas duas opções](ews-client-design-overview-for-exchange.md) em mais detalhes para descobrir qual é a melhor para você. 
  
> [!NOTE]
> A API gerenciada do EWS já está disponível como um projeto de código-fonte aberto no [GitHub](https://github.com/officedev/ews-managed-api). É possível usar a biblioteca de software livre para: 
> - Contribui com correções de bug e melhorias à API. 
> - Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial. 
> - Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. 
> 
>  Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via github. 
  
## <a name="development-environment-for-the-ews-managed-api"></a>Ambiente de desenvolvimento para a API gerenciada do EWS
<a name="bk_EWSMA"> </a>

Para criar um aplicativo da API gerenciada por EWS, você precisará de acesso ao seguinte:
  
- A [API gerenciada do EWS](https://aka.ms/ews-managed-api-readme). 
    
    Você pode armazenar os arquivos da API gerenciada do EWS em qualquer lugar no computador; Por padrão, eles são instalados na pasta Program Files\Microsoft\Exchange\Web Services \\<version number \> .
    
- Uma caixa de correio em um servidor do Exchange que está executando o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão do Exchange a partir do Exchange Server 2007. 
    
    Você pode obter um plano de negócios do Exchange Online, incluindo uma avaliação gratuita, no [site do Office 365](https://office.microsoft.com/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a). Para se conectar à caixa de correio, você deve ter o nome de usuário e as credenciais da conta associada à caixa de correio.

    
- Uma versão do Visual Studio que começa com o Visual Studio 2005. Se você não tiver o Visual Studio no momento, poderá baixar uma [versão gratuita](https://visualstudio.microsoft.com/).
    
- Uma versão do .NET Framework começando com o .NET Framework 3,5. Você pode baixar o .NET Framework 3,5 no [centro de download da Microsoft](https://go.microsoft.com/fwlink/?LinkId=191777).
    
Além disso, será útil se você tiver alguma familiaridade com C#. Embora o Visual Studio ofereça suporte a outros idiomas além do C#, a maior parte do código de exemplo disponível para a API gerenciada do EWS é escrita em C#.
  
## <a name="development-environment-for-ews"></a>Ambiente de desenvolvimento para EWS
<a name="bk_EWS"> </a>

Você pode usar o EWS para desenvolver seu aplicativo de algumas maneiras diferentes. A maneira mais simples de usar o EWS é criar arquivos de texto que contenham suas solicitações XML e transmiti-las para o Exchange. Para fazer isso, aqui está o que você precisa: 
  
- Um editor de texto simples, como o bloco de notas, para editar sua solicitação XML. Qualquer editor de texto fará, embora você possa desejar um que irá ajudar na sua validação de sintaxe XML, como XMetal.
    
- Uma ferramenta ou um aplicativo que pode enviar e receber solicitações e respostas XML do SOAP, a fim de se comunicar com o Exchange.
    
Ao trabalhar com XML bruto, também é útil ter uma compreensão básica da formatação XML.
  
A segunda maneira de usar o EWS é criar um proxy gerado automaticamente que permite que você trabalhe com as operações usando uma linguagem .NET como C#. Veja o que você precisa para trabalhar com um proxy autogerado:
  
- Uma versão do Visual Studio que começa com o Visual Studio 2005, para criar uma referência de proxy. Você pode baixar uma [versão gratuita](https://visualstudio.microsoft.com/).
    
- Uma versão do .NET Framework começando com o .NET Framework 2,0. Você pode baixar o .NET Framework 3,5 no [centro de download da Microsoft](https://go.microsoft.com/fwlink/?LinkId=191777).
    
Se você usar um proxy gerado automaticamente, convém ter alguma familiaridade com programação C#.
  
> [!NOTE]
> Se você é um desenvolvedor do .NET Framework, recomendamos que você use a API gerenciada do EWS em vez de proxies gerados automaticamente para desenvolver contra o EWS. O modelo de objeto da API gerenciada do EWS é mais fácil de usar do que os modelos de objeto proxy gerados automaticamente. Além disso, a API gerenciada do EWS implementa a [descoberta automática](autodiscover-for-exchange.md) e inclui a lógica do lado do cliente. 
  
## <a name="see-also"></a>Confira também

- [Configurando seu ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)  
- [Controlar o acesso ao EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)  
- [Modelos de objeto do Exchange gerados pelos EWS](https://msdn.microsoft.com/library/jj190899)
    