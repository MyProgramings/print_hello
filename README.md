# Print Hello World

Simple PHP page that prints "Hello World".

How to run locally (using PHP built-in server):

```bash
# open a bash shell and run from this directory
cd /c/Users/aaart/Desktop/Print_hello
php -S localhost:8000
```

Then open http://localhost:8000 in your browser.

## Docker

Build the Docker image and run it (this serves the same `index.php` through Apache on port 80):

```bash
# from this project directory
cd /c/Users/aaart/Desktop/Print_hello
docker build -t print_hello:latest .
docker run --rm -p 8080:80 print_hello:latest
```

Then open http://localhost:8080 in your browser.
