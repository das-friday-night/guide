# install and run mongoDB on Mac
1. Open the Terminal app and type `brew update`.
2. After updating Homebrew `brew install mongodb`.
3. After downloading Mongo, create the “db” directory. This is where the Mongo data files will live. You can create the directory in the default location by running `mkdir -p /data/db`.
4. Make sure that the /data/db directory has the right permissions by running
```sudo chown -R `id -un` /data/db```
5. Run the **Mongo daemon**, in one of your terminal windows run `mongod`. This should start the Mongo server.
6. Run the **Mongo shell**, with the Mongo daemon running in one terminal, type `mongo` in another terminal window. This will run the Mongo shell which is an application to access data in MongoDB.
7. To exit the Mongo shell run `quit()`.
8. To stop the Mongo daemon hit `ctrl-c`.