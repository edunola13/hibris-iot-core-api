# GSM Api

# Dependencies
Only run in Linuxs
`sudo apt-get install libi2c-dev python-dev python3-dev`

`redis`

# MQTT
Por un lado tiene que estar levantado el servicio de Mosquitto y por otro tenemos que lanzar el script:
`(env) python -m mqtt.live_server`
El cual corre en loop_forever y esta escuchando los topics.

# Redis
https://redis.io/download
Conviene usar un docker

# Celery
https://medium.com/@yedjoe/celery-4-periodic-task-in-django-9f6b5a8c21c7
"""
For dev: celery -A server worker -l info -B
"""

"""
For prod: 
celery -A server worker -l info
celery -A server beat -l info
"""