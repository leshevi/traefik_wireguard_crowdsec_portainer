Основные команды проверки работы crowdsec:
docker exec crowdsec cscli decisions list, 
docker exec crowdsec cscli metrics
Перезапускать crontab -e после настройки crowdsec добавить в конец файла 0 */3 * * * docker exec crowdsec cscli hub update && docker exec crowdsec cscli hub upgrade.
