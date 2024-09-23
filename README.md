# django_tutrial

# 仮想環境設定

```
$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
$ pip install -r requirements-dev.txt
```

## Useful commands

- `cdk ls` list all stacks in the app
- `cdk synth` emits the synthesized CloudFormation template
- `cdk deploy` deploy this stack to your default AWS account/region
- `cdk diff` compare deployed stack with current state
- `cdk docs` open CDK documentation

## deploy(manual)

```
$ cdk bootstrap --profile hht-takumi-dev
$ cdk diff --profile hht-takumi-dev
$ cdk deploy --all --require-approval never --profile hht-takumi-dev
```

## Django

```
$ django-admin startproject mysite
```

```
$ cd mysite
$ python3 manage.py runserver
```

```
$ python3 manage.py startapp polls
$ python3 manage.py makemigrations
$ python3 manage.py migrate
```

# mysql操作
```
$ mysql.server start
$ mysql.server stop
$ mysql -h localhost -u root
$ exit;
```

# user作成
```
CREATE USER 'django'@localhost identified by '0p-0p-0p-';
select User, host from mysql.user;
```

# databa操作
```
$ SHOW DATABASES;
$ CREATE DATABASE djangotr;
$ GRANT ALL PRIVILEGES ON djangotr.* TO 'django'@'localhost';
$ FLUSH PRIVILEGES;
```
