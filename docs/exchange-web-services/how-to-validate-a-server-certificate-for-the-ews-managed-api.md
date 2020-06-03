---
title: Validar um certificado de servidor para a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Saiba como criar e referenciar um método de retorno de chamada de validação de certificado para que você possa fazer solicitações de API gerenciada por EWS para um servidor Exchange.
localization_priority: Priority
ms.openlocfilehash: 195c51ca71890d6092e4182d23990bb528d37095
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456723"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="2c8cd-103">Validar um certificado de servidor para a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="2c8cd-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="2c8cd-104">Saiba como criar e referenciar um método de retorno de chamada de validação de certificado para que você possa fazer solicitações de API gerenciada por EWS para um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="2c8cd-105">Por padrão, as versões do Exchange a partir do Exchange 2007 SP1 usam certificados X509 autoassinados para autenticar chamadas do EWS.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="2c8cd-106">Quando estiver usando a API gerenciada do EWS, você precisará criar um método de retorno de chamada de validação de certificado; caso contrário, as solicitações de API gerenciada do EWS falharão.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="2c8cd-107">Se você estiver usando o serviço de descoberta automática, a chamada para o método autodiscover da API gerenciada do EWS falhará com um erro **AutodiscoverLocalException** .</span><span class="sxs-lookup"><span data-stu-id="2c8cd-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="2c8cd-108">Se você estiver usando um proxy de serviço Web gerado pela Web, também poderá ser necessário criar um método de retorno de chamada de validação, dependendo de como o proxy é criado.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="2c8cd-109">Pré-requisitos para a criação de um método de retorno de chamada de validação</span><span class="sxs-lookup"><span data-stu-id="2c8cd-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="2c8cd-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="2c8cd-110"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="2c8cd-111">Para configurar a validação de um certificado de servidor, verifique se os seguintes itens são verdadeiros:</span><span class="sxs-lookup"><span data-stu-id="2c8cd-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="2c8cd-112">O servidor do Exchange está usando um certificado autoassinado para EWS.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="2c8cd-113">Se o administrador tiver instalado um certificado válido que rastreia um certificado raiz, não será necessário criar um método de retorno de chamada de validação.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="2c8cd-114">Você está criando um aplicativo gerenciado que inclui uma referência para os seguintes namespaces .NET Framework necessários:</span><span class="sxs-lookup"><span data-stu-id="2c8cd-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="2c8cd-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="2c8cd-115">**System.Net**</span></span>
  - <span data-ttu-id="2c8cd-116">**System .net. Security**</span><span class="sxs-lookup"><span data-stu-id="2c8cd-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="2c8cd-117">**System. Security. Cryptography. X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="2c8cd-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="2c8cd-118">Exemplo: método de retorno de chamada para validar um certificado de servidor para a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="2c8cd-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="2c8cd-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="2c8cd-119"><a name="bk_example"> </a></span></span>

<span data-ttu-id="2c8cd-120">O exemplo de código a seguir mostra como criar um método de retorno de chamada de validação de certificado X509 para a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="2c8cd-121">Este método validará um certificado X509 e retornará apenas true quando um dos seguintes critérios for atendido:</span><span class="sxs-lookup"><span data-stu-id="2c8cd-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="2c8cd-122">O certificado é válido e rastreia de volta para um certificado raiz válido.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="2c8cd-123">O certificado é válido e é auto-assinado pelo servidor que o retornou.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="2c8cd-124">O método de retorno de chamada de validação de certificado neste exemplo fornece segurança suficiente para o desenvolvimento e teste de aplicativos da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="2c8cd-125">No entanto, ele pode não fornecer segurança suficiente para seu aplicativo implantado.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="2c8cd-126">Você sempre deve certificar-se de que o método de retorno de chamada de validação de certificado usado atenda aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
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

<span data-ttu-id="2c8cd-127">Você usa a classe **ServicePointManager** no namespace do .NET **System.net** para conectar um método de retorno de chamada de validação, definindo a propriedade **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="2c8cd-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="2c8cd-128">Você pode usar código semelhante ao exemplo de código a seguir para definir a propriedade **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="2c8cd-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="2c8cd-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2c8cd-129">Next steps</span></span>
<span data-ttu-id="2c8cd-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="2c8cd-130"><a name="bk_example"> </a></span></span>

<span data-ttu-id="2c8cd-131">Depois de criar o método de retorno de chamada de validação para a API gerenciada do EWS, você pode usar o serviço de descoberta automática para obter pontos de conexão e configurações de usuário e domínio de um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c8cd-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="2c8cd-132">Para saber mais, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="2c8cd-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="2c8cd-133">Usar a Descoberta Automática para localizar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="2c8cd-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="2c8cd-134">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="2c8cd-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="2c8cd-135">Obter as configurações de domínio de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="2c8cd-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="2c8cd-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c8cd-136">See also</span></span>

- [<span data-ttu-id="2c8cd-137">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="2c8cd-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="2c8cd-138">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="2c8cd-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

