# bitcoin
비트코인 자동매매 알고리즘입니다(빗썸)
import time
from datetime import datetime
import datetime

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

while True:
    now = datetime.now()
    now = datetime.datetime.now()
    if now == mid : 
        print("이제 다시 시작이야 젊은날의 꿈이여")
        now = datetime.now()
        mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
        now = datetime.datetime.now()
        mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

    print(now, "vs", mid)
    time.sleep(1)
import time
from datetime import datetime
import datetime

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

while True:
    now = datetime.now()
    now = datetime.datetime.now()
    if mid < now < mid + datetime.delta(seconds=10) : 
        print("이제 다시 시작이야 젊은날의 꿈이여")
        mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
        mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

    time.sleep(1) 
import time
import pybithumb
from datetime import datetime
import datetime

def get_target_price(ticker):
    df = pybithumb.get_ohlcv("BTC")
def get_target_price(ticker):
    target = today_open + (yesterday_high - yesterday_low) * 0.5
    return target

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
target_price = get_target_price("BTC")

while True:
    now = datetime.now()
    now = datetime.datetime.now()
    if mid < now < mid + datetime.delta(seconds=10) : 
        target_price = get_target_price("BTC")
        mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
        mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

    current_price = pybithumb.get_current_price("BTC")
    print(current_price)
import time
import pybithumb
from datetime import datetime
import datetime

con_key = "81dd5f25e5daa70b2fff603901d2c09c"
sec_key = "82333efegeg9eg3e77c573weg34af17a"
def get_target_price(ticker):
    target = today_open + (yesterday_high - yesterday_low) * 0.5
    return target

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
target_price = get_target_price("BTC")

while True:
    now = datetime.now()
    now = datetime.datetime.now()
    if mid < now < mid + datetime.delta(seconds=10): 
        target_price = get_target_price("BTC")
        mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
        mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)

    current_price = pybithumb.get_current_price("BTC")
    if current_price > target_price:
import time
import pybithumb
from datetime import datetime
import datetime

con_key = "81dd5f25e5daa70b2fff603901d2c09c"
sec_key = "82333efegeg9eg3e77c573weg34af17a"
def sell_crypto_currency(ticker):
    unit = bithumb.get_balance(ticker)[0]
    bithumb.sell_market_order(ticker, unit)

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
target_price = get_target_price("BTC")

while True:
    now = datetime.now()
    now = datetime.datetime.now()
    if mid < now < mid + datetime.delta(seconds=10): 
        target_price = get_target_price("BTC")
        mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
        mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
        sell_crypto_currency("BTC")

    current_price = pybithumb.get_current_price("BTC")
    if current_price > target_price:
        buy_crypto_currency("BTC")

    time.sleep(1) 
    time.sleep(1)
import time
import pybithumb
from datetime import datetime
import datetime

with open("bithumb.txt") as f:
    lines = f.readlines()
def sell_crypto_currency(ticker):
    unit = bithumb.get_balance(ticker)[0]
    bithumb.sell_market_order(ticker, unit)

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
target_price = get_target_price("BTC")

while True:
    try:
        now = datetime.now()
        now = datetime.datetime.now()
        if mid < now < mid + datetime.delta(seconds=10): 
            target_price = get_target_price("BTC")
            mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
            mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
            sell_crypto_currency("BTC")

        current_price = pybithumb.get_current_price("BTC")
import time
import pybithumb
from datetime import datetime
import datetime

with open("bithumb.txt") as f:
    lines = f.readlines()
def get_yesterday_ma5(ticker):
    ma = close.rolling(5).mean()
    return ma[-2]

now = datetime.now()
mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
now = datetime.datetime.now()
mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
ma5 = get_yesterday_ma5("BTC")
target_price = get_target_price("BTC")

while True:
    try:
        now = datetime.now()
        now = datetime.datetime.now()
        if mid < now < mid + datetime.delta(seconds=10): 
            target_price = get_target_price("BTC")
            mid = datetime(now.year, now.month, now.day) + datetime.timedelt(1)
            mid = datetime.datetime(now.year, now.month, now.day) + datetime.timedelta(1)
            ma5 = get_yesterday_ma5("BTC")
            sell_crypto_currency("BTC")
