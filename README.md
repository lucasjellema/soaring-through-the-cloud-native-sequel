# soaring-through-the-cloud-native-sequel
To support the Oracle Cloud demo "Soaring through the Clouds The Sequel" on microservices and container and cloud native computing. Our first performance: Oracle EMEA PaaS Partner Forum - March 2018, Budapest

I have used the Git Submodules feature to link the Logistics Microservice repo from the central GitHub repo. 
I used this command locally:
git submodule add -b master https://github.com/lucasjellema/logistics-microservice-soaring-clouds-sequel
then:
git submodule init

And then commit & push.

git commit -m "Adding submodule for product-ms"

git push


The same for other submodules:

https://github.com/gschmutz/product-soaring-clouds-sequel
https://github.com/svenbernhardt/financials-microservice-soaring-clouds-sequel
https://github.com/ldikmans/customer-microservice-soaring-clouds-sequel


to update the submodules in the main:

git submodule update --remote --merge
git add <each submodule that was updated>

git commit -m "updated submodules"

git push

https://stackoverflow.com/questions/1030169/easy-way-to-pull-latest-of-all-git-submodules

git submodule update --recursive --remote

https://chrisjean.com/git-submodules-adding-using-removing-and-updating/

