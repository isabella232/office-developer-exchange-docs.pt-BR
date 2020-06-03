---
title: Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Saiba como usar os cmdlets do Shell de gerenciamento do Exchange para criar uma ferramenta que retorna uma lista de usuários de caixa de correio do Exchange.
localization_priority: Priority
ms.openlocfilehash: 817d92ef1bb88017f471681b448c052ecaa54e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435706"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="897c1-103">Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="897c1-104">Saiba como usar os cmdlets do Shell de gerenciamento do Exchange para criar uma ferramenta que retorna uma lista de usuários de caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="897c1-105">**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="897c1-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="897c1-106">Obter uma lista de usuários do Exchange Online, do Exchange Online como parte do Office 365 ou de uma versão do Exchange que comece com o Exchange 2013 usando uma ferramenta gerenciada que chama um cmdlet do Shell de gerenciamento do Exchange é um processo de duas etapas.</span><span class="sxs-lookup"><span data-stu-id="897c1-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="897c1-107">Primeiro, você estabelece um runspace remoto em um servidor Exchange; em seguida, execute o cmdlet para recuperar as informações do usuário no runspace remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="897c1-108">Para se conectar ao runspace remoto, você precisa autenticar com o servidor do Exchange usando o esquema de autenticação que atende aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="897c1-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="897c1-109">Este artigo fornece exemplos de código que você pode usar para configurar um runspace remoto e executar um cmdlet do Shell de gerenciamento do Exchange para obter uma lista de usuários de um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="897c1-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-110"><a name="bk_prerequisites"> </a></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="897c1-111">Pré-requisitos para obter uma lista de usuários de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="897c1-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="897c1-112">Para executar essa tarefa, você precisa de uma referência para os seguintes namespaces:</span><span class="sxs-lookup"><span data-stu-id="897c1-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="897c1-113">**System. Collections. ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="897c1-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="897c1-114">**System. Management. Automation**</span><span class="sxs-lookup"><span data-stu-id="897c1-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="897c1-115">**System. Management. Automation. Remoting**</span><span class="sxs-lookup"><span data-stu-id="897c1-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="897c1-116">**System. Management. Automation. Runspaces**</span><span class="sxs-lookup"><span data-stu-id="897c1-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="897c1-117">Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência ao assembly System. Management. Automation. dll para o projeto.</span><span class="sxs-lookup"><span data-stu-id="897c1-117">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project.</span></span> <span data-ttu-id="897c1-118">O assembly pode ser encontrado em um dos seguintes locais:</span><span class="sxs-lookup"><span data-stu-id="897c1-118">The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="897c1-119">Para os sistemas operacionais Windows XP e Windows Vista, o diretório de instalação do Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="897c1-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="897c1-120">Para os sistemas operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\ GAC_MSIL \System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="897c1-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="897c1-121">Não carregue o snap-in de gerenciamento do Exchange 2013 no runspace em computadores que executam aplicativos que automatizam os cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="897c1-122">Em vez disso, o aplicativo deve criar um runspace remoto, conforme descrito posteriormente neste artigo.</span><span class="sxs-lookup"><span data-stu-id="897c1-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="897c1-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-123"><a name="bk_gettinglistmailbox"> </a></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="897c1-124">Conectar-se a um runspace remoto em um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="897c1-125">O método que você usa para se conectar a um runspace remoto para usar um cmdlet do Shell de gerenciamento do Exchange varia com base no esquema de autenticação que você está usando.</span><span class="sxs-lookup"><span data-stu-id="897c1-125">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using.</span></span> <span data-ttu-id="897c1-126">Esta seção fornece exemplos de código que mostram como se conectar a um runspace remoto quando você estiver usando um método de autenticação listado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="897c1-126">This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="897c1-127">**Método de autenticação**</span><span class="sxs-lookup"><span data-stu-id="897c1-127">**Authentication method**</span></span>|<span data-ttu-id="897c1-128">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="897c1-128">**Applies to**</span></span>|<span data-ttu-id="897c1-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="897c1-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="897c1-130">Conectar-se a um runspace remoto no Exchange Online usando a autenticação básica</span><span class="sxs-lookup"><span data-stu-id="897c1-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="897c1-131">Servidores do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="897c1-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="897c1-132">Conectar-se a um runspace remoto usando a autenticação de certificado</span><span class="sxs-lookup"><span data-stu-id="897c1-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="897c1-133">Servidores locais do Exchange Online e do Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="897c1-134">Conectar-se a um runspace remoto em um servidor do Exchange usando a autenticação Kerberos</span><span class="sxs-lookup"><span data-stu-id="897c1-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="897c1-135">Servidores locais do Exchange Online e do Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="897c1-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-136"><a name="bk_basic"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="897c1-137">Conectar-se a um runspace remoto no Exchange Online usando a autenticação básica</span><span class="sxs-lookup"><span data-stu-id="897c1-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="897c1-138">O exemplo de código a seguir define o método **GetUsersUsingBasicAuth** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto do Exchange Online usando a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="897c1-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="897c1-139">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="897c1-140">Este método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="897c1-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="897c1-141">**liveIDConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor Exchange Online que autenticará o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="897c1-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="897c1-142">Se o Exchange Online estiver em execução no Office 365, o URI será `https://outlook.office365.com/PowerShell-LiveID` ; caso contrário, o URI é `https://<servername>/PowerShell-LiveID` .</span><span class="sxs-lookup"><span data-stu-id="897c1-142">If Exchange Online is running in Office 365, the URI is `https://outlook.office365.com/PowerShell-LiveID`; otherwise, the URI is `https://<servername>/PowerShell-LiveID`.</span></span> 
    
