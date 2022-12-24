# Send Gotify Message
## Purpose
A Powershell function that can be called to automate sending Gotify messages. 
## SYNOPSIS
The function was written to address a need to automate notifications coming from other scripts. The function can be called in embedded code or can be ran as a standalone option. 

## Description
```
Language: Powershell
IDE: SublimeText with Powershell package
Author: Oscar J. Rivera
```
## Function Send-GotifyMessage
```
./Send-GotifyMessage.ps1
```

## Parameters
"The publically accessible uri to the Gotify server."*
> *-GotifyServer*

"The predefined app token on the gotify server"
> *-AppToken*

"The title of the message to be delivered"
> *-Title* 

"The message you want to send as the Gotify Notification"
> *-Message*

"The priority of the message to be sent"
>*-Priority*

+ The last one is a validatedset with the following options    
    + Min: Less than 1
    + Low: 1 - 3 
    + Normal: 4 - 7
    + High: Greater than 7

# Syntax
`Send-GotifyMessage -GotifyServer <https://somegotifyserver.com> -Apptoken <The app token> -Title <"Title">  -Message <"Some Message"> -Priority <High>`

# Examples

## Example 1
`Send-GotifyMessage -GotifyServer https://somegotifyserver.com -Apptoken AnPfM1cineEB32 -Title "This is a Title"  -Message "This is the Message" -Priority High `

# NOTES
--------------------
