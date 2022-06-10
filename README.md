# PayMe-In-Crypto

## Summary 

Fintech Finder is a web app that allows fintech professionals to be hired by the hour and paid in crypto currency ( Ethereum ) for their time. All payments are made using the ethereum blockchain. The application has been pre loaded with a few mock users and their information in order to test the application.

This app requires the use of ganache from the truffle suite and streamlit for the front end. all these python requirements are listed in the requirements.txt file.

## Application Usage

- Pick a professional from the list and decide how much time you want you need from them.
- The application will then calculate the amount of ether you need to pay to the professional based on their hourly rate and the time you need.
- The Total wage in ether is then displayed to the user with a button to confirm and send the payment.

Since we are testing this on our own private blockchain via Ganache, we will display the transaction hash of the transaction on the web app page and verify it on the Ganache console as well.

below is a quick demo of the application with a test transaction hash and the same transaction hash on the Ganache console.

![App Demo](imgs/app_demo.gif)

## How to use it in your own development environment

in case you would like to test this out you would need the following packages:

- [Ganache App](https://trufflesuite.com/ganache/)
- pip install -r requirements.txt
- install and run a quick start blockchain with Ganache
- copy the 12 word key from ganache and paste it into a .env file in the root directory of the project with a variable name of `MENMONIC`
- run the application with ` streamlit run fintech_finder.py` using the terminal window on your computer
