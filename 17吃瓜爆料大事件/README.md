### [👉👉点此进入♥观看入口👈👈](http://a.d44k.cc/hl.html)
<br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br><br></br>
if today_total >= self daily_limit * 1 5:
            return "建议: 今天不要再摄入咖啡因了，多喝水帮助代谢。"
        elif today_total >= self daily_limit:
            return "建议: 避免再摄入咖啡因，可以选择无咖啡因饮品。"
        elif today_total >= self daily_limit * 0 8:
            return "建议: 谨慎考虑是否继续摄入咖啡因，接近每日上限。"
        else:
            return "建议: 可以适量摄入咖啡因，但注意不要超过每日建议量。"
 
# 示例使用
if __name__ == "__main__":
    tracker = CaffeineTracker()
    
    # 添加一些示例记录
    tracker add_consumption("浓缩咖啡", 63)  # 一杯约63mg
    tracker add_consumption("美式咖啡", 150)  # 大杯约150mg
    tracker add_consumption("红茶", 47)      # 一杯约47mg
    tracker add_consumption("可乐", 34)      # 350ml约34mg
    
    # 检查状态
    tracker check_status()
    
    # 获取建议
    print("\n" + tracker get_advice())
