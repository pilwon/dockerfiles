FROM rabbitmq:3.5.0

# Management Plugin
RUN rabbitmq-plugins enable --offline rabbitmq_management
EXPOSE 15672

# Web-Storm Plugin
RUN rabbitmq-plugins enable --offline rabbitmq_web_stomp
EXPOSE 15674
