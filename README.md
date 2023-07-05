from pptx import Presentation
from pptx.util import Inches

# Create a new PowerPoint presentation
presentation = Presentation()

# Slide 1: Title slide
slide_1 = presentation.slides.add_slide(presentation.slide_layouts[0])
title = slide_1.shapes.title
subtitle = slide_1.placeholders[1]

title.text = "AI Domains, Data Privacy, and AI Bias"
subtitle.text = "An Overview"

# Slide 2: AI Domains
slide_2 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_2.shapes.title
content = slide_2.placeholders[1]

title.text = "AI Domains"
content.text = "AI is applied in various domains:\n\n- Healthcare\n- Finance\n- Education\n- Manufacturing\n- Transportation\n- Entertainment"

# Slide 3: Data Privacy
slide_3 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_3.shapes.title
content = slide_3.placeholders[1]

title.text = "Data Privacy"
content.text = "Data privacy is crucial in AI:\n\n- Personal data protection\n- Consent and control\n- Secure data storage\n- Anonymization and de-identification"

# Slide 4: AI Bias
slide_4 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_4.shapes.title
content = slide_4.placeholders[1]

title.text = "AI Bias"
content.text = "AI bias refers to:\n\n- Unfair treatment\n- Discrimination\n- Skewed outcomes\n- Lack of diversity\n\nMitigating bias is essential for ethical AI."

# Slide 5: Examples of AI Bias
slide_5 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_5.shapes.title
content = slide_5.placeholders[1]

title.text = "Examples of AI Bias"
content.text = "Examples of AI bias:\n\n- Biased facial recognition\n- Gender bias in hiring algorithms\n- Racial bias in criminal justice\n- Socioeconomic bias in loan approvals"

# Slide 6: Conclusion
slide_6 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_6.shapes.title
content = slide_6.placeholders[1]

title.text = "Conclusion"
content.text = "AI has vast domains of application, but data privacy and AI bias are important considerations. Addressing these challenges is crucial for responsible and ethical AI development."

# Save the PowerPoint presentation
presentation.save("AI_Domains_Data_Privacy_AI_Bias.pptx")
