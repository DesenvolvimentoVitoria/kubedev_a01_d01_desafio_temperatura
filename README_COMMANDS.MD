docker image build -t desenvolvimentovitoria/conversao-temperatura:v1 .
docker container run -d -p 8080:8080 --name conversao-temperatura desenvolvimentovitoria/conversao-temperatura:v1
docker tag desenvolvimentovitoria/conversao-temperatura:v1 desenvolvimentovitoria/conversao-temperatura:latest
docker push desenvolvimentovitoria/conversao-temperatura:v1
docker push desenvolvimentovitoria/conversao-temperatura:latest