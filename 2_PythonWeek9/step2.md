
## Task Description
We will be developing an app that will edit an uploaded PowerPoint, using content from an uploaded Excel File. This section will be setting up the intial files we'll be uploading and introducing you to Streamlit. 

**PowerPoint File**
<br>
All you need is to save a blank PowerPoint on you local machine.
Alternatively, you can see one of the mentors who can share a predone file. 

**Excel File**
<br>
Copy the below headings. You can use the example data included or fill it with your own information.
Alternatively, you can see one of the mentors who can share a preprepared file. 

<img width="412" alt="image" src="https://github.com/VCCBeginnerCoding/katacoda-scenarios/assets/110603725/b73d3bfe-08a7-461e-821d-c4e429ffb4fb">

## Introductions to Streamlit

**Installation Packages**
<br>
You'll need to install the streamlit and python-pptx package available on PyCharm. 
The below packages are also used:

```python
import streamlit as st                      
from datetime import datetime
import csv
import pandas as pd
from pptx import Presentation              
from io import BytesIO                
from pptx.enum.text import PP_PARAGRAPH_ALIGNMENT
from pptx.util import Inches, Pt
from pptx.dml.color import RGBColor
```
