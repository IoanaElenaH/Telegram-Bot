# **Telegram-Bot**
Node-red telegram bot that sends info about the weather and a random photo.

## **Running the project**
You must have node-red installed to run this project.

Open Telegram and search for “BotFather”. Using this bot you can create, delete and manage all your bots( /newbot->/mybot ). For a description of the Bot API, see this page:

https://core.telegram.org/bots/api

Use Node-RED to retrieve weather data from https://openweathermap.org/, and send it to a Telegram group through a bot. **For Node-red, I installed the following [node](https://flows.nodered.org/node/node-red-contrib-telegrambot).**

### **Desired API**

**OpenWeather**

The bot should accept commands beginning with /. Each command should return some weather information fetched on OpenWeather.

Generate your own API key for this service.

•	Sign up at https://home.openweathermap.org/

•	Go to the https://home.openweathermap.org/api_keys tab

•	Use already generated key or generate new one API key

•	Go to the https://openweathermap.org/current

We are interested in this API call:

http://api.openweathermap.org/data/2.5/weather?q={city}
The response from this request you can see here. You can adjust the request to the comfortable units, by default it used Kelvin temperature, to change it to Celsium just use the following request.

http://api.openweathermap.org/data/2.5/weather?q={city}&units=metric

Keep in mind that the requests above also should contain your API key as part of URL, so the final request would be following

http://api.openweathermap.org/data/2.5/weather?q={city}&units=metric&&appid={api_key}

**Unsplash**

https://unsplash.com/documentation

https://www.pluralsight.com/guides/using-the-unsplash-api




[Flow](https://github.com/Xiaxue1707/Telegram-Bot/files/8648008/Flows_Screenshot.pdf)
