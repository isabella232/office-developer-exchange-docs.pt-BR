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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435706"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a>Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange

Saiba como usar os cmdlets do Shell de gerenciamento do Exchange para criar uma ferramenta que retorna uma lista de usuários de caixa de correio do Exchange.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365 
  
Obter uma lista de usuários do Exchange Online, do Exchange Online como parte do Office 365 ou de uma versão do Exchange que comece com o Exchange 2013 usando uma ferramenta gerenciada que chama um cmdlet do Shell de gerenciamento do Exchange é um processo de duas etapas. Primeiro, você estabelece um runspace remoto em um servidor Exchange; em seguida, execute o cmdlet para recuperar as informações do usuário no runspace remoto. 

Para se conectar ao runspace remoto, você precisa autenticar com o servidor do Exchange usando o esquema de autenticação que atende aos requisitos de segurança da sua organização. 

Este artigo fornece exemplos de código que você pode usar para configurar um runspace remoto e executar um cmdlet do Shell de gerenciamento do Exchange para obter uma lista de usuários de um servidor Exchange.

<a name="bk_prerequisites"> </a>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a>Pré-requisitos para obter uma lista de usuários de caixa de correio

Para executar essa tarefa, você precisa de uma referência para os seguintes namespaces:
  
- **System. Collections. ObjectModel**
- **System. Management. Automation**
- **System. Management. Automation. Remoting**
- **System. Management. Automation. Runspaces**
    
> [!NOTE]
>  Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência ao assembly System. Management. Automation. dll para o projeto. O assembly pode ser encontrado em um dos seguintes locais:
> - Para os sistemas operacionais Windows XP e Windows Vista, o diretório de instalação do Windows PowerShell ($PSHOME).
> - Para os sistemas operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\ GAC_MSIL \System.Management.Automation. 
  
Não carregue o snap-in de gerenciamento do Exchange 2013 no runspace em computadores que executam aplicativos que automatizam os cmdlets do Shell de gerenciamento do Exchange. Em vez disso, o aplicativo deve criar um runspace remoto, conforme descrito posteriormente neste artigo.

<a name="bk_gettinglistmailbox"> </a>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a>Conectar-se a um runspace remoto em um servidor Exchange

O método que você usa para se conectar a um runspace remoto para usar um cmdlet do Shell de gerenciamento do Exchange varia com base no esquema de autenticação que você está usando. Esta seção fornece exemplos de código que mostram como se conectar a um runspace remoto quando você estiver usando um método de autenticação listado na tabela a seguir.
  
|**Método de autenticação**|**Aplica-se a**|**URI**|
|:-----|:-----|:-----|
|[Conectar-se a um runspace remoto no Exchange Online usando a autenticação básica](#bk_basic) <br/> |Servidores do Exchange Online  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[Conectar-se a um runspace remoto usando a autenticação de certificado](#bk_cert) <br/> |Servidores locais do Exchange Online e do Exchange  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[Conectar-se a um runspace remoto em um servidor do Exchange usando a autenticação Kerberos](#bk_Kerberos) <br/> |Servidores locais do Exchange Online e do Exchange  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<a name="bk_basic"> </a>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a>Conectar-se a um runspace remoto no Exchange Online usando a autenticação básica

O exemplo de código a seguir define o método **GetUsersUsingBasicAuth** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto do Exchange Online usando a autenticação básica. O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.
  
Este método requer os seguintes parâmetros:
  
-  **liveIDConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor Exchange Online que autenticará o aplicativo. Se o Exchange Online estiver em execução no Office 365, o URI será `https://outlook.office365.com/PowerShell-LiveID` ; caso contrário, o URI é `https://<servername>/PowerShell-LiveID` . 
    
-  **schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange. O URI do esquema é `https://schemas.microsoft.com/powershell/Microsoft.Exchange` . 
    
-  **credenciais** &ndash; Um objeto [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo. 
    
-  **contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados. 
    
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

<a name="bk_cert"> </a>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a>Conectar-se a um runspace remoto usando a autenticação de certificado

O exemplo de código a seguir define o método **GetUsersUsingCertificate** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando um certificado. O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.
  
Este método requer os seguintes parâmetros:
  
-  **impressão digital** &ndash; Uma cadeia de caracteres que contém a impressão digital do certificado usado para autenticar o aplicativo. 
    
-  **certConnectionUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor que autenticará o certificado. O URI será um dos listados na tabela a seguir. 
    
    **Tabela 1. URIs certConnectionUri**

    |**Servidor**|**URI**|
    |:-----|:-----|
    |Exchange Server sem usar SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Servidor Exchange usando SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
    |Exchange Online como parte do Office 365  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- **schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange. O URI do esquema é https://schemas.microsoft.com/powershell/Microsoft.Exchange . 
    
- **contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados. 
    
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

<a name="bk_Kerberos"> </a>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a>Conectar-se a um runspace remoto em um servidor do Exchange usando a autenticação Kerberos

O exemplo de código a seguir define o método **GetUsersUsingKerberos** , que cria um runspace do Shell de gerenciamento do Exchange em um servidor remoto usando a autenticação Kerberos. O método chama o método **GetUserInformation** , conforme definido na seção [obter uma lista de usuários de caixa de correio de um runspace remoto](#bk_remote), para retornar uma lista de usuários no servidor remoto.
  
Este método requer os seguintes parâmetros:
  
- **kerberosUri** &ndash; Uma cadeia de caracteres que contém o URI do servidor Kerberos que autenticará o aplicativo. O URI será um dos listados na tabela a seguir. 
    
    **Tabela 2. URIs kerberosUri**

    |**Servidor**|**URI**|
    |:-----|:-----|
    |Exchange Server sem usar SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Servidor Exchange usando SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- **schemaUri** &ndash; Uma cadeia de caracteres que contém o URI do documento de esquema que define o esquema do Shell de gerenciamento do Exchange. O URI do esquema é https://schemas.microsoft.com/powershell/Microsoft.Exchange . 
    
- **credenciais** &ndash; Um objeto [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que contém as credenciais do usuário que está executando o aplicativo. 
    
- **contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados. 
    
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

<a name="bk_remote"> </a>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a>Obter uma lista de usuários de caixa de correio de um runspace remoto

O exemplo de código a seguir define o método **GetUserInformation** , que retorna uma coleção de instâncias de [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) que representam usuários de caixa de correio do Exchange. Este método é chamado pelos métodos **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**e **GetUsersUsingKerberos** para retornar a lista de usuários do servidor remoto. 
  
Este método requer os seguintes parâmetros:
  
- **contagem** &ndash; O número de usuários de caixa de correio do Exchange a serem retornados. 
    
- **runspace** &ndash; O runspace remoto estabelecido para o servidor Exchange remoto. 
    
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

O método **GetUserInformation** retornará não mais do que _contagem_ usuários de caixa de correio. Para simplificar o código para este exemplo, o método não filtra ou limita os usuários de caixa de correio que são retornados. 
  
## <a name="see-also"></a>Confira também

- [Criar ferramentas do Shell de gerenciamento do Exchange](create-exchange-management-shell-tools.md)   
- [Usar a resposta do cmdlet do Shell de gerenciamento do Exchange](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

