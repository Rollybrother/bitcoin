# bitcoin
비트코인 자동매매 알고리즘입니다(빗썸)
@@ -1,15 +1,15 @@
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
 10  ch06/06_15.py 
@@ -1,13 +1,13 @@
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
  10  ch06/06_16.py 
@@ -1,6 +1,6 @@
import time
import pybithumb
from datetime import datetime
import datetime

def get_target_price(ticker):
    df = pybithumb.get_ohlcv("BTC")
@@ -12,15 +12,15 @@ def get_target_price(ticker):
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
  10  ch06/06_17.py 
@@ -1,6 +1,6 @@
import time
import pybithumb
from datetime import datetime
import datetime

con_key = "81dd5f25e5daa70b2fff603901d2c09c"
sec_key = "82333efegeg9eg3e77c573weg34af17a"
@@ -16,15 +16,15 @@ def get_target_price(ticker):
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
  12  ch06/06_18.py 
@@ -1,6 +1,6 @@
import time
import pybithumb
from datetime import datetime
import datetime

con_key = "81dd5f25e5daa70b2fff603901d2c09c"
sec_key = "82333efegeg9eg3e77c573weg34af17a"
@@ -27,19 +27,19 @@ def sell_crypto_currency(ticker):
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
  10  ch06/06_19.py 
@@ -1,6 +1,6 @@
import time
import pybithumb
from datetime import datetime
import datetime

with open("bithumb.txt") as f:
    lines = f.readlines()
@@ -29,16 +29,16 @@ def sell_crypto_currency(ticker):
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
  10  ch06/06_20.py 
@@ -1,6 +1,6 @@
import time
import pybithumb
from datetime import datetime
import datetime

with open("bithumb.txt") as f:
    lines = f.readlines()
@@ -35,17 +35,17 @@ def get_yesterday_ma5(ticker):
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
