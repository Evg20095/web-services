docker exec -it project_flask_flask_1 bash

docker exec -it project_flask_flask_1 python train_model.py

curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"flower":"1,2,3,4"}' \
  http://localhost:5000/iris_postZhemkov20095
  
  /submit
предиктивная модель скорит файл и возвращает обратно

/upload
предиктивная модель скорит файл и возвращает обратно, можно послать запрос машиной, например через postman

/iris/<param>
передайте четыре параметра, пример: ".../iris/1,2,3,4" Вернётся картинка с нужным цветком.
