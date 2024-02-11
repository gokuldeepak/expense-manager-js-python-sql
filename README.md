# expense-manager-js-python-sql

I'm trying to build a basic Expense Manager. 
Wanted to build in public as Opensource. Any contributions for Security and good practice is welcome. 


Installed Ubuntu 22.04

Not as a root user but with sudo privilege 
I'm not using venv as I'm using a Virtual VM only for this project

sudo apt update
python3 --version
 Python 3.10.12
sudo install pip
pip install flask

pip --version
pip 22.0.2 from /usr/lib/python3/dist-packages/pip (python 3.10)

python3 -m flask --version
 Python 3.10.12
 Flask 3.0.2
 Werkzeug 3.0.1

sudo apt install mysql-server
sudo systemctl start mysql.service
sudo mysql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';
exit
mysql -u root -p
ALTER USER 'root'@'localhost' IDENTIFIED WITH auth_socket;
CREATE USER 'gokul'@'localhost' IDENTIFIED BY 'gokul';
GRANT ALL PRIVILEGES ON *.* TO 'gokul'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;
exit


Install Dependencies:

pip3 install pymysql
python -m pip install mysql-connector-python
pip install Flask-Cors


Run flask:
export FLASK_APP=app.py
python3 -m flask run --host=0.0.0.0