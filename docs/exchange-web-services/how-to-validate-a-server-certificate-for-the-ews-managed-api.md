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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750835"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>Validar um certificado de servidor para a API gerenciada de EWS

Saiba como criar e fazer referência a um método de retorno de chamada de validação de certificado para que você possa fazer solicitações da API gerenciada de EWS para um servidor Exchange.
  
Por padrão, as versões do Exchange começando com o Exchange 2007 SP1 usam X509 autoassinado certificados para autenticar chamadas do EWS. Quando você estiver usando a API gerenciada de EWS, você precisa criar um método de retorno de chamada de validação de certificado; Caso contrário, as solicitações de API gerenciada de EWS falhará. Se você estiver usando o serviço Descoberta automática, a chamada para o método de descoberta automática de API gerenciada EWS falhará com um erro de **AutodiscoverLocalException** . Se você estiver usando um proxy de serviço web gerado pelo web, você também pode precisar criar um método de retorno de chamada de validação, dependendo de como o proxy é criado. 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>Pré-requisitos para a criação de um método de retorno de chamada de validação
<a name="bk_prereq"> </a>

Configurar para validar um certificado de servidor, certifique-se de que as seguintes condições forem verdadeiras: 
  
- Seu servidor do Exchange está usando um certificado autoassinado para o EWS. Se o administrador tiver instalado um certificado válido que rastreia a um certificado raiz, você não precisará criar um método de retorno de chamada de validação. 
    
- Você está criando um aplicativo gerenciado que inclui uma referência para os seguintes namespaces do .NET Framework necessárias: 
    
  - **System.Net**
  - **System.Net.Security**  
  - **System.Security.Cryptography.X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>Exemplo: Método de retorno de chamada para validar um certificado de servidor para a API gerenciada de EWS
<a name="bk_example"> </a>

O exemplo de código a seguir mostra como criar um X509 método de retorno de chamada de validação de certificado para a API gerenciada de EWS. Esse método irá validar um X509 de certificado e apenas retornar true quando um dos seguintes critérios é atendido: 
  
- O certificado é válido e rastreia de volta a um certificado raiz válido.    
- O certificado é válido e autoassinado para o servidor que retornados a ele. 
    
> [!IMPORTANT]
> O método de retorno de validação de certificado neste exemplo fornece segurança suficiente para o desenvolvimento e teste de aplicativos do EWS Managed API. No entanto, ele não pode fornecer segurança suficiente para seu aplicativo implantado. Sempre verifique se que o método de retorno de validação do certificado que você usa cumpre os requisitos de segurança da sua organização. 
  
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

Você pode usar a classe **ServicePointManager** no namespace .NET **System.Net** para ligar um método de retorno de chamada de validação, definindo a propriedade **ServerCertificateValidationCallback** . Você pode usar o código semelhante ao exemplo de código a seguir para definir a propriedade **ServerCertificateValidationCallback** . 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_example"> </a>

Após ter criado o método de retorno de validação para o EWS Managed API, você pode usar o serviço Descoberta automática para fazer configurações de domínio e de usuário e de pontos de conexão a partir de um servidor Exchange. Para obter mais informações, consulte os seguintes artigos:
  
- [Usar descoberta automática para encontrar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Fazer configurações de domínio a partir de um servidor do Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>Confira também

- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)  
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    

