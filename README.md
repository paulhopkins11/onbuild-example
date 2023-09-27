
First build the parent

```
cd parent
docker build -t parent .
```

Then build the child

```
cd ../child
docker build -t child .
```
Now we can test the child
```
docker run -p 80:80 child
```
The page should now load in a browser