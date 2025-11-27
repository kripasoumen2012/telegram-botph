# Telegram ESCROW Bot (Python)
# Paste your bot token in the TOKEN variable below and host on Railway/Render for 24/7 uptime.

from telegram import Update
from telegram.ext import ApplicationBuilder, CommandHandler, ContextTypes

TOKEN = "8332060736:AAG34dmawIkLrtDG3JevddII_TZS-Yu-g_8"

# /start command
async def start(update: Update, context: ContextTypes.DEFAULT_TYPE):
    message = (
        "🤖 WELCOME TO ESCROW BOT💙\n"
        "Escrow is our passion\n"
        "🔗 Join Our Telegram Group For Any Escrow Service\n"
        "👉 Group Link: https://t.me/+R4gqLnMw8aw4Zjg"
    )
    await update.message.reply_text(message)

# /owner command
async def owner(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await update.message.reply_text("@Ccsellersg")

# /dealinfo command
async def dealinfo(update: Update, context: ContextTypes.DEFAULT_TYPE):
    message = (
        "DEAL INFO : \n"
        "BUYER :  \n"
        "SELLER :  \n"
        "DEAL AMOUNT :\n"
        "TIME TO COMPLETE DEAL :\n"
        "PAYMENT METHOD :\n"
        "ESCROW TILL :\n\n"
        "WARNING ⚠️ READ CAREFULLY \n"
        "DON'T PAY TO ANYONE IN YOUR DM RELATED TO ESCROWS\n"
        "CROSS CHECK ADMIN's TAG BEFORE PROCEEDING"
    )
    await update.message.reply_text(message)

# /qr command
async def qr(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await update.message.reply_text("https://ibb.co/yctNq0Rq\nPay and send ss and message privately")

# MAIN FUNCTION
async def main():
    app = ApplicationBuilder().token(TOKEN).build()

    app.add_handler(CommandHandler("start", start))
    app.add_handler(CommandHandler("owner", owner))
    app.add_handler(CommandHandler("dealinfo", dealinfo))
    app.add_handler(CommandHandler("qr", qr))

    print("BOT IS RUNNING...")
    await app.run_polling()

if __name__ == "__main__":
    import asyncio
    asyncio.run(main())
