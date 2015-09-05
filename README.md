# Clean SOCS
A docker compose file which gets a media server including
* Sabnzb
* Owncloud
* Couchpotato
* Sickbeard
* Plex (just for fun)

## Installation

### Prerequisites
* In this case, the underlying OS was based on openmediavault (http://www.openmediavault.org/)
* Ensure that you install docker on debian (wheezy) as that was openmediavault is based on (https://docs.docker.com/installation/debian/#debian-wheezy-stable-7-x-64-bit)
* Install docker-compose: https://docs.docker.com/compose/install/

### Install, Download, and Run
* Clone the respository: `git clone https://github.com/javexed/clean_socs`
* cd into the respository: `cd clean_socs`
* Link to the data directory. For example, assuming you are using openmediavault, and have
a directory called "Data", the default location is /export/Data, and the command to
create the link is: `ln -S /export/Data ./data
* Download and run: `docker-compose up -d`
* Monitor progress: `docker-compose logs`

### Configure (assuming based on openmediavault)
Refer to each for specifics on configuration
* Start with Sabnzb at: http://openmediavault:8080
* Sickbeard at: http://openmediavault:8081
* Couchpotato at: http://openmediavault:5050
* Owncloud at: http://openmediavault:8082
* Plex at: http://openmediavault:32400

## Usage
Refer to docker-compose for commands to control.

## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D
## History

## Credits
This just ties the docker images together, please refer to:
* Tim Haak for Sabnzb, Couchpotato, Sickbeard, and Plex: https://github.com/timhaak
* Official Owncloud: https://hub.docker.com/_/owncloud/
* Official Mariadb: https://hub.docker.com/_/mariadb/
## License
Do with it as you will.
