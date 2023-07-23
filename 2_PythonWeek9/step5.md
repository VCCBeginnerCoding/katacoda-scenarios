## Create a PowerPoint Slide - Cover Page
_Note: all code used in this section should be included INSIDE the IF statement_

**Create PowerPoint Variables**
```python
# Creating PowerPoint
ppt = Presentation()

# Set Slide Size
ppt.slide_width = Inches(16)
ppt.slide_height = Inches(9)
```

**Decorate Slide**
```python
# Create Slide
title_slide_layout = ppt.slide_layouts[6]  # Slide Layout: Blank
slide1 = ppt.slides.add_slide(title_slide_layout)  # Add layout to PowerPoint

# Background Image
left = top = Inches(0)  # Image Position
background_img = "Cover Page.png"  # Background Image
pic = slide1.shapes.add_picture(background_img, left, top, width=ppt.slide_width, height=ppt.slide_height)

# This moves it to the background
slide1.shapes._spTree.remove(pic._element)
slide1.shapes._spTree.insert(2, pic._element)
```
**Add Textbox with Presenter & Date**
```python
# Text for Presented by and Date
textBox = slide1.shapes.add_textbox(Inches(0.5), Inches(7.2), Inches(4), Inches(1))  # left, top, width, height
tf1 = textBox.text_frame  # creating text frame for editable text
text1 = tf1.add_paragraph()
text1.text = str("Presented by " + presenter + '\n' + date)  # setting text to be current "month year"
text1.font.name = "Vodafone Rg"  # font to be Vodafone Rg
text1.font.size = Pt(28)  # font size
text1.font.color.rgb = RGBColor(255, 255, 255)  # white text
# Alternative option for date: datetime.date.today().strftime("%d %B %Y")
```

**Add Textbox for Title**
```python
# Text for Title
textBox = slide1.shapes.add_textbox(Inches(0.5), Inches(6), Inches(4), Inches(1))  # left, top, width, height
tf2 = textBox.text_frame  # creating text frame for editable text
text2 = tf2.add_paragraph()
text2.text = group
text2.font.name = "Vodafone Rg"  # font to be Vodafone Rg
text2.font.size = Pt(66)  # font size
text2.font.color.rgb = RGBColor(255, 255, 255)  # white text
text2.font.bold = True
```
