== Discord Bot Verification Questions in Plain English ==

=== Application Details ===

In this box, describe your bot's features. Be detailed, and describe what it does, who its audience is, and how it does what it does.
For example for a moderation bot, you'd list what moderation features it has.

== Data Collection ==

Here, document what you store from discord and why you store it. For example, you might be storing nicknames of users - state why. Go into as much detail as possible.

=== What discord data do you store? ===

In this box, list any databases your bot has inside it that store anything *at all* from discord, including snowflake IDs, usernames, channel names, server names.
If it comes from discord and you store it, in a file, a database, in redis, in mongodb or SQL, you should list it here. Be detailed and complete.
Don't put "i don't store anything" unless you really DON'T store anything. **Discord will know!** Very few bots store *nothing*.


=== For what purposes do you store it? ===

Discord are looking for the reasons why you need to keep their data in your bot. For example, if you have a bot that has a ban list, and the ban list is built from
snowflake ids of banned users, this data is stored for purposes of bot functionality and maintaining a ban list. You should list all such purposes and again, be detailed.

=== For how long do you store it? ===

It is acceptable to put here "we store information about that server and its members as long as the bot is on a server" as long as this is honest and truthful. It is also 
acceptable to state that you keep information beyond when the bot is kicked from the server, so long as you have a privacy policy that clearly states how long this is
retained for. For example you may keep audit logs. It is **not acceptable** to retain data forever. Again, it is important to be truthful and detailed. Having a privacy
policy in place before you proceed with this question and publishing it on your bot's website helps a lot, as you can refer to it here with a link.

=== What is the process for users to request deletion of their data? ===

Again, having a privacy policy in place before you answer this question helps a lot. The privacy policy should dictate the answer to this question and you can refer
the bot reviewer to this link, and summarise here. It is normal that for removal of data, you might contact the developer by DM (this is an acceptable answer) or
on the official support server of the bot, via email, or via post. The faster the removal request could be processed if you receive one, the better this will be
for your application. Again, be honest. Don't say you'll remove data if you have no framework in place to remove it. If you don't have something in place to handle
data removal requests from users, **implement something before continuing**!

== Infrastructure ==

=== What systems and infrastructure do you use? ===

You should list here what operating system (and its version), where it's hosted, wether or not it is free hosting, what libraries, programming languages etc you use.
Go into as much detail as possible.

=== How have you secured access to your systems and infrastrucutre? ===

In short: How do you stop the bad guys wrecking your bot? How do you protect access to SSH accounts, stop random people getting access to the bot code? How do you
protect your token (**this is important!**) and how do you vet people who are on your bot's team (if you have a team). Go into detail, and cover every possibility.
Discord want to know that you've considered the security of your bot and taken it as seriously as they do.

=== How can users contact you with security issues ===

This really does need to be documented and made clear not only on this form but on your bot's site. If your bot doesn't have a website now is a good idea to create one.
Be clear, honest, and to the point. For example "users can DM the bot developer (your discord username here) in strictest confidence on the official server". Be aware
that reporting security vulnerabilities needs to be handled in a confidential way to stop others exploiting bugs. There must be a way for users to contact you!

=== Does your application utilize other third-party auth services or connections? if so, which, and why? ===

This field is where you list any additional services your bot talks to, which your users must log in to. For example, if your bot has a way to authenticate with steam,
roblox, google, facebook or **anything that is not discord**. Think if you are using oauth2 for anything other than discord.

It's also useful to list any services here that you use for analytics such as google analytics, facebook pixel etc. Although you don't auth with them they are third party
services and it doesn't harm your application to be up-front about your use of them here.

== Privileged intents ==

If your bot uses privileged intents, you should apply for them. Generally, most bots would make use of the members intent unless they are *stateless*, for example,
if you dont have any need to be looking up member list details. If you do apply for intents, you should indicate why and this is specific to how your bot operates
and outside of the scope of this document. For help with if your bot needs the intents or not you should consider visiting the [discord developers server](https://discord.gg/discord-developers).




