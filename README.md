# Robinhood for Google Finance

https://youtu.be/T17CHHhvsmc

Here is a pretty good tutorial I found on youtube! It should be sufficient to help most run this program without much experience.

### Usage instructions

#### Before

Robinhood has updated it's security scheme. You need following parameters in order to login.
`username` - your login username or email
`password` - your password
`device_token` - your frequently login device has a token tied to it. Often related to device you use browser to login.

To get device token, you need to use Chrome Dev tool to look for request Logs.
Open browser, go to robinhood.com.
Open Dev Tool, select prevserve log.
Start your regular login process.
Find url path */token*. Payload of this request should provide a `device_token`.


### Description

A Python script to export your [Robinhood](https://www.robinhood.com) trades to a .csv file (In a nice, Google Finance friendly format). Based on the [Robinhood library by Rohan Pai](https://github.com/Jamonek/Robinhood) and [Robinhood to CSV by Josh Fraser](https://github.com/joshfraser).
Works on Python 2.7+ and 3.5+

### Install:

    pip install -r requests

### Run:

    python gf-export.py
