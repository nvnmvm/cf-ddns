一键脚本

curl https://raw.githubusercontent.com/nvnmvm/cf-ddns/refs/heads/main/cf-ddns.sh > /root/cf-ddns.sh && chmod +x /root/cf-ddns.sh

定时任务

crontab -e
*/2 * * * * /root/cf-v4-ddns.sh >/dev/null 2>&1
