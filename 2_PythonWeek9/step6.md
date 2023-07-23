## Create Slide 2 - Textboxes & Notes

**Create Slide & Title**
```python
# Create Slide
slide_layout = ppt.slide_layouts[1]  # Slide Layout: Title Only
slide2 = ppt.slides.add_slide(slide_layout)  # Add layout to PowerPoint

# Slide Title
title1 = slide2.shapes.title

# Positioning
title1.left = Inches(0.5)
title1.top = Inches(0.4)
title1.width = Inches(10)
title1.height = Inches(1)

# Title Text
text3 = title1.text_frame.paragraphs[0]
text3.text = "All About Me"
text3.alignment = PP_PARAGRAPH_ALIGNMENT.LEFT
text3.font.name = "Vodafone Rg"  # font to be Vodafone Rg
text3.font.size = Pt(72)  # font size
text3.font.bold = True
text3.font.color.rgb = RGBColor(230, 0, 0)  # red text
```
**Summary Sentence**
```python
# Summary title
textBox1 = slide2.shapes.add_textbox(Inches(0.55), Inches(1.3), Inches(15), Inches(1))  # left, top, width, height
tf3 = textBox1.text_frame  # creating text frame for editable text
text4 = tf3.add_paragraph()
text4.text = str("Summary:")  # setting text to be current "month year"
text4.font.name = "Vodafone Rg"  # font to be Vodafone Rg
text4.font.size = Pt(36)  # font size
text4.font.bold = True
text4.font.underline = True
```
**Bullet Points**
```python
# Slide Bullet Points | 1
bullet_point_box = slide2.shapes.placeholders[1]  # Creating shape
bullet_point_box.width = Inches(15)
bullet_point_box.height = Inches(4)
bullet_point_box.top = Inches(2.4)
bullet_point_box.left = Inches(0.55)

# Bullet Point Text | 1
bullet_point_lvl1 = bullet_point_box.text_frame.paragraphs[0]  # Create placeholder for bullet points
bullet_point_lvl1.font.name = "Vodafone Rg"
bullet_point_lvl1.font.size = Pt(34)
bullet_point_lvl1.text = name

# Bullet Point Text | 2
bullet_point_lvl2 = bullet_point_box.text_frame.add_paragraph()  # Create placeholder for bullet points
bullet_point_lvl2.font.name = "Vodafone Rg"
bullet_point_lvl2.font.size = Pt(34)
bullet_point_lvl2.text = hobby

# Bullet Point Text | 3
bullet_point_lvl3 = bullet_point_box.text_frame.add_paragraph()  # Create placeholder for bullet points
bullet_point_lvl3.font.name = "Vodafone Rg"
bullet_point_lvl3.font.size = Pt(34)
bullet_point_lvl3.text = jobSchool
```
**Hobby Sentence**
```python
# Hobby line
textBox2 = slide2.shapes.add_textbox(Inches(0.55), Inches(5), Inches(15), Inches(1))  # left, top, width, height
tf4 = textBox2.text_frame  # creating text frame for editable text
text5 = tf4.add_paragraph()
text5.text = "I love " + hobby + "!"
text5.font.name = "Vodafone Rg"  # font to be Vodafone Rg
text5.font.size = Pt(34)  # font size
text5.font.italic = True
```
**Notes Text**
```python
# Notes Paragraph
notes_slide = slide2.notes_slide
text_frame = notes_slide.notes_text_frame
p = text_frame.add_paragraph()
p.text = "These are my notes."
```
