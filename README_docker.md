# hello_http
Hello world with a webserver in C


# Install Docker (https://docs.docker.com/desktop/)

## Setup Instructions

 **Clone the Repository:**
   ```sh
   git clone https://github.com/jt1975SC/hello_http.git
   cd hello_http


  ```bash
    cd hello_http
    ```

## How to build
  ```bash
    docker build -t hello_http .
    ```


## How to run


    ```bash
    docker run -p 12344:12344 hello_http
    ```


## Access Application from Host
from web browser on local host machine navigate to http://localhost:12344 to access the app
