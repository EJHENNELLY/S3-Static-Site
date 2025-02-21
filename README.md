# S3-Static-Site
Host a static website on AWS using S3 and use Cloudfront to serve it through HTTPS

To begin, Navigate to AWS console and search S3. <br/>
Create a bucket, give it a unique name, leave everything else default and proceed with creating your bucket. <br/>
![Screenshot (62)](https://github.com/user-attachments/assets/d87e3117-cc96-4551-971b-638746cd643c)

Click on your bucket -> Properties -> scroll all the way down to "static website hosting" and click enable. -> type in the html name (most likely index.hmtl) <br/>
Next navigate to the "permissions" tab -> edit block all public access and deselect all checkboxes <br/>
Click edit bucket policy and type in the following code: (Remember to add in your own bucket name)
![Screenshot (63)](https://github.com/user-attachments/assets/9f935479-8fde-48ff-ae4c-0cbe94d45eaa)

Click Save Changes. <br/>
Now the bucket is set up to host our website. <br/>

Navigate to the "objects" tab and upload your html and any other website files. <br/>
![image](https://github.com/user-attachments/assets/846a66af-4b72-41a3-8f0f-2d543300b077)

Once that is done navigate back to the url found at the bottom of the "properties" tab and you should have your website!
![Screenshot (66)](https://github.com/user-attachments/assets/99bfff9f-aefc-43f1-acd2-cc8fff466065)

That was Easy!

When you are done, make sure to delete the bucket if you do not want to leave the static site up!
