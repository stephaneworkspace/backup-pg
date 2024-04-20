# backup-pg

Script : BACKUP POSTGRESQL from VPS Infomaniak to SwissBackup Infomaniak Swift

needed:
sudo pacman -Sy cronie
sudo systemctl enable cronie
sudo systemctl start cronie
export EDITOR=vim

cron:
crontab -e
0 6 * * * /bin/bash /home/arch/backup-pg/backup_daily.sh
