easy_cd_tute

https://medium.freecodecamp.org/how-to-set-up-continuous-deployment-in-your-home-project-the-easy-way-41b84a467eed

https://medium.com/@fidelvti/first-steps-with-docker-54cff8fe78f3

instead of running 
docker run -d --name <my-project> <username>/<my-project>
run the following
docker run -p 4000:80 -d --name <my-project> <username>/<my-project>
	to rerun
docker run -p 4000:80 -d <username>/<my-project>

once this is done, either goto 
http://0.0.0.0:4000
or
curl 0.0.0.0:4000
which you'll see something like the following 

```
<h3>Hello World!</h3><b>Hostname:</b> c0784df2064d<br/><b>Visits:</b> <i>cannot connect to Redis, counter disabled</i>
```