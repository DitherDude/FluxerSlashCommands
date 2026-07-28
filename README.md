## MISC
* Blstmo's specsheet https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1525162657806557184
* Shardion's summary https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1524528985743040512
* UI/UX overview https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530253121631035392
* GH discussion https://github.com/orgs/fluxerapp/discussions/1339 ; locked https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1524507929284190208

## Privacy-focused
* Slash command bots will 'ride' on the command executor, invoking the action on their behalf https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529874318656282624 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526618333770686464
  - invalidates https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526614873226616832
* This is done via obtaining a one-time-use 'privelege' token to act on behalf of the user https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526619534486675456
* Oauth2? https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526615792416727040
* duration-based token? https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526619937118887936
* UI/UX for notifing executor of invoken action
  - NOT popup https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526619938687557632
  - The first time the command is run (per executor per community) https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526620378623909888
  - before execution (in command autocomplete list) https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526620622371692544
* Bots therefore are permissionless by default https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526618914350440448
* insight is still somewhat needed https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526616869459468288
* Bots will by-default **not** have message read permissions
* Bots with read message perms have a notice https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531398357002493952

## AutoMod
* a specific subset of bots that _can_ read messages. Privacy etc. TBD. Blocked by pending Fluxer API changes? https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526619896069234688 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531607698485813248

## Discord compatibility
* atp drop compatibility; allows focus on privacy-oriented features than bending to discord's impl https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531606151509057536
  - INITIALLY pro-compat; invalidates https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1523857070158258176 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1524756534167347200 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1528421561785131008 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531355020207857664

## Fluxer Native bot alternatives
* common bot features like Starboard/Message Quoting/Message Purge could be baked into Fluxer https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531612522455506944
* upto Fluxer OSS community to maintain https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531617860936278016
* Leveling TBD https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531614590998159360

## Command prefixes
* still discussing, current sentiment AGAINST https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529882845848281088
  - INITIALL pro-prefixes; invalidates https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1525181680053133312 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1528339378764521472
* S/E/D collision https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1528269525617745920
* three-letter prefix https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530055435376140288
* shift === bad https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530056134084272128

## Multi-select
* ability for a command argument to be a list of items

## Moderation dashboard
* Fluxer guild settings should support the ability to control guild-specific bot settings; currently discord bots redirect to webdashboards https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526620881793589248
* I'm too tired to summarise this wall of text sorry Lilith https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530253109610160128

## Command heirarchy
* If two commands share a name, which appears above; conflicting opinions:
  - user specified https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1525162657806557184
  - user specified (server compute) https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529882810305748992
  - guild specified
  - most recent at the top

## Command Registration
* pain point to manage/revoke/register commands
  - proposal for clients to cache/hash command list, and bots push updates as needed https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1523847742961491968
  
## Command Gating/Guild command controls
* hide commands if insufficient permissions https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1523854692193411072
* requires renting highway billboards to advertise https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1524513865801408512
* fine-tuning command availability https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1525182454535561216 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530422380327870464
* command renaming (to avoid collisions) https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526613375214166016
* cannot action a user higher than both the role of the executor and the bot https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1528133793473372160

## Command Categories
* Note sure what became of this https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1523870904604434432


## Boolean DSL
* NO https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529874318656282624
* YES https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529882551831764992

## Chips (I have no fucking clue what this means)
* Cap at 50 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529874318656282624

## Bot hosting
* instance hosts https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529879596453863424
* Fluxer hosts https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529886887907434496
* Fluxer hosts can guarantee data safety https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530096629506383872

## Auditing
* every action but with filters https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1529885851922735104
* no pressure to get it right https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531614321237303296
* custom categories
  - YES https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531622291463479296
  - NO (Fluxer predefined categories) https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531621912206123008
* very good https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531623553336614912
  
## Ephemeral Messages
* optionally moderators could receive too https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1531620874900217856

## Lolz
* Moon Landings, because anything's possible https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1526615480704442368
* Shardion likes beans https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1523870904604434432 https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1525178101569429504
* sleep-texting https://web.canary.fluxer.app/channels/1427764813854588940/1523845240144801793/1530254095607144448

