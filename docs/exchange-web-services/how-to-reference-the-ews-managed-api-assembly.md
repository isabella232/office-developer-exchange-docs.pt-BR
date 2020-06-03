---
title: Fazer referência ao assembly da API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Encontre informações sobre como fazer referência ao assembly da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: d49091781da279d87a1eab35608f19ece43a0333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527758"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="365cc-103">Fazer referência ao assembly da API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="365cc-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="365cc-104">Encontre informações sobre como fazer referência ao assembly da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="365cc-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="365cc-105">A API gerenciada do EWS fornece uma interface simples e com recursos completos para desenvolver e estender aplicativos que usam os serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="365cc-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="365cc-106">Se você estiver usando o Visual Studio ou outro editor de código para desenvolver seu aplicativo de API gerenciada do EWS, será necessário fazer uma referência ao assembly da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="365cc-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="365cc-107">Se você ainda não instalou a API gerenciada do EWS, não se esqueça de [baixar a API](https://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="365cc-107">If you haven't installed the EWS Managed API already, be sure to [download the API](https://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
> <span data-ttu-id="365cc-108">A API gerenciada do EWS já está disponível como um projeto de código-fonte aberto no [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="365cc-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="365cc-109">É possível usar a biblioteca de software livre para:</span><span class="sxs-lookup"><span data-stu-id="365cc-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="365cc-110">Contribui com correções de bug e melhorias à API.</span><span class="sxs-lookup"><span data-stu-id="365cc-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="365cc-111">Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial.</span><span class="sxs-lookup"><span data-stu-id="365cc-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="365cc-112">Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. </span><span class="sxs-lookup"><span data-stu-id="365cc-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
>  <span data-ttu-id="365cc-113">Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via github.</span><span class="sxs-lookup"><span data-stu-id="365cc-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="365cc-114">Fazer referência ao assembly</span><span class="sxs-lookup"><span data-stu-id="365cc-114">Referencing the assembly</span></span>

<span data-ttu-id="365cc-115">A maneira mais comum de adicionar uma referência é usar o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="365cc-115">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="365cc-116">Sabemos que alguns desenvolvedores gostam de usar outros editores, portanto, estamos incluindo instruções para usar o compilador de linha de comando e instruções para usar o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="365cc-116">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="365cc-117">Você pode notar que os exemplos de código a seguir têm as mesmas instruções **using** .</span><span class="sxs-lookup"><span data-stu-id="365cc-117">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="365cc-118">A diferença entre os dois métodos é que o compilador de linha de comando precisa do local do arquivo de assembly.</span><span class="sxs-lookup"><span data-stu-id="365cc-118">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="365cc-119">A referência do Visual Studio trata isso para você em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="365cc-119">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="365cc-120">Para adicionar uma referência usando o Visual Studio</span><span class="sxs-lookup"><span data-stu-id="365cc-120">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="365cc-121">Coloque o arquivo Microsoft. Exchange. WebServices. dll e o arquivo Microsoft. Exchange. WebServices. xml em uma pasta de sua escolha.</span><span class="sxs-lookup"><span data-stu-id="365cc-121">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="365cc-122">Por padrão, os arquivos são instalados no `C:\Program Files\Microsoft\Exchange\Web Services\2.0\` , mas você pode armazenar os arquivos em qualquer lugar no seu computador.</span><span class="sxs-lookup"><span data-stu-id="365cc-122">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="365cc-123">No painel Gerenciador de soluções no Visual Studio, selecione **referências**e, em seguida, escolha **Adicionar referência**.</span><span class="sxs-lookup"><span data-stu-id="365cc-123">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="365cc-124">Isso abre a janela Adicionar referência.</span><span class="sxs-lookup"><span data-stu-id="365cc-124">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="365cc-125">Na janela Adicionar referência, navegue até a guia **procurar** , navegue até o local do arquivo Microsoft. Exchange. WebServices. dll, selecione esse arquivo e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="365cc-125">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="365cc-126">Para usar a API gerenciada do EWS em seu aplicativo, adicione uma instrução **using** para o namespace **Microsoft. Exchange. WebServices. Data** .</span><span class="sxs-lookup"><span data-stu-id="365cc-126">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="365cc-127">Para adicionar uma referência e compilar seu aplicativo com o compilador de linha de comando</span><span class="sxs-lookup"><span data-stu-id="365cc-127">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="365cc-128">Coloque o arquivo Microsoft. Exchange. WebServices. dll em uma pasta de sua escolha.</span><span class="sxs-lookup"><span data-stu-id="365cc-128">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice.</span></span> <span data-ttu-id="365cc-129">Esta pasta será a pasta de saída para o compilador.</span><span class="sxs-lookup"><span data-stu-id="365cc-129">This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="365cc-130">No editor de código-fonte, adicione uma instrução **using** ao código-fonte do namespace **Microsoft. Exchange. WebServices. Data** .</span><span class="sxs-lookup"><span data-stu-id="365cc-130">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="365cc-131">Execute o compilador de linha de comando para compilar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="365cc-131">Run the command-line compiler to build the application.</span></span> <span data-ttu-id="365cc-132">O comando a seguir usa o compilador C# do .NET Framework para criar o aplicativo do Windows definido no arquivo de código-fonte "program.cs".</span><span class="sxs-lookup"><span data-stu-id="365cc-132">The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs".</span></span> <span data-ttu-id="365cc-133">Ele pressupõe que o compilador está localizado no diretório de instalação padrão e que o arquivo Microsoft. Exchange. WebServices. dll está em um subdiretório do diretório atual chamado "Build".</span><span class="sxs-lookup"><span data-stu-id="365cc-133">It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="365cc-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="365cc-134">See also</span></span>

- [<span data-ttu-id="365cc-135">Introdução aos aplicativos clientes de API gerenciada por EWS</span><span class="sxs-lookup"><span data-stu-id="365cc-135">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="365cc-136">Configurando seu ambiente de desenvolvimento de aplicativos do Exchange</span><span class="sxs-lookup"><span data-stu-id="365cc-136">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="365cc-137">Comunicar-se com o EWS usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="365cc-137">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

