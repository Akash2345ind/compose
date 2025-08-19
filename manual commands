docker build -t todo-app-image ./app
docker run -d --name todo-database -p 27017:27017 mongo:6
docker run -d --name todo-app --link todo-database -p 3000:3000 -p 35729:35729 todo-app-image
