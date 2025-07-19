total = 0
        for record in self records:
            record_date = record['time'] date()
            if record_date == date:
                total += record['amount']
        
        return total
    
    def get_daily_records(self, date=None):
        """获取指定日期的所有记录"""
        if date is None:
            date = datetime date today()
        
        return [record for record in self records 
                if record['time'] date() == date]
    
    def check_status(self, date=None):
        """检查咖啡因摄入状态"""
        if date is None:
            date = datetime date today()
        
        total = self get_daily_total(date)
        records = self get_daily_records(date)
