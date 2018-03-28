0. this assumes testing through our docker image and this is cloned under `Web/`
1. run `php bin/console cache:clear` and `php bin/console cache:warmup`
2. create `./var` and then an empty file `./var/bootstrap.php.cache`
3. add `example.apache.conf` to your apache -- change paths as needed
4. you should be able to go to `http://symfony34.readitlater.localhost/somepage` and see a symfony-served 404:
  > Oops! An Error Occurred
  > The server returned a "404 Not Found".
