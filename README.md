# AWSprojects
HOSTING A STATIC WEBSITE ON AMAZON S3
I created a frontend project a while ago which was a stop watch app by using HTML, CSS and javascript.
I then created an S3 bucket on AWS management console called staticwebbucket111.
I then uploaded the index.html, style.css and script.js files to the bucket.
I then enabled static web hosting in the bucket properties tab.
I then set the Index document to index.html and saved the changes.
I set the permissions for public access as follows:
  {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::staticwebbucket111/*"
        }
    ]
}

I finally copied the url created for the website by enabling the static web hosting from the properties tab.

I disabled my antivirus so that the webpage could load because it said it was not secure.
