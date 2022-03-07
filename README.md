# Deploy configuration
Some files and commands for deployment
<br>
If you in project directory


```
sudo ln -s ${PWD}/nginx/app.conf /etc/nginx/sites-enabled/
sudo ln -s ${PWD}/gunicorn/gunicorn.service /etc/systemd/system/
sudo ln -s ${PWD}/gunicorn/gunicorn.socket /etc/systemd/system/

sudo systemctl daemon-reload
sudo systemctl start gunicorn
sudo systemctl enable gunicorn
sudo service nginx restart
```
