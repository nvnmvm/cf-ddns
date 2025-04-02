一键脚本

curl https://raw.githubusercontent.com/nvnmvm/cf-ddns/refs/heads/main/cf-ddns.sh > /root/cf-ddns.sh && chmod +x /root/cf-ddns.sh

定时任务

crontab -e
*/2 * * * * /root/cf-ddns.sh >/dev/null 2>&1

# 如果需要日志，替换上一行代码
*/2 * * * * /root/cf-ddns.sh >> /var/log/cf-ddns.log 2>&1
