# demeter
Python module for fetching historical market data

Demeter was the Greek god of harvest. These scripts 'harvest' historical
market data from the interwebs for your data pleasure.

### ingest_raw_data.py
Pull reads Stooq CSV data files and creates a HDF5 file where each
ticker is stored as a key. Data is stored in a data frame structure
with the following columns:
`open high low close volume`

### list_hdf_keys.py
Reads all keys from HDF5 file and outputs those keys to the console.

### read_ohlc.py
Return the first and last row of a ticker's data frame. This is the first
and last day in the HDF5 data set.
