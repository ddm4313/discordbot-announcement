import discord, time, datetime, asyncio
from time import gmtime, strftime
import ctypes

class MyClient(discord.Client):
    async def on_ready(self):
        print(f"[#] User: {self.user}")
        game = discord.Game("Activity")
        await client.change_presence(status=discord.Status.online, activity=game)
    async def on_message(self, message):
        welcome_channel = client.get_guild('channel token')
        # write !start to start the script
        if message.content == "!start":
            while 2 > 1:
                await message.channel.purge() # purges everythin
                day = strftime("%A", gmtime())
                appro_date = strftime("%c", gmtime())
                # it announces what day it is, simple but nice.
                await message.channel.send(f"@everyone It's {day}", embed=embed)
                print(f"[#] Announcement made at {appro_date}")
                # sleeps for 12hrs
                await asyncio.sleep(57600)

client = MyClient()
client.run('# bot token')
