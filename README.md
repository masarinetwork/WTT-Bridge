# WTT-Bridge (WIP)

A Bot that forwards conversations and media from Whatsapp to Telegram. 
To make it as seamless as possible, the bot will simulate conversations on Telegram by creating a separate group chat for each Whatsapp conversation and forward the messages accordingly.

>TODO screenshot



## Configuration

You have to fill out all values in the config.json to run the bot:

#### Telegram: 

- "token": Talk to https://telegram.me/botfather and create a bot to get a token

- "api_id" and "api_hash": Visit https://my.telegram.org/

- "owner": You can talk to @getidsbot to get your telegram ID 

#### Whatsapp:

- "phonenumber": your phone number with country code but without + or 0 at the beginning

- "client_static_keypar": to get your keypair do the following: 

1. Run ```yowsup-cli registration --requestcode sms --config-phone 49XXXXXXXXXXX --config-cc 49 --config-mcc 228 --config-mnc 02``` to start the registration. 
You can find your MMC and MNC codes here:
https://en.wikipedia.org/wiki/Mobile_country_code

2. When you receive the verification sms, run ```yowsup-cli registration --register 123456 --config-phone 49XXXXXXXX``` to verify your number.

3. If the verification was successfull you should now be able to see your client_static_keypair in the console. Copy it into the config.json 



## Notes
 