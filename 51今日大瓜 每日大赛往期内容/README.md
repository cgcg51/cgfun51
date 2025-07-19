### [👉👉点此进入♥观看入口👈👈](http://a.d44k.cc/hl.html)
<br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br>
import datetime
 
class CaffeineTracker:
    def __init__(self):
        self records = []  # 存储咖啡因摄入记录
        self daily_limit = 400  # 每日建议最大摄入量(mg)
    
    def add_consumption(self, drink_type, amount_mg, time=None):
        """添加咖啡因摄入记录"""
        if time is None:
            time = datetime datetime now()
        record = {
            'type': drink_type,
            'amount': amount_mg,
            'time': time
        }
        self records append(record)
        print(f"已记录: {drink_type} - {amount_mg}mg 咖啡因")
    
    def get_daily_total(self, date=None):
        """计算指定日期的总摄入量"""
        if date is None:
            date = datetime date today()
