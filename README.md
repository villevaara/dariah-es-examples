# dariah-es-examples

Example scripts for querying the Elasticsearch API vie the Python wrapper.

## Installation

The scrips have been written for Python 3. `requirements.txt` has the required libraries listed. Install those with e.g. `pip install -r requirements.txt`.

## Usage

See the video at [https://www.dariah.fi/subsetting-tool/](https://www.youtube.com/watch?v=EVe5ZUo8tOM) on how to integrate the scripts here with the Kibana GUI.

The basic workflow is:
1. Use Kibana's Discover-view to work out a subset of the data you want to query with the API. 
2. Save the query json (Discover -> Inspector -> Request -> Copy to clipboard) into a file (see examples in this repo).
3. Copy and adapt the example script in `download_query.py` in this repo, filling in the username, password and index names, and possibly using a paginated version of the script is necessary. See comments in the script for details.
4. Run the script to download your subset.
