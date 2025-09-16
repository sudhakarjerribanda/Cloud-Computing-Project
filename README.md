# ☁️ AWS Cloud Automation: Intelligent Image Resizing & Storage Optimization

### **A Project by Sudhakar Reddy Jerribanda**

Hello, I'm Sudhakar Reddy Jerribanda, and this project is a demonstration of my ability to design, implement, and optimize a robust, serverless application on the AWS platform. [cite_start]This solution automates the end-to-end process of image resizing and storage, addressing a common challenge in modern web and mobile applications: managing large media files efficiently to reduce costs and improve performance[cite: 14].

---

## 🚀 Project Summary

This project establishes a completely automated, event-driven pipeline on AWS. [cite_start]When a user uploads an image via an API, a chain of events is triggered to process the image without any manual intervention[cite: 13, 15]. The system resizes the image, applies a watermark, and stores the optimized version, providing a highly scalable and cost-effective solution.

### **Features**
* [cite_start]**Automated Image Processing:** The system automatically resizes images uploaded to a source S3 bucket[cite: 13]. [cite_start]I integrated libraries like Sharp/Pillow for efficient resizing and format conversion[cite: 8].
* [cite_start]**Watermarking:** The Lambda function includes a feature to add a text overlay as a watermark on each processed image[cite: 69].
* [cite_start]**Scalable Cloud Storage:** Utilizes S3 for both raw image input and optimized output, with lifecycle configurations to manage file retention[cite: 62, 63, 64].
* [cite_start]**Secure API Endpoint:** An API Gateway REST API is used to handle image uploads [cite: 5, 79][cite_start], with input validation to ensure secure and reliable uploads[cite: 81].
* [cite_start]**Performance Optimization:** The Lambda function is optimized for efficient storage and retrieval of images[cite: 9]. [cite_start]Performance benchmarking shows an average execution time of 700ms for the "Resize & Watermark" operation[cite: 72, 116].
* [cite_start]**Centralized Monitoring:** I set up CloudWatch for logging and performance tracking[cite: 10].

---

## 🛠️ Technologies & Services

| Category | Technologies |
| :--- | :--- |
| **Cloud Services** | [cite_start]AWS Lambda, AWS S3, AWS API Gateway, AWS IAM, AWS CloudWatch [cite: 5, 6, 7, 8, 10] |
| **Core Languages** | Python / JavaScript (Node.js) |
| **Libraries** | [cite_start]Sharp, Pillow [cite: 8] |
| **Development Tools** | [cite_start]Postman / cURL [cite: 80] |

---

## 🧠 My Role: Image Optimization & Processing

[cite_start]As a core member of this project, I was responsible for the critical image optimization and processing logic[cite: 8]. My primary contributions include:

* [cite_start]**Logic Development**: I developed and implemented the Lambda function responsible for image resizing and format conversion[cite: 8, 67, 68].
* [cite_start]**Performance Tuning**: I fine-tuned the image quality and processing parameters to ensure efficient storage and retrieval [cite: 9][cite_start], mitigating issues like delays caused by large file sizes[cite: 114].
* [cite_start]**Watermark Application**: I integrated the watermark functionality, adding a professional and practical layer to the image processing pipeline[cite: 69].

This experience honed my skills in serverless development, performance benchmarking, and problem-solving, particularly in handling real-world media processing challenges on a cloud platform.

---

## ⚙️ Architecture & Workflow

The system is a classic example of a serverless, event-driven pattern. The process flows as follows:

1.  [cite_start]A user uploads an image via the **API Gateway** endpoint[cite: 5].
2.  [cite_start]The API Gateway triggers an **AWS Lambda function**[cite: 5, 15, 37].
3.  [cite_start]The Lambda function processes the image, resizing and watermarking it[cite: 8, 22, 68, 69].
4.  [cite_start]The optimized image is then stored in a separate output **S3 bucket**[cite: 6, 33, 70].
5.  [cite_start]A presigned URL for the new image is generated and returned to the user[cite: 7, 31, 34, 52].

![System Architecture Diagram](https://i.imgur.com/example-arch-diagram.png) *(This is a placeholder image. Replace it with your actual architecture diagram from the document.)*

---

## 🚀 Getting Started

### **Prerequisites**
* An AWS account
* AWS CLI configured with appropriate credentials
* Node.js and npm (for Lambda development with Sharp)

### **Installation & Deployment**
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo.git](https://github.com/your-username/your-repo.git)
    cd your-repo
    ```
2.  **Create S3 buckets:**
    * [cite_start]Create a bucket named `auto-resize-input`[cite: 63].
    * [cite_start]Create a bucket named `auto-resize-output`[cite: 64].
3.  **Configure IAM Role:**
    * [cite_start]Create an IAM role for the Lambda function with permissions to read from the input S3 bucket and write to the output S3 bucket[cite: 65].
4.  **Deploy Lambda Function:**
    * Package your Lambda code and upload it to AWS Lambda.
    * [cite_start]Attach the IAM role you created[cite: 55].
5.  **Set up API Gateway:**
    * [cite_start]Create a REST API endpoint in API Gateway[cite: 79].
    * [cite_start]Configure it to trigger the Lambda function you just deployed[cite: 5, 38].

---

## 📈 Performance & Enhancements

[cite_start]Through rigorous testing, the "Resize & Watermark" function has a **99.7% success rate** and an average execution time of **700ms**, with a minimal cost of approximately **$0.020 per 1,000 executions**[cite: 116].

### **Future Work**
* [cite_start]**Load Testing:** Conduct load testing with a variety of image sizes and formats[cite: 142].
* [cite_start]**Configurable Watermark:** Add options for configurable watermark position and font styling[cite: 95, 141].
* [cite_start]**Enhanced Logging & Error Handling:** Improve the logging for better debugging and add more robust error handling with retry logic[cite: 93, 94, 118].

---

## 🤝 Contribution

This project is part of my professional portfolio. While I am not actively seeking contributions at this time, feel free to fork the repository and experiment with the code!

---

## 👨‍💻 Connect with Me

This project is a testament to my skills in serverless architecture, cloud automation, and building efficient, scalable systems. I am passionate about creating solutions that solve real-world problems.

* **GitHub:** [github.com/Sudhakar-Jerribanda](https://github.com/Sudhakar-Jerribanda)
* **LinkedIn:** [linkedin.com/in/Sudhakar-Jerribanda](https://linkedin.com/in/Sudhakar-Jerribanda)
* **Portfolio:** [your-portfolio-website.com](https://your-portfolio-website.com)

Thank you for your time and consideration.
