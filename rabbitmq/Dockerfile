FROM rabbitmq:3.5.0

RUN rabbitmq-plugins enable --offline rabbitmq_management
RUN rabbitmq-plugins enable --offline rabbitmq_web_stomp

EXPOSE 15672  # management
EXPOSE 15674  # web-storm
