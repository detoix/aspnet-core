# deploy to heroku
dotnet publish -c Release -o publish

sudo docker build -t registry.heroku.com/aspnet-core-detoix/web .

sudo heroku container:push web -a aspnet-core-detoix

heroku container:release web -a aspnet-core-detoix

heroku open -a aspnet-core-detoix
