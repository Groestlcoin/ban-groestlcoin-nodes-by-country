# ban-groestlcoin-nodes-by-country
Ban all connected groestlcoin nodes by filtering that country.

## Requirements for the bash script (ban.sh)

### Command-line JSON processor jq.

Install on Debian-based Linux
````
sudo apt-get install jq
````
### geoiplookup database and tool

Install on Debian-based Linux
````
sudo apt-get install geoip-bin
````
## Download and use the script

`git clone https://github.com/Groestlcoin/ban-groestlcoin-nodes-by-country.git`

Run:

````
cd ban-groestlcoin-nodes-by-country   
chmod u+x ban.sh   
./ban.sh
````
Adjust ISO 3166 Country Codes in ban.sh to your needs:
````
Shortcode=CN
````

### To view banned IP addresses:

````
groestlcoin-cli listbanned
````

### To clear banned IP addresses:

````
groestlcoin-cli clearbanned
````
