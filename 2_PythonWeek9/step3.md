## Initial Code - Streamlit

**Create Title**
<br>
```python
st.title('Edit/Update PowerPoint(s)')
```{{copy}}

**Setup Upload Areas**
<br>
```python
# Section to upload blank PowerPoint
PowerPoint = st.file_uploader('Blank PowerPoint', type=['pptx'], key='PP')

# Section to upload Excel File
Excel = st.file_uploader('Character Details', type=['xlsx'], key='ExcelFile')
```{{copy}}

**IF Statement**
<br>
This section of code will only run when a powerpoint AND excel file have been uploaded.
```python
if (PowerPoint is not None) and (Excel is not None):
    st.header("Updated PowerPoint:")

    binary_output = BytesIO()
    ppt.save(binary_output)
    st.download_button(label='Download PowerPoint', data=binary_output.getvalue(), file_name='New PowerPoint.pptx')
```{{copy}}
