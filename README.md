📫 How to reach me for any questions, Discord: APLPlayz#8615 or Twitter: @APL_Playz
Enjoy this list of Twitch Commands!

# Twitch:
## Commands for EVERYONE:
* ```/mods``` - This command will display a list of all chat moderators for that specific channel
* ```/vips``` - This command will display a list of VIPs for that specific channel
* ```/color [colorname]``` - Allows you to change the color of your username.
  * Color Names Available: (Blue, Coral, DodgerBlue, SpringGreen, YellowGreen, Green, OrangeRed, Red, GoldenRod, HotPink, CadetBlue, SeaGreen, Chocolate, BlueViolet, and Firebrick)
* ```/block {username}``` - Allows you to block all messages from a specific user in chat and whispers
  * (In chat, users can also click on a username and then on the Block button on the user badge that appears)
* ```/unblock {username}``` - This command will allow you to remove users from your block list that you previously added.
Users can also click on the Unignore button which replaces the Block button.
* ```/me ______``` - This command will remove the colon that typically appears after your chat name and italicize your message text
* ```/disconnect``` - This command will simply disconnect you from the chat server.
  * To reconnect, simply refresh the page.
* ```/w {username} ______``` - This command sends a private message to another user on Twitch.

## Commands for Broadcasters and all Moderators
* ```/user {username}``` - This command opens a user’s profile card where channel moderators and streamers can share channel-specific moderation comments, see when the user made their account, and view that user's channel-specific chat, timeout, and ban history.
* ```/timeout {username} [seconds]``` - This command allows you to temporarily ban someone from the chat room for 10 minutes by default.
  * (This will be indicated to yourself and the temporarily banned subject in chat on a successful temporary ban. A new timeout command will overwrite an old one)
  * (The command also supports banning for a specific set of time via the optional SECONDS value)
* ```/ban {username}``` - This command will allow you to permanently ban a user from the chat room.
  * (Can also do this by clicking the Cancel symbol either directly in chat or on the user badge which appears when clicking on a username.)
* ```/unban {username}``` - This command will allow you to lift a permanent ban on a user from the chat room.
  * (You can also use this command to end a ban early; this also applies to timeouts)
* ```/slow [seconds]``` - This command allows you to set a limit on how often users in the chat room are allowed to send messages (rate limiting).
* ```/slowoff``` - This command allows you to disable slow mode if you had previously set it
* ```/followers``` - This command allows you or your mods to restrict chat to all or some of your followers, based on how long they’ve followed
  * (From 0 minutes (all followers) to 3 months)
* ```/followersoff``` - This command will disable followers only mode if it was previously enabled on the channel.

## Commands for Channel Editor and Broadcaster
* ```/commercial``` - An Affiliate and Partner command that runs a commercial, for 30 seconds, for all of your viewers.
* ```/commercial [30|60|90|120|150|180]``` - An Affiliate and Partner command that runs a commercial, for the seconds specified, for all of your viewers.
* ```/goal``` - This command will enable you to manage a sub or follower goal
* ```/prediction``` - This command will enable you to manage predictions
* ```/host {channel}``` - This command will allow you to host another channel on yours (embedded video player)
* ```/unhost``` - This command will send the viewer to another live channel
* ```/raid {channel}``` - This command will send the viewer to another live channel
* ```/unraid``` - This command will cancel the raid
* ```/marker [description]``` - Adds a stream marker at the current timestamp.
  * (With an optional description, max 140 characters)

## Commands for Broadcaster
* ```/mod {username}``` - This command will allow you to promote a user to a channel moderator allowing them to have access to all of the above commands and features
* ```/unmod {username}``` - This command will allow you to demote an existing moderator back to viewer status
  * (Removing their moderator abilities)
* ```/vip {username}``` - This command will grant VIP status to a user
* ```/unvip {username}``` - This command willl revoke VIP status from a user.


# Streamlabs
## Variables:
* ``` {target.name} ```
* ```{user} ```
  * ```  {user.name} ```
  * ```  {user.time} ```
