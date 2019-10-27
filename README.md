# Kleis website

The website is based on Jekyll and Tale

## to test locally
 
1. install gems

```` sh
docker run --rm -ti --workdir '/code' -v "${PWD}:/code" -v "${PWD}/.gems:/usr/local/bundle" -p "4000:4000" mathieubrun/jekyll:latest 
````

2. local run : 
```` sh
docker run --rm -ti --workdir '/code' -v "${PWD}:/code" -v "${PWD}/.gems:/usr/local/bundle" -p "4000:4000" mathieubrun/jekyll:latest
````

## to deploy manually (for now) on infomaniak 

3. local build
```` sh
docker run --rm -ti --workdir '/code' -v "${PWD}:/code" -v "${PWD}/.gems:/usr/local/bundle" -p "4000:4000" mathieubrun/jekyll:latest exec jekyll build
````

4. copy the content of _site directory to in the destination server
 

## License
See [LICENSE](https://github.com/chesterhow/tale/blob/master/LICENSE)
