<div align="center">
  <img src="https://github.com/Flummidill/SimpleMerchantEdit/blob/HEAD/icons/SimpleMerchantEdit-250x250.png?raw=true" alt="VillagerEdit-Icon">
  
  <h1>SimpleMerchantEdit</h1>
  <a href="https://modrinth.com/plugin/villager_edit/versions">
    <img src="https://img.shields.io/modrinth/dt/villager_edit?style=for-the-badge&label=Downloads&color=29A100">
  </a>
</div>


## 🎯 Features
- **Self Whitelisting by Players**  
They can whitelist themselves by Linking their Discord and Minecraft Accounts.
This removes the need for manual Whitelisting and can still be restricted by using an Access Role.

- **Fast & Easy Account Linking**
It only takes a few Seconds and is very Easy to do.
Generate a code on Discord, enter it in Minecraft, and you’re already Done.

- **Automatic Role-Based Whitelisting**  
When an Account is Linked, the Player automatically receives the configured Whitelist Role on Discord.
This makes managing Server Access to Players very Simple.

- **Admin Account Management**  
Admins can easily remove Linked Accounts by either Kicking the User from the Discord Server or taking away their Whitelist/Access Role.
This makes Moderation and Account Management Simpler and Efficient.

- **Automatic Nicknames**  
When a Player Links their Account, their Discord Nickname is automatically Updated to their Minecraft Username every 15 Minutes.
This makes Identifying Players on the Discord Server Effortless and helps with Moderation.


<hr/>


### DC-Commands:
```
/linkmc - Get your Linking/Auth Code
/unlinkmc - Unlink your Minecraft Account
```

### MC-Commands:
```
/linkdc <Auth-Code> - Link your Discord Account
/unlinkdc - Unlink your Discord Account
```

### Admin Commands (DC + MC):
```
/forceunlink <Player> [<Remove-Access-Role>] - Unlink another Player's Account
```

### Permissions:
```
dcwhitelistlinker.linkdc (Default: true)
dcwhitelistlinker.unlinkdc (Default: true)
dcwhitelistlinker.forceunlink (Default: false)
```

### Config:
```
bot-token - Your Discord Bot-Token
server-id - ID of your Discord Server
whitelist-role-id - ID of the Whitelist Role
require-access-role - If Linking should require a specific Access Role
remove-access-role-on-unlink - If the Access Role should also be removed when UnLinking
access-role-id - ID of the Access Role
use-linking-channel - If Linking should be restricted to a specific Linking Channel
linking-channel-id - ID of the Linking Channel
```