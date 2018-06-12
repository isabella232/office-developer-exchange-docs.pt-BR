---
title: Validar um certificado de servidor para a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Saiba como criar e fazer referência a um método de retorno de chamada de validação de certificado para que você possa fazer solicitações da API gerenciada de EWS para um servidor Exchange.
ms.openlocfilehash: 13d7c51e55308b9e9997697a075c8a9e6b4f10d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750835"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="0209b-103">Validar um certificado de servidor para a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0209b-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="0209b-104">Saiba como criar e fazer referência a um método de retorno de chamada de validação de certificado para que você possa fazer solicitações da API gerenciada de EWS para um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="0209b-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="0209b-105">Por padrão, as versões do Exchange começando com o Exchange 2007 SP1 usam X509 autoassinado certificados para autenticar chamadas do EWS.</span><span class="sxs-lookup"><span data-stu-id="0209b-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="0209b-106">Quando você estiver usando a API gerenciada de EWS, você precisa criar um método de retorno de chamada de validação de certificado; Caso contrário, as solicitações de API gerenciada de EWS falhará.</span><span class="sxs-lookup"><span data-stu-id="0209b-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="0209b-107">Se você estiver usando o serviço Descoberta automática, a chamada para o método de descoberta automática de API gerenciada EWS falhará com um erro de **AutodiscoverLocalException** .</span><span class="sxs-lookup"><span data-stu-id="0209b-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="0209b-108">Se você estiver usando um proxy de serviço web gerado pelo web, você também pode precisar criar um método de retorno de chamada de validação, dependendo de como o proxy é criado.</span><span class="sxs-lookup"><span data-stu-id="0209b-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="0209b-109">Pré-requisitos para a criação de um método de retorno de chamada de validação</span><span class="sxs-lookup"><span data-stu-id="0209b-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="0209b-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="0209b-110"></span></span>

<span data-ttu-id="0209b-111">Configurar para validar um certificado de servidor, certifique-se de que as seguintes condições forem verdadeiras:</span><span class="sxs-lookup"><span data-stu-id="0209b-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="0209b-112">Seu servidor do Exchange está usando um certificado autoassinado para o EWS.</span><span class="sxs-lookup"><span data-stu-id="0209b-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="0209b-113">Se o administrador tiver instalado um certificado válido que rastreia a um certificado raiz, você não precisará criar um método de retorno de chamada de validação.</span><span class="sxs-lookup"><span data-stu-id="0209b-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="0209b-114">Você está criando um aplicativo gerenciado que inclui uma referência para os seguintes namespaces do .NET Framework necessárias:</span><span class="sxs-lookup"><span data-stu-id="0209b-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="0209b-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="0209b-115">**System.Net**</span></span>
  - <span data-ttu-id="0209b-116">**System.Net.Security**</span><span class="sxs-lookup"><span data-stu-id="0209b-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="0209b-117">**System.Security.Cryptography.X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="0209b-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="0209b-118">Exemplo: Método de retorno de chamada para validar um certificado de servidor para a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0209b-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="0209b-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="0209b-119"></span></span>

<span data-ttu-id="0209b-120">O exemplo de código a seguir mostra como criar um X509 método de retorno de chamada de validação de certificado para a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="0209b-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="0209b-121">Esse método irá validar um X509 de certificado e apenas retornar true quando um dos seguintes critérios é atendido:</span><span class="sxs-lookup"><span data-stu-id="0209b-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="0209b-122">O certificado é válido e rastreia de volta a um certificado raiz válido.</span><span class="sxs-lookup"><span data-stu-id="0209b-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="0209b-123">O certificado é válido e autoassinado para o servidor que retornados a ele.</span><span class="sxs-lookup"><span data-stu-id="0209b-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="0209b-124">O método de retorno de validação de certificado neste exemplo fornece segurança suficiente para o desenvolvimento e teste de aplicativos do EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="0209b-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="0209b-125">No entanto, ele não pode fornecer segurança suficiente para seu aplicativo implantado.</span><span class="sxs-lookup"><span data-stu-id="0209b-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="0209b-126">Sempre verifique se que o método de retorno de validação do certificado que você usa cumpre os requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0209b-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

<span data-ttu-id="0209b-127">Você pode usar a classe **ServicePointManager** no namespace .NET **System.Net** para ligar um método de retorno de chamada de validação, definindo a propriedade **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="0209b-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="0209b-128">Você pode usar o código semelhante ao exemplo de código a seguir para definir a propriedade **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="0209b-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="0209b-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="0209b-129">Next steps</span></span>
<span data-ttu-id="0209b-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="0209b-130"></span></span>

<span data-ttu-id="0209b-131">Após ter criado o método de retorno de validação para o EWS Managed API, você pode usar o serviço Descoberta automática para fazer configurações de domínio e de usuário e de pontos de conexão a partir de um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="0209b-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="0209b-132">Para obter mais informações, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="0209b-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="0209b-133">Usar descoberta automática para encontrar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="0209b-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="0209b-134">Obter configurações de usuário do Exchange usando a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0209b-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="0209b-135">Fazer configurações de domínio a partir de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="0209b-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="0209b-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="0209b-136">See also</span></span>

- [<span data-ttu-id="0209b-137">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="0209b-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="0209b-138">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="0209b-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

