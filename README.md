# 🐧 Linux Command Cheat Sheet for Developers & Production Servers

This repository contains **must-know Linux commands (prompts)** for:
- Daily development work
- Production server management
- Django backend development

You can bookmark this, fork it, or extend it for your own workflows.

---

## 📌 Table of Contents
1. [30 Must-Know Linux Commands for Developers](#-30-must-know-linux-commands-for-developers)
2. [30 Linux Commands for Production Servers](#-30-linux-commands-for-production-servers)
3. [Linux Commands for Django Developers](#-linux-commands-for-django-developers)

---

# 🔥 30 Must-Know Linux Commands for Developers

```bash
sudo apt update
```
### Use case: refresh package list

```bash
sudo apt upgrade -y
```
Use case: upgrade installed packages

```bash
sudo apt install git -y
```
Use case: install software

```bash
pwd
```
Use case: show current directory

```bash
ls -la
```
Use case: list files with permissions

```bash
cd /path/to/dir
```
Use case: navigate directories

```bash
mkdir -p app/src
```
Use case: create nested directories

```bash
touch file.txt
```
Use case: create file

```bash
rm -rf temp/
```
Use case: delete file/folder

```bash
cp -r src backup
```
Use case: copy files

```bash
mv old.txt new.txt
```
Use case: rename/move file

```bash
less logs.txt
```
Use case: read large file

```bash
tail -f logs.txt
```
Use case: live logs

```bash
grep -r "ERROR" .
```
Use case: search text in files

```bash
find . -name "*.py"
```
Use case: find files

```bash
chmod +x script.sh
```
Use case: make script executable

```bash
sudo chown user:user file.txt
```
Use case: change ownership

```bash
sudo command
```
Use case: run as admin

```bash
ps aux
```
Use case: list running processes

```bash
htop
```
Use case: system monitor

```bash
kill -9 PID
```
Use case: kill process

```bash
ss -tulpn
```
Use case: check open ports

```bash
df -h
```
Use case: disk usage

```bash
free -h
```
Use case: memory usage

```bash
ping google.com
```
Use case: network test

```bash
curl https://api.example.com
```
Use case: API testing

```bash
git status
```
Use case: git repo status

```bash
git add . && git commit -m "update"
```
Use case: commit changes

```bash
tar -xzvf app.tar.gz
```
Use case: extract archive

```bash
sudo systemctl restart nginx
```
Use case: restart service

---

# 🛡️ 30 Linux Commands for Production Servers

```bash
uptime
```
Use case: server load & uptime

```bash
who
```
Use case: logged-in users

```bash
df -h
```
Use case: disk monitoring

```bash
du -sh /var/log
```
Use case: directory size

```bash
free -h
```
Use case: RAM usage

```bash
htop
```
Use case: live monitoring

```bash
kill -9 PID
```
Use case: stop hung process

```bash
ss -tulpn
```
Use case: check services

```bash
sudo systemctl restart nginx
```
Use case: restart web server

```bash
sudo systemctl status nginx
```
Use case: service status

```bash
sudo systemctl enable nginx
```
Use case: auto-start service

```bash
journalctl -u nginx
```
Use case: service logs

```bash
journalctl -u nginx -f
```
Use case: live logs

```bash
sudo tail -f /var/log/auth.log
```
Use case: auth/security logs

```bash
sudo ufw status
```
Use case: firewall status

```bash
sudo ufw allow 80
```
Use case: open port

```bash
sudo ufw delete allow 80
```
Use case: close port

```bash
ip a
```
Use case: IP info

```bash
ping google.com
```
Use case: connectivity

```bash
curl localhost:8000
```
Use case: health check

```bash
tar -czvf backup.tar.gz /var/www
```
Use case: backup

```bash
tar -xzvf backup.tar.gz
```
Use case: restore

```bash
chmod -R 755 /var/www
```
Use case: permissions fix

```bash
sudo chown -R www-data:www-data /var/www
```
Use case: web ownership

```bash
env
```
Use case: env variables

```bash
crontab -l
```
Use case: list cron jobs

```bash
crontab -e
```
Use case: edit cron

```bash
sudo reboot
```
Use case: reboot server

```bash
sudo shutdown now
```
Use case: shutdown

```bash
history
```
Use case: command history

---

# 🐍 Linux Commands for Django Developers

```bash
python3 -m venv venv
```
Use case: create virtual environment

```bash
source venv/bin/activate
```
Use case: activate venv

```bash
pip install -r requirements.txt
```
Use case: install dependencies

```bash
pip freeze > requirements.txt
```
Use case: save dependencies

```bash
python manage.py runserver
```
Use case: run dev server

```bash
python manage.py migrate
```
Use case: apply migrations

```bash
python manage.py makemigrations
```
Use case: create migrations

```bash
python manage.py createsuperuser
```
Use case: admin user

```bash
python manage.py shell
```
Use case: Django shell

```bash
python manage.py collectstatic
```
Use case: production static files

```bash
python manage.py test
```
Use case: run tests

```bash
python manage.py check
```
Use case: config validation

```bash
gunicorn project.wsgi:application
```
Use case: production server

```bash
gunicorn --workers 3 project.wsgi
```
Use case: scale workers

```bash
sudo systemctl restart gunicorn
```
Use case: restart app

```bash
tail -f logs/django.log
```
Use case: debug errors

```bash
python manage.py dbshell
```
Use case: DB access

```bash
python manage.py dumpdata > data.json
```
Use case: backup data

```bash
python manage.py loaddata data.json
```
Use case: restore data

```bash
export DEBUG=False
```
Use case: production env

```bash
sudo systemctl start redis
```
Use case: caching / Celery

```bash
celery -A project worker -l info
```
Use case: background jobs

```bash
celery -A project beat -l info
```
Use case: scheduled tasks

```bash
sudo systemctl restart celery
```
Use case: restart workers

```bash
sudo systemctl status postgresql
```
Use case: DB status

```bash
export DJANGO_SETTINGS_MODULE=project.settings.prod
```
Use case: multi-env config

```bash
find . -name "__pycache__" -delete
```
Use case: cleanup cache

```bash
which python
```
Use case: verify venv

```bash
pip list
```
Use case: installed packages

```bash
git pull origin main
```
Use case: deploy update

---

## ✅ Tip
Keep this file as `LINUX_COMMANDS.md` in your GitHub repo and extend it as you learn more.

Happy hacking 🚀

