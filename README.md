# GNG-5300-Group-Backend
install requirements.txt


python3 -m venv venv

MACOS:
source venv/bin/activate

WIN:
.\venv\Scripts\activate


deactivate


test:
python -m unittest discover tests

tree -I "venv|*.pyc|__pycache__"

see error message

python -c "import app"

## run server
uvicorn main:app --host 0.0.0.0 --port 8000 --reload --log-level debug


## jenkins docker
docker build -t fitness-app .
docker run -d -p 80:8000 fitness-app




