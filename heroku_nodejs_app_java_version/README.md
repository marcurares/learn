# How to setup a custom version of Java on a NodeJS Heroku app

I ran into this problem the other day, trying to run a Java binary on a Heroku instance, the binary required 1.8 and on the instance Java 1.7 was installed.

Lurking around the internet, you can find a solution, but hardly, bouncing from questions on stackoverflow.

In order to setup a custom version of Java on a NodeJS Heroku instance:

```
heroku buildpacks:clear
heroku buildpacks:add https://github.com/heroku/heroku-buildpack-jvm-common
heroku buildpacks:add heroku/nodejs
```

Then redeploy your app (`make a change & git commit & git push`).

You can test it by running:

```
heroku run java -version
```

I found the answer [here](http://stackoverflow.com/questions/34834990/java-unsupported-class-version-on-heroku-for-nodejs-app).
