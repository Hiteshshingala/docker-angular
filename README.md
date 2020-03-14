Steps:
1) docker build -t example:dev .
2) docker run -v ${PWD}:/app -v /app/node_modules -p 4201:4200 --rm example:dev
3)  docker run -it -v ${PWD}:/app -v /app/node_modules -p 4201:4200 --rm example:dev
4) docker run -d -v ${PWD}:/app -v /app/node_modules -p 4201:4200 --name foo --rm example:dev