-  <span data-ttu-id="897c1-143">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="897c1-144">O URI do esquema é `https://schemas.microsoft.com/powershell/Microsoft.Exchange` .</span><span class="sxs-lookup"><span data-stu-id="897c1-144">The schema URI is `https://schemas.microsoft.com/powershell/Microsoft.Exchange`.</span></span> 
    
-  <span data-ttu-id="897c1-145">**credenciais** &ndash; Um objeto [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="897c1-145">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="897c1-146">**contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="897c1-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="897c1-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-147"><a name="bk_cert"> </a></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="897c1-148">Conectar-se a um runspace remoto usando a autenticação de certificado</span><span class="sxs-lookup"><span data-stu-id="897c1-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="897c1-149">O exemplo de código a seguir define o método **GetUsersUsingCertificate** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando um certificado.</span><span class="sxs-lookup"><span data-stu-id="897c1-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="897c1-150">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="897c1-151">Este método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="897c1-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="897c1-152">**impressão digital** &ndash; Uma cadeia de caracteres que contém a impressão digital do certificado usado para autenticar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="897c1-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="897c1-153">**certConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor que autenticará o certificado.</span><span class="sxs-lookup"><span data-stu-id="897c1-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="897c1-154">O URI será um dos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="897c1-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="897c1-155">**Tabela 1. URIs certConnectionUri**</span><span class="sxs-lookup"><span data-stu-id="897c1-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="897c1-156">**Servidor**</span><span class="sxs-lookup"><span data-stu-id="897c1-156">**Server**</span></span>|<span data-ttu-id="897c1-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="897c1-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="897c1-158">Exchange Server sem usar SSL</span><span class="sxs-lookup"><span data-stu-id="897c1-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="897c1-159">Servidor Exchange usando SSL</span><span class="sxs-lookup"><span data-stu-id="897c1-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="897c1-160">Exchange Online como parte do Office 365</span><span class="sxs-lookup"><span data-stu-id="897c1-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="897c1-161">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="897c1-162">O URI do esquema é https://schemas.microsoft.com/powershell/Microsoft.Exchange .</span><span class="sxs-lookup"><span data-stu-id="897c1-162">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="897c1-163">**contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="897c1-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="897c1-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-164"><a name="bk_Kerberos"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="897c1-165">Conectar-se a um runspace remoto em um servidor do Exchange usando a autenticação Kerberos</span><span class="sxs-lookup"><span data-stu-id="897c1-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="897c1-166">O exemplo de código a seguir define o método **GetUsersUsingKerberos** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando a autenticação Kerberos.</span><span class="sxs-lookup"><span data-stu-id="897c1-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="897c1-167">O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="897c1-168">Este método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="897c1-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="897c1-169">**kerberosUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor Kerberos que autenticará o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="897c1-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="897c1-170">O URI será um dos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="897c1-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="897c1-171">**Tabela 2. URIs kerberosUri**</span><span class="sxs-lookup"><span data-stu-id="897c1-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="897c1-172">**Servidor**</span><span class="sxs-lookup"><span data-stu-id="897c1-172">**Server**</span></span>|<span data-ttu-id="897c1-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="897c1-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="897c1-174">Exchange Server sem usar SSL</span><span class="sxs-lookup"><span data-stu-id="897c1-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="897c1-175">Servidor Exchange usando SSL</span><span class="sxs-lookup"><span data-stu-id="897c1-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="897c1-176">**schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="897c1-177">O URI do esquema é https://schemas.microsoft.com/powershell/Microsoft.Exchange .</span><span class="sxs-lookup"><span data-stu-id="897c1-177">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="897c1-178">**credenciais** &ndash; Um objeto [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="897c1-178">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="897c1-179">**contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="897c1-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="897c1-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="897c1-180"><a name="bk_remote"> </a></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="897c1-181">Obter uma lista de usuários de caixa de correio de um runspace remoto</span><span class="sxs-lookup"><span data-stu-id="897c1-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="897c1-182">O exemplo de código a seguir define o método **GetUserInformation** , que retorna uma coleção de instâncias de [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que representam usuários de caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="897c1-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="897c1-183">Este método é chamado pelos métodos **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**e **GetUsersUsingKerberos** para retornar a lista de usuários do servidor remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="897c1-184">Este método requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="897c1-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="897c1-185">**contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="897c1-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="897c1-186">**runspace** &ndash; O runspace remoto estabelecido para o servidor Exchange remoto.</span><span class="sxs-lookup"><span data-stu-id="897c1-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
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

<span data-ttu-id="897c1-187">O método **GetUserInformation** retornará não mais do que _contagem_ usuários de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="897c1-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="897c1-188">Para simplificar o código para este exemplo, o método não filtra ou limita os usuários de caixa de correio que são retornados.</span><span class="sxs-lookup"><span data-stu-id="897c1-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="897c1-189">Confira também</span><span class="sxs-lookup"><span data-stu-id="897c1-189">See also</span></span>

- [<span data-ttu-id="897c1-190">Criar ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="897c1-191">Usar a resposta do cmdlet do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="897c1-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

