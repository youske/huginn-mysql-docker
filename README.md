huginn mysql for docker
=======================

# about

# setup

    install docker for windows (Hyper-V)

    git clone https://github.com/youske/huginn-mysql-docker.git
    cd huginn-mysql-docker

# run

## docker run

    mysql server
    docker run --name huginn_mysql --env ./env/huginn_mysql.env mysql

    huginn server
    docker run --name huginn --link huginn_mysql:mysql -p 3000:3000 --env ./env/huginn.env cantino/huginn

## compose run

    docker-compose up -d


# etc
    huginn admin
    admin:password (default)
