# FeedbackApp

A simple Java Servlet web application. Users submit their name, email, feedback type, and comments through an HTML form. The servlet displays the submitted feedback along with the current date and time.

## Requirements

1. HTML Page (feedback.html)
o Fields:
§ Name
§ Email
§ Feedback Type (dropdown: Complaint / Suggestion / Compliment)
§ Comments (textarea)
o Submit button that sends data to the servlet using POST method.

2. Servlet Class (FeedbackServlet.java)
o Read input parameters using request.getParameter()
o Display output as HTML with:
§ “Thank you, [Name] for your feedback!”
§ Feedback type and comments
§ Current date and time

3. Deployment Descriptor (web.xml)
o Map the servlet name FeedbackServlet to the URL pattern
/submitFeedback.

## Project structure

```text
FeedbackApp/
├── src/
│   └── com/
│       └── example/
│           └── FeedbackServlet.java
└── web/
    ├── feedback.html
    └── WEB-INF/
        └── web.xml
