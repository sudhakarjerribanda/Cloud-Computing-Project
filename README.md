# ☁️ AWS Cloud Automation: Intelligent Image Resizing & Storage Optimization

### **A Project by Sudhakar Reddy Jerribanda**

Hello, I'm Sudhakar Reddy Jerribanda, and this project is a demonstration of my ability to design, implement, and optimize a robust, serverless application on the AWS platform. This solution automates the end-to-end process of image resizing and storage, addressing a common challenge in modern web and mobile applications: managing large media files efficiently to reduce costs and improve performance.

---

## 🚀 Project Summary

This project establishes a completely automated, event-driven pipeline on AWS. When a user uploads an image via an API, a chain of events is triggered to process the image without any manual intervention. The system resizes the image, applies a watermark, and stores the optimized version, providing a highly scalable and cost-effective solution.

### **Features**
* **Automated Image Processing:** The system automatically resizes images uploaded to a source S3 bucket. The Lambda function utilizes libraries like Sharp/Pillow for efficient resizing and format conversion.
* **Watermarking:** The Lambda function includes a feature to add a text overlay as a watermark on each processed image.
* **Scalable Cloud Storage:** The project uses S3 for both raw image input and optimized output. It's configured with lifecycle rules to manage file retention: 7 days for raw uploads and 30 days for processed files.
* **Secure API Endpoint:** I established a REST API endpoint using API Gateway to handle secure image uploads. Input validation is managed through the Lambda function to ensure reliable uploads.
* **Performance Optimization:** The Lambda function is optimized for efficient storage and retrieval. Performance benchmarking shows the "Resize & Watermark" operation has an average execution time of 700ms.
* **Centralized Monitoring:** I implemented CloudWatch for logging and performance tracking to monitor the system's performance.

---

## 🛠️ Technologies & Services

| Category | Technologies |
| :--- | :--- |
| **Cloud Services** | AWS Lambda, AWS S3, AWS API Gateway, AWS IAM, AWS CloudWatch |
| **Core Languages** | JavaScript (Node.js) |
| **Libraries** | Sharp, Pillow |
| **Development Tools** | Postman / cURL |

---

## 🧠 My Role: Image Optimization & Processing

As a core member of this project, I was responsible for the critical image optimization and processing logic. My primary contributions include:

* **Logic Development**: I developed and implemented the Lambda function responsible for image resizing and format conversion.
* **Performance Tuning**: I fine-tuned the image quality and processing parameters to ensure efficient storage and retrieval, mitigating issues like delays caused by large file sizes.
* **Watermark Application**: I integrated the watermark functionality, adding a professional and practical layer to the image processing pipeline.

This experience honed my skills in serverless development, performance benchmarking, and problem-solving, particularly in handling real-world media processing challenges on a cloud platform.

---

## ⚙️ Architecture & Workflow

The system is a classic example of a serverless, event-driven pattern. The process flows as follows:

1.  A user uploads an image via the **API Gateway** endpoint.
2.  The API Gateway triggers an **AWS Lambda function**.
3.  The Lambda function processes the image, resizing and watermarking it.
4.  The optimized image is then stored in a separate output **S3 bucket**.
5.  A presigned URL for the new image is generated and returned to the user.



[Image of AWS architecture diagram]


---

## 🚀 Getting Started

### **Prerequisites**
* An AWS account
* AWS CLI configured with appropriate credentials
* Node.js and npm (for Lambda development with Sharp)

### **Installation & Deployment**
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sudhakarjerribanda/My_Portfolio.git](https://github.com/sudhakarjerribanda/My_Portfolio.git)
    cd My_Portfolio
    ```
2.  **Create S3 buckets:**
    * Create an input S3 bucket (e.g., `auto-resize-input`).
    * Create an output S3 bucket (e.g., `auto-resize-output`).
3.  **Configure IAM Role:**
    * Create an IAM role for the Lambda function with permissions to read from the input S3 bucket and write to the output S3 bucket.
4.  **Deploy Lambda Function:**
    * Package your Lambda code and upload it to AWS Lambda.
    * Attach the IAM role you created.
5.  **Set up API Gateway:**
    * Create a REST API endpoint in API Gateway to test Lambda manually.
    * Configure it to trigger the Lambda function.

---

## 📈 Performance & Enhancements

Through rigorous testing, the "Resize & Watermark" function has a **99.7% success rate** and an average execution time of **700ms**, with a minimal cost of approximately **$0.020 per 1,000 executions**.

### **Future Work**
* **Load Testing:** Conduct load testing with a variety of image sizes and formats.
* **Configurable Watermark:** Add options for configurable watermark position and font styling.
* **Enhanced Logging & Error Handling:** Improve the logging for better debugging and add more robust error handling with retry logic.

---

## 🤝 Contribution

This project is part of my professional portfolio. While I am not actively seeking contributions at this time, feel free to fork the repository and experiment with the code!

---

## 👨‍💻 Connect with Me

This project is a testament to my skills in serverless architecture, cloud automation, and building efficient, scalable systems. I am passionate about creating solutions that solve real-world problems.

* **GitHub:** [https://github.com/sudhakarjerribanda](https://github.com/sudhakarjerribanda)
* **LinkedIn:** [https://www.linkedin.com/in/sudhakar-reddy-jerribanda-1845381b4/](https://www.linkedin.com/in/sudhakar-reddy-jerribanda-1845381b4/)
* **Portfolio:** [https://github.com/sudhakarjerribanda/My_Portfolio](https://github.com/sudhakarjerribanda/My_Portfolio)

Thank you for your time and consideration.
