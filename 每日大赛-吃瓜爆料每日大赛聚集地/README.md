print(f"\n=== {date} 咖啡因摄入报告 ===")
        print(f"今日已摄入: {total}mg / {self daily_limit}mg")
        
        if total > self daily_limit * 1 2:
            print("⚠️ 警告: 咖啡因摄入过量! 可能引起不适")
        elif total > self daily_limit:
            print("⚠️ 注意: 咖啡因摄入接近上限")
        elif total > self daily_limit * 0 8:
            print("⚠️ 注意: 咖啡因摄入较高")
        else:
            print("✅ 咖啡因摄入在安全范围内")
        
        print("\n详细记录:")
        for record in records:
            print(f"- {record['time'] strftime('%H:%M')}: {record['type']} - {record['amount']}mg")
    
    def get_advice(self):
        """提供健康建议"""
        today_total = self get_daily_total()
