# build from Dockerfile
docker build .
# or with tag name
docker build -t <image_name> .

# build from docker-compose.yml
docker-compose build
 
# Linting : install flake8 package
docker-compose run --rm app sh -c "flake8" 

# Django Testing
docker-compose run --rm app sh -c "python manage.py test" 