* ```{touser}``` - Adds an @ before the user's name
  * ```{touser.name}```
  * ```{touser.followage}``` - Shows how long the user has been following the channel
* ```{uptime}``` - Shows how long the user has been currently streaming
* ```{channel}```
  * ```{channel.name}``` - Streamer's name
  * ```{channel.followers}``` - Current followers for the streamer
  * ```{channel.subs}``` - Current subs for the streamer
* ```{randnum.minNumber-MaxNumber}``` - Outputs a random number between the range you give it, checkout examples to see how to use it

## Commands:
* Add command
  * ```!addcommand !commandName ______```
* Edit command
  * ```!editcommand !commandName ______```
* Remove command
  * ```!removecommand !commandName```
* Hug command
  * ```!addcommand !hug {user.name} is giving {target.name} a big warm hug.```
* Uptime command
  * ```!editcommand !uptime ______ has been streaming for {uptime}!!!```
* Sets custom title of the stream on Twitch
  * ```!settitle Title of Stream :D```
* Tells user in Twitch chat how many followers the streamer has at the time of use
  * ```!addcommand !followers Dj Little Rock has {channel.followers} followers! :pog:```
* Tells user how long they have been following the channel
  * (If unfollowed and refollowed, it will show the amount of time since refollow)
    * ```!addcommand !followage {touser.name} has been following {channel. name} for {touser.followage}```
* Tells use in Twitch chat how many subscribers the streamer has at the time of use
  * ```!editcommand !subs DjNotes has {channel.subs} subscribers! <3```
* Vibe command (Percentage)
  * ```!addcommand !vibe {user.name} got a {randnum.0-100}% on their vibin test!```


# StreamElements
## Variables:
* ```${sender}``` - works like user in Streamlabs
* ```${user} or ${1}```
* ```${touser}```
* ```${uptime}```
* ```${channel}```
  * ```${channel.followers}``` - Current followers for the streamer
  * ```${channel.subscribers}``` - Current subs for the streamer
  * ```${channel.alias}``` - Streamer's name
* ```${random.minNumber-MaxNumber}``` - Outputs a random number between the range you give it

## Commands:
* Add command
  * ```!command add !commandName ______```
* Edit command
  * ```!command edit !commandName ______```
* Remove command
  * ```!command remove !commandName```
* Hug command
  * ```!command add !hug {sender} is hugging {user}```
* Tells user in Twitch chat how many subscribers the streamer has at the time of use
  * ```!command add !subs ${channel.alias} has ${channel.subscribers}!!```
* Shoutout command
  * ```!command add !so Checkout ${user} at www.twitch.tv/${user}```
* Tells user in Twitch chat how many followers the streamer has at the time of use
  * ```!command add !followers ${channel.alias} has ${channel.followers}!!```
* Complex Shoutout command
  * (Colorful and also shows what game they were playing last)
    * ```!command edit !so /me $(user) was last seen in "$(game $(user))" at twitch.tv/$(user) ! Go check them out!```
* Vibe command (Percentage)
  * ```!command add !vibe ${user} is ${random.0-100}% vibin```


# Nightbot
## Variables:
* ```$(user)```
* ```$(touser)```

## Commands:
* Add command
  * ```!command add !commandName ______```
* Edit command
  * ```!command edit !commandName ______```
* Remove command
  * ```!command remove !commandName```
* User activated command for bits
* *(Give thanks to someone who donates bits)
!command edit !bits /me Thank you so much for the bitties $(touser) bleedPurple VirtualHug
* Tells user in Twitch chat how many followers the streamer has at the time of use
!command add !followers $(channel) has $(twitch $(channel) "{{followers}} followers!")
* Gives a random number
!command add !randNum $(eval Math.floor(Math.random() * 101))
* Vibe command
!command add !vibeTest /me $(user) got a $(eval Math.floor(Math.random() * 101))% on their vibe test :O
