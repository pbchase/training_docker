FROM ubuntu

RUN apt-get update && apt-get install -y \
  curl \
  pv

ENV SPEED 9600

RUN echo "Wingardium Leviosa"
CMD curl -s http://kevinhanson.org/shuttle.vt | pv -L${SPEED} -q
