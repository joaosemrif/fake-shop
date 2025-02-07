# Fake Shop
Imagem: https://hub.docker.com/r/joaolopesneto/fake-shop

Criar imagem: docker build -t NOME_IMAGEM: versao -f Dockerfile .

Docker hub: docker push

Criar clauster: k3D cluster create
Criar objeto: kubectl apply -f K8s/deployment.yaml

## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.

kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
