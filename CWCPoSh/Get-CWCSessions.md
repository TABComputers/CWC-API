# Get-CWCSessions
## SYNOPSIS
Will return a list of sessions.
## SYNTAX
```powershell
Get-CWCSessions [-Server] <Object> [-User] <Object> [-Password] <Object> [-Type] <Object> [[-Group] <Object>] [[-Search] <Object>] [[-Limit] <Object>] [<CommonParameters>]
```
## DESCRIPTION
Allows you to search for access or service sessions.
## PARAMETERS

### -Server &lt;Object&gt;
The address to your Control server. Example 'https://control.labtechconsulting.com' or 'http://control.secure.me:8040'
```
Required?                    true
Position?                    1
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -User &lt;Object&gt;
User to authenticate against the Control server.
```
Required?                    true
Position?                    2
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -Password &lt;Object&gt;
Password to authenticate against the Control server.
```
Required?                    true
Position?                    3
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -Type &lt;Object&gt;
The type of session Support/Access
```
Required?                    true
Position?                    4
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -Group &lt;Object&gt;
Name of session group to use.
```
Required?                    false
Position?                    5
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -Search &lt;Object&gt;
Limit results with search patern.
```
Required?                    false
Position?                    6
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
``` 
### -Limit &lt;Object&gt;
Limit the number of results returned.
```
Required?                    false
Position?                    7
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
```
## INPUTS

## OUTPUTS
ConnectWise Control session objects
## NOTES
Version:        1.0
Author:         Chris Taylor
Creation Date:  10/10/2018
Purpose/Change: Initial script development
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Get-CWCAccessSessions -Server $Server -User $User -Password $Password -Search "server1" -Limit 10

Will return the first 10 access sessions that match 'server1'.
```

