FROM python:3.9

WORKDIR /src 
COPY requirements.txt ./
RUN pip install -r requirements.txt
COPY . .
 
EXPOSE 8000  

CMD python3 manage.py makemigrations && python3 manage.py migrate && python3 manage.py runserver 0.0.0.0:8000  
# CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]