Functionality of a quoter app
- reads a config .yaml (or .json (to be specified)) file
- parses the config and based on the information creates the connection to exchange and kafka
- uses implementations of quoters from py-exchange to acquire market-data from exchange
- pushes data into kafka
