- 👋 Hi, I’m @APLPlayz
- 📫 How to reach me for any questions, Discord: APLPlayz#8615 or Twitter: @APL_Playz

Enjoy this list of Twitch Commands!

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
* ```${sender} works like user in streamlabs```
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
