---
title: Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Saiba como usar cmdlets do Shell de gerenciamento do Exchange para criar uma ferramenta que retorna uma lista de usuários de caixa de correio do Exchange.
ms.openlocfilehash: 6f64330a11e372bffbea2fcd88bcfa0231ec0f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750966"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="86557-103">Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="86557-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="86557-104">Saiba como usar cmdlets do Shell de gerenciamento do Exchange para criar uma ferramenta que retorna uma lista de usuários de caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="86557-105">**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="86557-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="86557-106">Obtendo uma lista de usuários do Exchange Online, Exchange Online como parte do Office 365, ou uma versão do Exchange, começando com o Exchange 2013 usando uma ferramenta gerenciada que chama um cmdlet do Shell de gerenciamento do Exchange é um processo de duas etapas.</span><span class="sxs-lookup"><span data-stu-id="86557-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="86557-107">Primeiro, você estabelece um espaço de trabalho remoto em um servidor do Exchange; em seguida, você pode executar o cmdlet para recuperar as informações do usuário do espaço de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="86557-108">Para conectar o espaço de trabalho remoto, você precisará autenticar com o Exchange server usando o esquema de autenticação que atenda aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="86557-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="86557-109">Este artigo fornece exemplos de código que você pode usar para configurar um espaço de trabalho remoto e executar um cmdlet do Shell de gerenciamento do Exchange para obter uma lista de usuários a partir de um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="86557-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-110"></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="86557-111">Pré-requisitos para obter uma lista de usuários de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="86557-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="86557-112">Para realizar essa tarefa, você precisa de uma referência para os namespaces a seguir:</span><span class="sxs-lookup"><span data-stu-id="86557-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="86557-113">**System.Collections.ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="86557-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="86557-114">**System.Management.Automation**</span><span class="sxs-lookup"><span data-stu-id="86557-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="86557-115">**System.Management.Automation.Remoting**</span><span class="sxs-lookup"><span data-stu-id="86557-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="86557-116">**System.Management.Automation.Runspaces**</span><span class="sxs-lookup"><span data-stu-id="86557-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="86557-117">Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência para o assembly Automation ao projeto.</span><span class="sxs-lookup"><span data-stu-id="86557-117">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project.</span></span> <span data-ttu-id="86557-118">O assembly pode ser encontrado em um dos seguintes locais:</span><span class="sxs-lookup"><span data-stu-id="86557-118">The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="86557-119">Para Windows XP e Windows Vista sistemas operacionais, o diretório de instalação do Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="86557-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="86557-120">Para os sistemas de operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="86557-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="86557-121">Não carrega o snap-in de gerenciamento do Exchange 2013 no runspace em computadores que estão executando aplicativos que automatizam o cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="86557-122">O aplicativo em vez disso, deve criar um espaço de trabalho remoto, conforme descrito neste artigo.</span><span class="sxs-lookup"><span data-stu-id="86557-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="86557-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-123"></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="86557-124">Conectar a um espaço de trabalho remoto em um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="86557-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="86557-125">O método que você usa para se conectar a um espaço de trabalho remoto para usar um Shell de gerenciamento do Exchange cmdlet varia com base no esquema de autenticação que você está usando.</span><span class="sxs-lookup"><span data-stu-id="86557-125">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using.</span></span> <span data-ttu-id="86557-126">Esta seção fornece exemplos de código que mostram como se conectar a um espaço de trabalho remoto quando você estiver usando um método de autenticação listado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="86557-126">This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="86557-127">**Método de autenticação**</span><span class="sxs-lookup"><span data-stu-id="86557-127">**Authentication method**</span></span>|<span data-ttu-id="86557-128">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="86557-128">**Applies to**</span></span>|<span data-ttu-id="86557-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="86557-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="86557-130">Conectar a um espaço de trabalho remoto no Exchange Online usando autenticação básica</span><span class="sxs-lookup"><span data-stu-id="86557-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="86557-131">Servidores do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="86557-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="86557-132">Conectar a um espaço de trabalho remoto usando a autenticação de certificado</span><span class="sxs-lookup"><span data-stu-id="86557-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="86557-133">Exchange Online e Exchange servidores locais</span><span class="sxs-lookup"><span data-stu-id="86557-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="86557-134">Conectar a um espaço de trabalho remoto em um servidor Exchange usando a autenticação Kerberos</span><span class="sxs-lookup"><span data-stu-id="86557-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="86557-135">Exchange Online e Exchange servidores locais</span><span class="sxs-lookup"><span data-stu-id="86557-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="86557-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-136"></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="86557-137">Conectar a um espaço de trabalho remoto no Exchange Online usando autenticação básica</span><span class="sxs-lookup"><span data-stu-id="86557-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="86557-138">O exemplo de código a seguir define o método **GetUsersUsingBasicAuth** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor Exchange Online remoto usando a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="86557-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="86557-139">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um espaço de trabalho remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="86557-140">Esse método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="86557-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="86557-141">**liveIDConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor do Exchange Online que fará a autenticação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86557-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="86557-142">Se estiver executando o Exchange Online no Office 365, o URI é https://outlook.office365.com/PowerShell-LiveID; Caso contrário, o URI é https://\<nomedoservidor\>/PowerShell-LiveID.</span><span class="sxs-lookup"><span data-stu-id="86557-142">If Exchange Online is running in Office 365, the URI is https://outlook.office365.com/PowerShell-LiveID; otherwise, the URI is https://\<servername\>/PowerShell-LiveID.</span></span> 
    
