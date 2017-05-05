## An Http hello world python program

### How to run

- Install Apache benchmark (Mac)  
`brew install homebrew/apache/ab`  

- Build the docker image  
`docker build . -t helloworld`

- Run it, expose a port  
`docker run --rm -itp 8080:8888 helloworld`

- (In a new terminal tab) Benchmark to your heart's desire
`ab -c 1 -n 1000 http://localhost:8888/`


Inspired by [Stella Cotton's](https://twitter.com/practice_cactus) [talk](https://speakerdeck.com/stellacotton/site-availability-is-for-everybody)
