# Market-Trend-Analysis-Dashboard

## **Repository Description**

A Python-based application designed for analyzing customer reviews in an e-commerce dataset. The system allows the processing of product reviews across different departments (e.g., Dresses, Bottoms, Tops, Intimate, Jackets, and Trend), performs feedback analysis, and provides insightful visualizations for administrative users.

The application facilitates user authentication (both Admin and Employee), adding new employees to the system, extracting customer review data, and categorizing the reviews by product department. Additionally, it generates detailed reports and statistics based on customer ratings, reviews, and feedback.

## **Key Features**

### 1. **User Authentication**
   - **Admin Authentication:** Only authorized users (admin) can log in using their credentials stored in `admin_credentials.txt`.
   - **Employee Authentication:** Employees can log in to access product review data.
   - **Add New Employees:** Admin users have the ability to add new employees, providing a username and password.

### 2. **Data Extraction and Categorization**
   - **Data Extraction:** The system reads a CSV file (`ECommerce_Dataset_converted.csv`) containing customer reviews. Each review is parsed and stored in a list of tuples.
   - **Department Categorization:** Reviews are sorted into different product categories such as Dresses, Bottoms, Tops, Intimate, Jackets, and Trend for easier analysis.

### 3. **Department-Specific Review Display**
   - **Detailed Department Analysis:** Users can choose a department and view a detailed list of customer reviews, including the clothing ID, age of the reviewer, rating, positive feedback count, and department name.

### 4. **Most Reviewed Products**
   - **Bar Chart Visualization:** The system calculates and displays a bar chart showing the number of reviews per department. The categories are sorted in descending order of reviews.

### 5. **Recommendation and Feedback Analysis**
   - **Recommendation Analysis:** The system can analyze positive vs. negative feedback for each department. Positive and negative feedbacks are categorized based on specific rating criteria and plotted in a visual bar chart.
   - **Comparison of Feedback:** Users can compare the results for positive and negative feedback, generating insights into product sentiment.

### 6. **Interactive Interface**
   - The system includes an interactive interface where users can input their choices to navigate through different functionalities, making it intuitive for both admins and employees.

### 7. **Data Visualization**
   - **Matplotlib Integration:** The application uses `matplotlib` to generate visualizations such as bar charts for the most reviewed products and positive/negative feedback comparisons, enhancing the user experience.

---

## **Significance of the System**

### **1. Data-Driven Decision Making**
   This system empowers e-commerce businesses to make data-driven decisions by analyzing customer feedback. The reviews, categorized by department, help identify which product lines perform better in terms of customer satisfaction, allowing for targeted improvements in inventory, marketing, and customer service strategies.

### **2. Enhanced Customer Experience**
   By analyzing customer sentiment (positive vs. negative feedback), businesses can improve customer experience by understanding pain points. Positive feedback can be leveraged in marketing campaigns, while negative feedback provides opportunities for product improvement.

### **3. Efficient Review Management**
   With the ability to categorize and display reviews by department, this system aids in organizing vast amounts of customer feedback efficiently. The system also provides easy access to essential customer insights, helping businesses monitor their products effectively.

### **4. Administrative Control**
   The admin user role is central in ensuring that only authorized users (employees) access and analyze the data. By controlling access to the system, the integrity of data is maintained.

### **5. Visual Analytics**
   The use of bar charts to represent review data visually makes it easier to spot trends and patterns, enhancing decision-making. For example, the `Most Reviewed Products` chart quickly informs users about the product categories that are most frequently reviewed, aiding inventory decisions.

---

## **Technologies Used**

- **Python:** The main programming language for developing the system.
- **Matplotlib:** Used for generating data visualizations (bar charts).
- **CSV:** Used to read and write the product review data.
- **File Handling:** The system reads and writes user credentials and review data to `.txt` and `.csv` files, respectively.
- **User Authentication:** Admin and employee login functionality for secure access.
  
---

## **How to Use**

### **1. Set up the System**
   - Ensure you have Python installed on your system.
   - Clone the repository to your local machine using the following command:
     ```bash
     git clone https://github.com/your-username/e-commerce-review-analysis.git
     ```
   - Install necessary libraries (e.g., `matplotlib`, `pandas`) using pip:
     ```bash
     pip install matplotlib pandas
     ```

### **2. Input Files**
   - Place the required input files (`ECommerce_Dataset_converted.csv`, `emp_credentials.txt`, and `admin_credentials.txt`) in the root directory of the project.

### **3. Running the Program**
   - Run the `main.py` file to start the system:
     ```bash
     python main.py
     ```

### **4. Interacting with the System**
   - Upon running the program, follow the prompts to log in as an admin or employee.
   - Choose options to view department-specific reviews, visualize the most reviewed products, or analyze positive vs. negative feedback.
   - Admin users can add new employee usernames and passwords.

---

## **Future Improvements**

- **User Role Enhancement:** More granular roles (e.g., manager, analyst) with different levels of access and privileges.
- **Advanced Sentiment Analysis:** Implement natural language processing (NLP) techniques to analyze the sentiment of product reviews more accurately.
- **Database Integration:** Transition from CSV to a database for better scalability and performance.
