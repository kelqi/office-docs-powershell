---
external help file:
applicable: SharePoint Server 2013, SharePoint Server 2016, SharePoint Online
schema: 2.0.0
author: vesajuvonen
ms.author: vesaj
ms.reviewer:
---
# Add-PnPWikiPage

## SYNOPSIS
Adds a wiki page

## SYNTAX 

### WithContent
```powershell
Add-PnPWikiPage -Content <String>
                -ServerRelativePageUrl <String>
                [-Web <WebPipeBind>]
                [-Connection <SPOnlineConnection>]
```

### WithLayout
```powershell
Add-PnPWikiPage -Layout <WikiPageLayout>
                -ServerRelativePageUrl <String>
                [-Web <WebPipeBind>]
                [-Connection <SPOnlineConnection>]
```

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
Add-PnPWikiPage -PageUrl '/sites/demo1/pages/wikipage.aspx' -Content 'New WikiPage'
```

Creates a new wiki page '/sites/demo1/pages/wikipage.aspx' and sets the content to 'New WikiPage'

## PARAMETERS

### -Content


```yaml
Type: String
Parameter Sets: WithContent

Required: True
Position: Named
Accept pipeline input: False
```

### -Layout


```yaml
Type: WikiPageLayout
Parameter Sets: WithLayout

Required: True
Position: Named
Accept pipeline input: False
```

### -ServerRelativePageUrl
The server relative page URL

```yaml
Type: String
Parameter Sets: (All)
Aliases: PageUrl

Required: True
Position: Named
Accept pipeline input: False
```

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: SPOnlineConnection
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

### -Web
This parameter allows you to optionally apply the cmdlet action to a subweb within the current web. In most situations this parameter is not required and you can connect to the subweb using Connect-PnPOnline instead. Specify the GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)

Required: False
Position: Named
Accept pipeline input: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](http://aka.ms/sppnp)
