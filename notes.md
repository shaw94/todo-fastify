I learned how to setup a server, i find mysel unfamiliar with a lot of the syntax, but that will change for sure.

I implemented my DB in docker as I usually do.

I know from my work with laravel, and the fastify docs, that they rely on mygrations too.

So I will setup a todo migration I want to have the following columns:

- title
- content (optional)
- created_at
- updated_at

hmmm from my research. It seems migrations are usually done by an ORM of your choosing. The docs show something different though. It shows something called postgrator. which is basically the way to make migrations work from sql files.

Right, from a video I just learned that you can get your docker variable point to a .env file which will basically make it easy for me to control everything in one place.

Let's take the migrator route, we will learn about doing this with ORMs later.

But before that let's make a .env file and have the postgres variables I need there. .ENV is a package, must get it via npm.

Right so this is spiraling a bit. My node version is outdated, and me install dotenv package, I noticed my node version is 18, while they are at 20. Naturally I wanted to install this version, and it seems the best way to have multiple version is to use nvm.

Right, I just got NVM and downloading the latest node version, then updating the dependencies within my project

Next, .env, then migrator. As we did in laravel, lets do a .env.example. We did .env.testing also, but i am not so sure I want to dable with testing just yet. it has been a while since I used Javascript. So let's give this time.

Right, made the .env, i remember from a video who recommended to never use the latest tag on dependencies within docker. Also, the port is for me to see the database on my host machine via my client.

Anyways just got the latest postgres docker image, and next is postgrator (hopefully before something else does not grab my attention)