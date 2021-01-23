FROM node:14.15.4-buster

# Install dependencies
RUN apt-get update && apt-get install -y \
    python3.4 \
    python3-pip

RUN pip3 install pyatv
RUN npm install -g @sebbo2002/pyatv-mqtt-bridge

CMD pyatv-mqtt-bridge /var/lib/atv/config.json
