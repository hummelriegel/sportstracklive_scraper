# sportstracklive_scraper
Download your data from https://www.sportstracklive.com

Quick and dirty notebook that downloads all your tracks (html and gpx) from sportstracklive.com in case you want to have a backup or upload your tracks to another service.

Basic idea:
1) Get an overview of the tracks on the search page: http://old.sportstracklive.com/search?what=user:USERNAME
2) Download a specific number of those overview pages
3) Download all linked "Info" pages with track details
4) Download the corresponding gpx-files
5) Clean up "empty" files, since we download "empty" gpx-tracks as well.

Setup:
1) Use the conda environment.yml to set up your python environment
2) Run the notebook in Jupyter (Lab)
3) Enter e-mail, password, username and number of search pages to scrape