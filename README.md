# NBlog Setup Guide
Welcome to NBlog! Follow these steps to set up the application on your local environment.

<br>

---

## Step 1: Import the Database

1. Navigate to the `database` folder.
2. Import the `blogapplication.sql` file into your local database system.
3. Name the database `blogapplication` to maintain consistency with the application's configuration.

---

## Step 2: Update Spring Application Properties

1. Navigate to `src/main/resources/application.properties`.
2. Update the database credentials (`username` and `password`) to match your local database configuration.
    - This will allow the Spring application to connect to your local database.

---

## Step 3: Configure the Python Script

1. Go to the [nblog-machine-learning](https://github.com/Lsiewchen/nblog-machine-learning.git) repository to retrieve the Python script.
2. Update the database credentials within the script to match your local database username and password.
    - This step is crucial for the Python script to access and interact with your local database.
3. Activate your Python environment and install the required dependencies by running the following command:

    ```bash
    pip install flask SQLAlchemy flask_sqlalchemy scikit-learn numpy
    ```

---

## Step 4: Run the Python Script

1. Execute the Python script.
    - Ensure that it runs successfully as it may perform necessary initializations for the application.

---

## Step 5: Launch and Access NBlog
1. After the Python script has executed, start the Spring application.
    - You can use your IDE or the command line to launch the application.
2. Open your web browser and navigate to `http://localhost:8080/account/create`.
    - You should now be able to use NBlog and explore its features.

---

## Step 6: Run the Android App

1. Go to the [nblog-android](https://github.com/Lsiewchen/nblog-android.git) repository to retrieve the Andriod code.
2. Navigate to `app/src/main/res/values/strings.xml`.
3. Replace the string in `<string name="xuexiao">10.249.155.87</string>` with your IPv4 address.
4. Run the Android app using Android Studio or your preferred IDE.

---

### Final Notes:

Thank you for setting up NBlog! Enjoy using the application and feel free to explore its various features.