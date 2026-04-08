# 🌐 AWS S3 Static Website Hosting Project

## 🔗 Live Website

👉 https://aditya-miniproject2-s3.s3.ap-southeast-2.amazonaws.com/index.html

---

## 📌 Project Information

**Project Name:** `aditya-miniproject2-s3`

**Created By:** Aditya Kumar Singh

**AWS Service Used:** Amazon S3

**Region:** Asia Pacific (Sydney) 🌏

**Region Code:** `ap-southeast-2`

**Main Website File:** `index.html` 📄

---

## 🎯 Objective

The objective of this assignment is to create and host a simple static website using Amazon S3. The website must be uploaded to an S3 bucket, configured for public access, and opened through a public URL.

Amazon S3 is commonly used to store files such as HTML, CSS, JavaScript, images, and documents. It can also be used to host static websites because static websites do not require server-side processing.

---

## 📖 Project Description

In this project, a static webpage was created using HTML and CSS. The page contains information about the AWS assignment, the hosting task, the bucket name, the region, and the final website link.

The webpage was prepared as `index.html`, which is the default home page file name used by most static website hosting setups. This file was uploaded to an Amazon S3 bucket named `aditya-miniproject2-s3`.

After uploading the file, public access settings were configured so the webpage could be accessed from a browser using the S3 public URL.

---

## 📂 Files in This Project

```text
unit3/
|-- index.html
`-- README.md
```

### 📄 File Details

| File Name    | Description                                                                        |
| ------------ | ---------------------------------------------------------------------------------- |
| `index.html` | Main static website page created using HTML and CSS.                               |
| `README.md`  | Documentation file that explains the project, task, setup steps, and final output. |

---

## 🧱 Step 1: Create the Static Website

The first step was to create an HTML file named `index.html`.

The webpage includes:

* Project title
* Student name
* AWS S3 assignment information
* Project overview
* Task workflow
* Hosting details
* Final public website link

The website was designed as a single static page, which means it does not need a backend server, database, or dynamic framework.

### 🛠️ Technologies Used

* HTML for page structure
* CSS for layout, colors, spacing, and responsive design

---

## 🪣 Step 2: Create an S3 Bucket

An S3 bucket was created in the AWS Management Console.

### 📌 Bucket Details

```text
Bucket Name: aditya-miniproject2-s3
Region: Asia Pacific (Sydney)
Region Code: ap-southeast-2
```

### ✅ Steps Followed

1. Opened the AWS Management Console
2. Searched for and opened the S3 service
3. Clicked on **Create bucket**
4. Entered the bucket name as `aditya-miniproject2-s3`
5. Selected the region as **Asia Pacific (Sydney)**
6. Created the bucket

The bucket name must be unique because S3 bucket names are globally unique across AWS.

---

## ⬆️ Step 3: Upload the Website File

After creating the S3 bucket, the `index.html` file was uploaded.

### ✅ Steps Followed

1. Opened the S3 bucket named `aditya-miniproject2-s3`
2. Clicked on **Upload**
3. Added the `index.html` file
4. Clicked on **Upload** to store the file in the bucket

After upload, the file was available inside the bucket as:

```text
index.html
```

---

## 🔓 Step 4: Enable Public Access

To allow the website to open in a browser, the uploaded HTML file must be publicly readable.

### ⚠️ Important Public Access Steps

1. Open the S3 bucket
2. Go to the **Permissions** tab
3. Review **Block public access** settings
4. Allow public access only if the assignment requires a public website
5. Add a bucket policy that allows public read access

### 📜 Example Bucket Policy

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicRead",
      "Effect": "Allow",
      "Principal": "*",
      "Action": ["s3:GetObject"],
      "Resource": ["arn:aws:s3:::aditya-miniproject2-s3/*"]
    }
  ]
}
```

This policy allows public users to read objects inside the bucket.

---

## 🌍 Step 5: Static Website Hosting

For a standard S3 static website hosting setup, static website hosting can be enabled from the bucket properties.

### ✅ Steps

1. Open the bucket named `aditya-miniproject2-s3`
2. Go to the **Properties** tab
3. Scroll to **Static website hosting**
4. Click **Edit**
5. Select **Enable**
6. Choose **Host a static website**
7. Enter the index document as:

```text
index.html
```

8. Save the changes

### 🔗 Website Endpoint Format

```text
http://aditya-miniproject2-s3.s3-website.ap-southeast-2.amazonaws.com
```

---

## 🔗 Step 6: Public Website URL Used

The public S3 object URL used for this project is:

```text
https://aditya-miniproject2-s3.s3.ap-southeast-2.amazonaws.com/index.html
```

This URL opens the uploaded `index.html` file directly from the S3 bucket.

---

## 🎉 Final Output

The final output of the assignment is a publicly accessible static website hosted using Amazon S3.

### 🌐 Final Link

```text
https://aditya-miniproject2-s3.s3.ap-southeast-2.amazonaws.com/index.html
```

---

## 📚 Learning Outcome

Through this project, the following AWS concepts were practiced:

* Creating an Amazon S3 bucket 🪣
* Uploading static website files ⬆️
* Understanding bucket names and AWS regions 🌍
* Configuring public access for static files 🔓
* Using a bucket policy for public read permission 📜
* Hosting and opening a static webpage from an S3 URL 🌐

---

## 🏁 Conclusion

This project successfully demonstrates how to create a simple static website and host it using Amazon S3. The website was created with HTML and CSS, uploaded to the `aditya-miniproject2-s3` bucket in the Asia Pacific (Sydney) region, and made accessible through a public S3 URL.
