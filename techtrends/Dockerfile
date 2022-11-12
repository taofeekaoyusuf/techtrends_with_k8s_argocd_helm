# Command to execute python
FROM python:3.8

# Command to add a Label
LABEL maintainer="Taofeek Yusuf"

# Command to organized the project
COPY . /app
WORKDIR /app

# Command to install the requirements
RUN pip install -r requirements.txt

# Command to initialized the database
RUN python init_db.py

# Command to expose a port
EXPOSE 3111

# Entry point for the application
ENTRYPOINT [ "python" ]

# Command to run on container start
CMD [ "app.py" ]
