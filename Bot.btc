import telebot
import os

TOKEN = os.getenv("
7002866926:AAGIPSVcj1S-gnRVLCMp-LFi9ipqIDQN2Ws")
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "سلام 👋 نام و نام خانوادگی‌تو بفرست:")

@bot.message_handler(func=lambda message: True)
def echo_all(message):
    bot.reply_to(message, "مرسی 🌹 اطلاعاتت ذخیره شد.")

bot.polling()
