# How to build a Realtime chat app in the terminal using Python and Pusher Channels

Realtime chat is virtually any online communication that provides a realtime or live transmission of text messages from sender to receiver. This tutorial will show you how to build a realtime terminal chat using Python and Pusher channels. The full tutorial can be found here : [here](https://pusher.com/tutorials/chat-terminal-python) 

## Getting Started
First, we need to install a package called `virtualenv`. Virtualenv helps to manage environments in python. This is so we do not end up with conflicting libraries due to install operations from project to project. To install Virtualenv, we run:


    sudo pip install virtualenv

Once the install is completed, we can verify by running:


    virtualenv --version

Next, let us create a new environment with Virtualenv:


    virtualenv terminal-chat

Once the environment is done creating, we move into the new directory created and we activate the environment:


    # change directory
    cd terminal-chat
    # activate environment
    source bin/activate

Clone the project repository by running the command below if you use SSH

```
git clone git@github.com:samuelayo/terminal-chat.git
```

If you use https, use this instead

```
git clone https://github.com/samuelayo/terminal-chat.git
```

Move into the new directory

```
cd terminal-chat
```

install Pysher from the github link, as the one delivered to pypy is outdated.

```
pip install git+https://github.com/nlsdfnbch/Pysher.git
```

install the required libraries

```
pip install -r requirements.txt
```

### Prerequisites

#### Setup Pusher

If you don't have one already, create a free Pusher account at https://pusher.com/signup then login to your dashboard and create an app. 


Then fill in your Pusher app credentials in your `.env` file by replacing this line with your appid, appkey and app secret respectively:

```
PUSHER_APP_ID=XXX_APP_ID
PUSHER_APP_KEY=XXX_APP_KEY
PUSHER_APP_SECRET=XXX_APP_SECRET
PUSHER_APP_CLUSTER=XXX_APP_CLUSTER
```



### Run the app

```
python terminalChat.py
```


## Built With

* [Pusher Channels](https://pusher.com/channels) - APIs to enable devs building realtime features.
* [Python](https://www.python.org/) - Python is a programming language that lets you work more quickly and integrate your systems more effectively.

