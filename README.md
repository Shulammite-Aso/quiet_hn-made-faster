## Make Quiet Hacker News Faster

The goal was to take a clone of [Hacker News](https://news.ycombinator.com) callled Quiet Hacker News and make it faster using go routines and catching, while handling race conditions.

Note: this was completed as part of [gophercises](https://gophercises.com) exercise to practice effective use of concurrency in go.

### How to test

If your're familier with Go and already have it installed, then clone code and run main file with ``go run -race main.go``, otherwise, open in a cloud dev environment, e.g [Gitpod](https://www.gitpod.io), and run ``go run -race main.go`` on the terminal. View page on port 3000 of your server, then observe at the bottom of the page how much time it took to load. Reload page several times observing the load time still. Check your terminal output where you ran ``go run -race main.go`` to see if any race conditions where reported.