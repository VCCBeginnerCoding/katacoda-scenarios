## Reading Excel File
_Note: all code used in this section should be included INSIDE the IF statement_

**See Code Below**
<br>
Read comments to underst line purpose.
```python
ExcelFile = Excel.name.replace(".xlsx", ".csv")           #  Convert file type from .xlsx to .csv (this is to use a simpler coding format)
data = []                                                 #  List to store the row of information wanted from the Excel File

try:
    for r in csv.reader(open(ExcelFile, 'r')):            #  FOR loop to read through each row in the Excel file
        if r[0] != "Group" and r[0] != "":                #  IF the first item in the list is not the title or empty then...
            data = r                                      #  Store the list in the variable named 'data'

except Exception:
    print()

# Store excel content in variable names
# Column Headers: Group, Presenter, Date, Name, Hobby, Job/School 
group = data[0]
presenter = data[1]
date = datetime.strptime(data[2], "%Y-%m-%d")
date = date.strftime("%d %B %Y")
name = data[3]
hobby = data[4]
jobSchool = data[5]
```{{copy}}
