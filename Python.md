## Datetime now with timezone
'''python
from datetime import datetime
import pytz
tz_colombo = pytz.timezone('Asia/Colombo')
datetime.now(tz_colombo).strftime('%Y-%m-%d %H:%M:%S')
'''