-  <span data-ttu-id="86557-143">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento do esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="86557-144">O esquema URI é http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-144">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
-  <span data-ttu-id="86557-145">**credenciais** &ndash; Um objeto [PSCredential](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86557-145">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="86557-146">**contagem** &ndash; o número de usuários de caixa de correio do Exchange para retornar.</span><span class="sxs-lookup"><span data-stu-id="86557-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingBasicAuth(
    string liveIDConnectionUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(liveIDConnectionUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingBasicAuth( _
    ByVal LiveIDConnectionUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(LiveIDConnectionUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="86557-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-147"></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="86557-148">Conectar a um espaço de trabalho remoto usando a autenticação de certificado</span><span class="sxs-lookup"><span data-stu-id="86557-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="86557-149">O exemplo de código a seguir define o método **GetUsersUsingCertificate** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando um certificado.</span><span class="sxs-lookup"><span data-stu-id="86557-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="86557-150">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um espaço de trabalho remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="86557-151">Esse método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="86557-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="86557-152">**impressão digital** &ndash; Uma cadeia de caracteres que contém a impressão digital do certificado que é usado para autenticar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86557-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="86557-153">**certConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor que irá autenticar o certificado.</span><span class="sxs-lookup"><span data-stu-id="86557-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="86557-154">O URI será uma das listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="86557-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="86557-155">**Tabela 1. certConnectionUri URIs**</span><span class="sxs-lookup"><span data-stu-id="86557-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="86557-156">**Server**</span><span class="sxs-lookup"><span data-stu-id="86557-156">**Server**</span></span>|<span data-ttu-id="86557-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="86557-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="86557-158">Servidor do Exchange sem usar SSL</span><span class="sxs-lookup"><span data-stu-id="86557-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="86557-159">Servidor do Exchange usando SSL</span><span class="sxs-lookup"><span data-stu-id="86557-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="86557-160">O Exchange Online como parte do Office 365</span><span class="sxs-lookup"><span data-stu-id="86557-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="86557-161">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento do esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="86557-162">O esquema URI é http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-162">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="86557-163">**contagem** &ndash; o número de usuários de caixa de correio do Exchange para retornar.</span><span class="sxs-lookup"><span data-stu-id="86557-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingCertificate(
    string thumbprint, string certConnectionUri, string schemaUri, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(certConnectionUri),
        schemaUri,
        thumbprint)
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingCertificate( _
    ByVal Thumbprint As String, ByVal CertConnectionUri As String, _
    ByVal SchemaUri As String, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo
    ConnectionInfo = New WSManConnectionInfo(New Uri(CertConnectionUri), SchemaUri, Thumbprint)
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="86557-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-164"></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="86557-165">Conectar a um espaço de trabalho remoto em um servidor Exchange usando a autenticação Kerberos</span><span class="sxs-lookup"><span data-stu-id="86557-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="86557-166">O exemplo de código a seguir define o método **GetUsersUsingKerberos** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando a autenticação Kerberos.</span><span class="sxs-lookup"><span data-stu-id="86557-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="86557-167">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um espaço de trabalho remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="86557-168">Esse método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="86557-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="86557-169">**kerberosUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor Kerberos que fará a autenticação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86557-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="86557-170">O URI será uma das listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="86557-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="86557-171">**Tabela 2. kerberosUri URIs**</span><span class="sxs-lookup"><span data-stu-id="86557-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="86557-172">**Server**</span><span class="sxs-lookup"><span data-stu-id="86557-172">**Server**</span></span>|<span data-ttu-id="86557-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="86557-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="86557-174">Servidor do Exchange sem usar SSL</span><span class="sxs-lookup"><span data-stu-id="86557-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="86557-175">Servidor do Exchange usando SSL</span><span class="sxs-lookup"><span data-stu-id="86557-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="86557-176">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento do esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="86557-177">O esquema URI é http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-177">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="86557-178">**credenciais** &ndash; Um objeto [PSCredential](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86557-178">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="86557-179">**contagem** &ndash; o número de usuários de caixa de correio do Exchange para retornar.</span><span class="sxs-lookup"><span data-stu-id="86557-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingKerberos(
    string kerberosUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(kerberosUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```

```vb
  Function GetUsersUsingKerberos( _
    ByVal KerberosUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(KerberosUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="86557-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="86557-180"></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="86557-181">Fazer uma lista de usuários de caixa de correio a partir de um espaço de trabalho remoto</span><span class="sxs-lookup"><span data-stu-id="86557-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="86557-182">O exemplo de código a seguir define o método **GetUserInformation** , que retorna uma coleção de instâncias de [PSObject](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) que representam os usuários de caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86557-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](http://msdn.microsoft.com/pt-br/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="86557-183">Este método é chamado pelos métodos **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**e **GetUsersUsingKerberos** para retornar a lista de usuários do servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="86557-184">Esse método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="86557-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="86557-185">**contagem** &ndash; o número de usuários de caixa de correio do Exchange para retornar.</span><span class="sxs-lookup"><span data-stu-id="86557-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="86557-186">**Runspace** &ndash; o espaço de trabalho remoto estabelecido para o servidor Exchange remoto.</span><span class="sxs-lookup"><span data-stu-id="86557-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
```cs
public Collection<PSObject> GetUserInformation(int count, Runspace runspace)
{
    using (PowerShell powershell = PowerShell.Create())
    {
        powershell.AddCommand("Get-Users");
        powershell.AddParameter("ResultSize", count);
        runspace.Open();
        powershell.Runspace = runspace;
        return powershell.Invoke();
    }
}
```

```vb
Function GetUserInformation(ByVal Count As Integer, ByVal RemoteRunspace As Runspace) As Collection(Of PSObject)
    Dim RemotePowerShell As PowerShell = PowerShell.Create
    RemotePowerShell.AddCommand("Get-Users")
    RemotePowerShell.AddParameter("ResultSize", Count)
    ' Open the remote runspace on the server.
    RemoteRunspace.Open()
    ' Associate the runspace with the Exchange Management Shell.
    RemotePowerShell.Runspace = RemoteRunspace
    ' Invoke the Exchange Management Shell to run the command.
    Return RemotePowerShell.Invoke
End Function

```

<span data-ttu-id="86557-187">O método **GetUserInformation** retornará não mais do que a _contagem de_ usuários de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="86557-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="86557-188">Para simplificar o código neste exemplo, o método não filtrar ou caso contrário, limite os usuários de caixa de correio que são retornados.</span><span class="sxs-lookup"><span data-stu-id="86557-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="86557-189">Confira também</span><span class="sxs-lookup"><span data-stu-id="86557-189">See also</span></span>

- [<span data-ttu-id="86557-190">Criar ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="86557-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="86557-191">Use a resposta de cmdlet do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="86557-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

