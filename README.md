# hello_http
Hello world with a webserver in C


# hello_http Development Environment Setup

## Requirements
- Vagrant
- VirtualBox

## Setup Instructions

 **Clone the Repository:**
   ```sh
   git clone https://github.com/jt1975SC/hello_http.git
   cd hello_http


## Setting Up the Development Environment

- verify `Vagrantfile` is in the repository directory with the following content:

   ```ruby
   Vagrant.configure("2") do |config|
     config.vm.box = "ubuntu/bionic64"
     config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
     config.vm.network "forwarded_port", guest: 12344, host: 12344
   end




## How to build
```gcc -o dummyserv dummy_serv.c```

Or to build a static binary

```gcc -o dummyserv dummy_serv.c```

## How to run

```dummyserv 12344```


## Access Application from Host
from web browser on local host machine navigate to http://localhost:12344 to access the app