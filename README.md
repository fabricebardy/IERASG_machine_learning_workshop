# IERASG_machine_learning_workshop
Code and Data for the IERASG machine learning workshop happening in Sydney 2019

The machine learning workshop will provide an introduction to some of basic principle behind machine learning.
We are going to use Google Colab for the tutorial session

### How to create a New Colab Notebook
- Open your google Drive
- Create a new notebook via Right Click > More > Colaboraty

### Mount your Google Drive

```
from google.colab import drive
drive.mount('/content/drive/')
```
It would need a authentication process. Do whatever it needs.

### Set current directory the path you want to clone the GIt projet 

```
path_clone = "drive/My Drive/"
!cd path_clone
```

### Cloning Github Repo to Google Colab

```
!git clone https://github.com/fabricebardy/IERASG_machine_learning_workshop.git
```

### Check your Folder Data

```
!ls Drive/test
```
### Upload code from your system

```
from google.colab import files
uploaded = files.upload()
```
### Make zip file of your Data

```
from google.colab import files
import zipfile
import sys
foldername = 'your folder or filename'
zipfile.ZipFile('Drive/'+foldername + '.zip', 'w', zipfile.ZIP_DEFLATED)
```

### Downloading the data from the colab

```
from google.colab import files
files.download('Drive/test.zip')
```
