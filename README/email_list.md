# EMAIL_List

### Dependencies (Also refer to requirements.txt) ### 
<!-- Buttons for libraries -->
[![Streamlit](https://img.shields.io/badge/Streamlit-%230f4c75.svg?&style=flat-square&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Streamlit AgGrid](https://img.shields.io/badge/Streamlit--aggrid-%230f4c75.svg?&style=flat-square)](https://github.com/ranjeetraj/Streamlit-AGGrid)
[![Plotly](https://img.shields.io/badge/Plotly-%233399FF.svg?&style=flat-square&logo=plotly&logoColor=white)](https://plotly.com/)
[![Pandas](https://img.shields.io/badge/Pandas-%23150458.svg?&style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Selenium](https://img.shields.io/badge/Selenium-%2343B02A.svg?&style=flat-square&logo=selenium&logoColor=white)](https://www.selenium.dev/)
[![NumPy](https://img.shields.io/badge/NumPy-%23013243.svg?&style=flat-square&logo=numpy&logoColor=white)](https://numpy.org/)
[![Pyzotero](https://img.shields.io/badge/Pyzotero-%23FF6600.svg?&style=flat-square)](https://github.com/urschrei/pyzotero)
[![Beautiful Soup](https://img.shields.io/badge/Beautiful%20Soup-%23000000.svg?&style=flat-square&logo=beautifulsoup&logoColor=white)](https://www.crummy.com/software/BeautifulSoup/)
[![subprocess](https://img.shields.io/badge/subprocess-%230f4c75.svg?&style=flat-square)](https://docs.python.org/3/library/subprocess.html)
[![datetime](https://img.shields.io/badge/datetime-%230f4c75.svg?&style=flat-square)](https://docs.python.org/3/library/datetime.html)
[![dateutil](https://img.shields.io/badge/dateutil--parser-%230f4c75.svg?&style=flat-square)](https://dateutil.readthedocs.io/)
[![os](https://img.shields.io/badge/os-%230f4c75.svg?&style=flat-square)](https://docs.python.org/3/library/os.html)
[![sys](https://img.shields.io/badge/sys-%230f4c75.svg?&style=flat-square)](https://docs.python.org/3/library/sys.html)


## CMSE Scrapper ##
- #### This is an automated data scraping and reorganization tool. ####

- ### Zotero Scrapper ###
  CMSE facutly's publication are managed in Zotero (https://www.zotero.org/groups/2465063/cmseatmsu). The zotero scrapper function scrapes it using PyZotero library and the acquired data is stored in publication csv files.

- ### Directory scrapper ###
    The directory scrapper function scrapes the CMSE directory web page (https://cmse.msu.edu/Directory/index.aspx) using selenium and BeautifulSoup libraries. The acquired is stored in new Email list spreadsheet which is then merged with old Email list (as the directory on web page does not list all members of CMSE department)

These scrappers improves data accessibility and organization within the department. The Zotero Scrapper automates the collection and structuring of faculty publication data, reducing manual entry errors. Meanwhile, the Directory Scrapper simplifies contact list maintenance by merging fresh data with existing spreadsheets, 
ensuring accurate and up-to-date information. These tools collectively enhance efficiency and streamline administrative tasks.

### Streamlit GUI ###
- This program can be visualized on streamlit's app interface.
- Run the following command . This opens the webapp on your default web browser.
  - **streamlit run app.py**
  - or call "run_streamlit_app" method on CMSE class instance as shown in example file
- Email list file is displayed using streamlit's Ag-Grid, a powerful and highly customizable data grid component.
- You can see two menus on the left, Database and Stats. These two menu are handled by the respective files in app_menu_handlers folder.

#### How to install dependency libraries ####
- pip install streamlit
- pip install streamlit-aggrid
- pip install plotly
- pip install pandas
- pip install selenium
- pip install numpy
- pip install pyzotero
- pip install beautifulsoup4
- pip install python-dateutil
