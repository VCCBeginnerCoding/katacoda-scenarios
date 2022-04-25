Below will show an example solution to the previous exercise.
<br>
Note that we have included extra code in the methods - don't worry if you only have print statements!

<pre class="file" data-filename="solution.py" data-target="replace">

import re

class Human():
  def __init__(self, email, address):
    self.email = email
    self.address = address
    

  def verify(self):
    regex = '^[a-z0-9]+[\._]?[a-z0-9]+[@]\w+[.]\w{2,3}$'
    
    if not re.search(regex, self.email) or not re.search(regex, self.address):   
      print("You have entered at least one invalid email")
      return False
      
    print("You have entered valid information")
    return True

  def sendMail(self):
    if verify(self):
      print("Sending your email to " + self.address + " from " + self.email)
    else:
      print("Could not send mail!")

name1 = Human("sender@vodafone.com", "recipient@vodafone.com")
name2 = Human("sender-vodafone", "recipient@vodafone.com")
name3 = Human("sender@vodafone.com", "recipient@vodafone")

name1.sendMail()
name2.sendMail()
name3.sendMail()
</pre>

`python solution.py`{{execute}}
