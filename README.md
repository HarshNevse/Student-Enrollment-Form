
# Student Enrollment Form

This project is a web-based **Student Enrollment Form** that allows users to input and manage student information, such as Roll No., Full Name, Class, Birth Date, Address, and Enrollment Date. The project is built using **HTML**, **CSS**, **JavaScript**, and **Bootstrap** for the front-end, while the **JsonPowerDB** API is used as the back-end database for saving and retrieving data.

## Features

- **Form Input**: Users can input student details such as Roll No., Full Name, Class, Birth Date, Address, and Enrollment Date.
- **Save Student Data**: After filling in the form, users can save student records in the JsonPowerDB database.
- **Fetch Existing Data**: Users can retrieve existing student data by entering the Roll No.
- **Update Data**: Users can modify existing student data and save the changes.
- **Reset Form**: The form can be reset to its initial empty state at any time.
- **Responsive Design**: The form is styled using Bootstrap to ensure it looks good on various screen sizes.

## Technology Stack

### Frontend:
- **HTML5**: For structuring the content of the form.
- **CSS3 (Bootstrap)**: For styling and ensuring the form is responsive.
- **JavaScript (jQuery)**: For dynamic interactions and making API calls.

### Backend:
- **JsonPowerDB**: A high-performance, NoSQL, and simple-to-use database that allows easy integration with REST APIs.
  
### API URL:
- **JsonPowerDB API**: `http://api.login2explore.com:5577`

## How to Run the Project

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/student-enrollment-form.git
    ```
   
2. **Open the project**: Navigate to the project directory and open `index.html` in your browser.

3. **Ensure Internet Connection**: Since the project relies on external libraries (Bootstrap, jQuery) and a cloud-based database (JsonPowerDB), it requires an active internet connection.

4. **Using the Form**:
    - Enter a **Roll No.** to retrieve an existing student's information or leave it blank to add a new record.
    - Fill in the required fields: Full Name, Class, Birth Date, Address, and Enrollment Date.
    - Click **Save** to save a new record, or **Change** to update an existing record.
    - Use **Reset** to clear the form.

## How the Code Works

### Key JavaScript Functions:

- `getStudent()`:
  - Retrieves student data based on the Roll No. provided.
  - Uses the JsonPowerDB `GET_BY_KEY` API to fetch records.

- `saveData()`:
  - Validates and saves student data to JsonPowerDB using the `PUT` API.
  
- `changeData()`:
  - Updates the existing student record in the database using the `UPDATE` API.

- `resetForm()`:
  - Resets the form fields and button states.

### Database Information:

- **Database Name**: `SCHOOL-DB`
- **Table Name**: `STUDENT-TABLE`
- **Connection Token**: A token for authenticating with the JsonPowerDB API.

## Dependencies

- **Bootstrap 3.4.1**: For responsive design and styling.
- **jQuery 3.5.1**: For handling DOM manipulation and API requests.
- **JsonPowerDB Commons JS**: For interacting with the JsonPowerDB API.

## JsonPowerDB Documentation

For detailed documentation on how to use JsonPowerDB, visit the official [JsonPowerDB documentation](https://login2explore.com/jpdb/docs.html).

## License

This project is licensed under the MIT License.

---

### Created by Harsh Nevse

