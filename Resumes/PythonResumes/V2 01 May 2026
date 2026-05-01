from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, ListFlowable
from reportlab.lib.styles import getSampleStyleSheet
from reportlab.lib.pagesizes import A4

doc_path = "/mnt/data/Md_Atiquz_Zaman_Final_Resume_Final_Update_v3.pdf"

styles = getSampleStyleSheet()
story = []

# Header with proper clickable links (only values clickable)
story.append(Paragraph("<b>Md Atiquz Zaman</b>", styles['Title']))
story.append(Spacer(1, 4))
story.append(Paragraph(
    'Email: <link href="mailto:atiquzz42@gmail.com">atiquzz42@gmail.com</link> | '
    'Phone: <link href="tel:+916026557964">+916026557964</link> | '
    'Portfolio: <link href="https://atiquz.github.io/">atiquz.github.io</link>',
    styles['Normal']
))
story.append(Paragraph("Location: Goalpara, Assam, India | Open to Relocation Across India & Remote Work", styles['Normal']))
story.append(Spacer(1, 4))

# Professional Summary
story.append(Paragraph("<b>Professional Summary</b>", styles['Heading2']))
story.append(Paragraph(
    "I am Md Atiquz Zaman, currently pursuing a BS Degree in Data Science and Applications from IIT Madras which is ranked #1 in India in the NIRF rankings.",
    styles['Normal']
))
story.append(Spacer(1, 6))
story.append(Paragraph(
    "I specialize in customer support, HR recruitment, office administration, social media management, e-commerce operations, and digital marketing. "
    "I can manage CRM systems, handle customer queries, support hiring processes, manage social media engagement, handle e-commerce operations, and run marketing campaigns. "
    "I am detail-oriented, adaptable, and capable of working efficiently in both in-office and remote environments.",
    styles['Normal']
))
story.append(Spacer(1, 4))

# Education
story.append(Paragraph("<b>Education</b>", styles['Heading2']))
education = [
    "Indian Institute of Technology Madras – BS Data Science and Applications (Pursuing)",
    "PR Govt H.S. & M.P. School – Class 12 (2022)",
    "Oasis Academy, Goalpara – Class 10 (2020)"
]
story.append(ListFlowable([Paragraph(i, styles['Normal']) for i in education], bulletType='bullet'))
story.append(Spacer(1, 4))

# Core Skills
story.append(Paragraph("<b>Core Skills</b>", styles['Heading2']))
skills = [
    "Programming: HTML, CSS, Java, Python, PHP",
    "Web Development: Frontend & Basic Backend",
    "Databases: MySQL, SQL, Firebase",
    "Customer Support: Chat, Email, SMS, Live Chat",
    "HR & Recruitment: Sourcing, Screening, Job Posting, Hiring",
    "Office & Administration: Data Entry, Documentation, MS Office, Google Workspace",
    "Social Media Management: Content, Chats, Comments, Engagement",
    "E-commerce Management: Orders, Customer Support, Issue Handling",
    "Marketing & Campaigns: Setup, Ads Management, Performance Tracking",
    "Travel Management: Planning, coordination, booking and itinerary handling",
    "Communication: Professional Communication & Problem-Solving"
]
story.append(ListFlowable([Paragraph(i, styles['Normal']) for i in skills], bulletType='bullet'))
story.append(Spacer(1, 4))

# Platforms
story.append(Paragraph("<b>Platforms & Tools</b>", styles['Heading2']))
platforms = [
    "CRM: Salesforce, ActiveCampaign",
    "Helpdesk: Zoho Desk, Freshdesk, Zendesk, LiveAgent, Intercom",
    "HR Platforms: LinkedIn, Indeed, Apna, Monster, Naukri",
    "Productivity: Microsoft Office, Google Workspace",
    "Social Media: Facebook, Instagram, LinkedIn, Twitter (X), TikTok, WhatsApp",
    "E-commerce: Shopify, WooCommerce, Amazon, Flipkart, eBay, BigCommerce",
    "Marketing Tools: Meta Business Suite, Meta Ads, Google Ads, TikTok Ads, LinkedIn Ads"
]
story.append(ListFlowable([Paragraph(i, styles['Normal']) for i in platforms], bulletType='bullet'))
story.append(Spacer(1, 4))

# Key Responsibilities
story.append(Paragraph("<b>Key Responsibilities</b>", styles['Heading2']))
final_section = [
    "Resolve customer queries across multiple channels ensuring a positive experience",
    "Support recruitment activities including sourcing, screening, and coordination",
    "Manage social media interactions and maintain consistent audience engagement",
    "Handle e-commerce operations including order processing and issue resolution",
    "Assist in executing marketing campaigns and tracking performance",
    "Maintain accurate records, documentation, and administrative operations",
    "Support daily office tasks, coordination, and ensure timely completion of work"
]
story.append(ListFlowable([Paragraph(i, styles['Normal']) for i in final_section], bulletType='bullet'))
story.append(Spacer(1, 4))

# Languages
story.append(Paragraph("<b>Languages</b>", styles['Heading2']))
langs = ["English", "Hindi", "Urdu", "Bengali", "Assamese"]
story.append(ListFlowable([Paragraph(i, styles['Normal']) for i in langs], bulletType='bullet'))

# Margins
doc = SimpleDocTemplate(doc_path, pagesize=A4, topMargin=10, bottomMargin=15)
doc.build(story)

doc_path
